# TrackingApp — Gemini Instructions

## 1. Project Overview

TrackingApp is a personal reading tracker for manga, manhwa, manhua, comics, novels, web novels, and books.

The application will allow users to organize their reading libraries, track reading progress, manage ratings and reviews, maintain reading history, record rereads, filter and sort titles, and discover new titles through AI-powered recommendations.

The goal is to build a maintainable, reliable, user-friendly application that demonstrates sound software engineering practices.

## 2. Technology Stack

Use the following technology stack:

- Frontend: React with TypeScript
- Backend: Node.js with Express and TypeScript
- Database: PostgreSQL
- ORM: Prisma
- Version Control: Git and GitHub

Do not introduce additional frameworks, libraries, databases, or services without a clear requirement or explicit approval.

## 3. Development Principles

- Prefer simple, maintainable solutions over unnecessary complexity.
- Use TypeScript and take advantage of its type system.
- Follow established conventions for React, Node.js, Express, and Prisma.
- Keep components, functions, and modules focused on a single responsibility.
- Write reusable code where it improves maintainability.
- Avoid unnecessary abstractions, duplicated logic, and dependencies.
- Keep the application architecture understandable for a developer learning and building the project incrementally.
- Follow consistent naming and formatting conventions.

## 4. Database Guidelines

- Use PostgreSQL as the primary database.
- Use Prisma to define models, relationships, migrations, and database access.
- Design the schema around entities such as users, titles, libraries, reading progress, ratings, reviews, and reading history.
- Use appropriate primary keys, foreign keys, unique constraints, indexes, and validation.
- Maintain data integrity and use transactions when multiple related operations must succeed or fail together.
- Support differences between reading formats without forcing irrelevant fields onto every title.
- Use optional fields, related tables, or PostgreSQL JSONB fields when justified by actual requirements.
- Never store credentials, database passwords, or API keys directly in source code.
- Never apply destructive schema changes or delete existing data without explicit approval.

## 5. Frontend Guidelines

- Build interfaces using React and TypeScript.
- Use functional components and React hooks appropriately.
- Keep UI components focused and reusable.
- Handle loading, empty, error, and success states where relevant.
- Provide clear navigation, accessible controls, and responsive layouts.
- Keep business logic separate from presentation logic when practical.
- Avoid unnecessary state and avoid adding dependencies without justification.

## 6. Backend Guidelines

- Use Express to implement API endpoints.
- Organize routes, controllers, services, and database access according to project complexity.
- Validate incoming data on the server.
- Handle errors consistently and return appropriate HTTP status codes.
- Keep database queries and business logic maintainable.
- Implement authentication and authorization securely when required.
- Do not expose sensitive information in API responses or logs.
- Never trust client-side validation alone.

## 7. AI-Assisted Development Workflow

- Inspect the existing repository and relevant files before making changes.
- Understand the current architecture before proposing implementation details.
- Explain the proposed approach before making substantial or potentially destructive changes.
- Prefer small, focused, reviewable changes.
- Implement only requested features and necessary supporting changes.
- Ask for clarification when requirements are ambiguous or conflict with existing decisions.
- Do not silently change the technology stack, architecture, or project requirements.
- Do not overwrite user work or delete files without permission.
- Explain important technical decisions in clear, concise language.
- Help the developer understand the reasoning behind significant implementation choices.

## 8. Testing and Verification

- Write appropriate tests as the application develops.
- Run relevant tests, linting, type checks, and builds when available.
- Check for regressions after modifying existing functionality.
- Report which checks were actually executed and their results.
- Never claim that code works, builds, or passes tests without appropriate verification.
- If a check cannot be performed, explain why.

## 9. Git and Commit Conventions

Follow the Conventional Commits specification.

Use commit messages in this format:

`type: short description`

Common types include:

- `feat`: introduce a feature
- `fix`: correct a bug
- `docs`: update documentation
- `refactor`: restructure code without changing intended behavior
- `test`: add or update tests
- `chore`: maintenance and tooling changes

Keep commits focused on one logical change. Do not rewrite Git history, bypass branch protection, or push changes without explicit authorization.

## 10. Security and Configuration

- Store local secrets in environment variables.
- Keep `.env` files out of version control.
- Provide an `.env.example` containing placeholder values when needed.
- Validate and sanitize untrusted input appropriately.
- Follow secure authentication, authorization, and database-access practices.
- Never commit API keys, passwords, tokens, or private credentials.
- Respect the repository's LICENSE and its restrictions.

## 11. Project Scope and Feature Priorities

Develop the application incrementally:

1. Establish the project structure and development tooling.
2. Design the database schema and core domain models.
3. Implement title management and personal reading libraries.
4. Implement reading progress, ratings, reviews, and history.
5. Add filtering, sorting, and format-specific tracking.
6. Improve usability, accessibility, testing, and reliability.
7. Introduce AI-powered recommendations when the core functionality is stable.

Treat this list as a high-level roadmap, not authorization to implement every feature immediately.

## 12. General Instructions

- Read the relevant project instructions before starting work.
- Treat the existing repository and approved requirements as the source of truth.
- Prefer official documentation when uncertain about a library or API.
- Do not invent project requirements or assume unfinished features already exist.
- Keep documentation consistent with the actual implementation.
- Ask before introducing major architectural changes, paid services, or new infrastructure.
- Prioritize correctness, maintainability, security, and incremental progress.
