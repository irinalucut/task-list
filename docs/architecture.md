# Architecture

How the main parts connect. Read this before adding a module or changing how
parts talk to each other. Describe the shape, not every file.

## Parts

- Frontend UI: Standalone client pages (Login, Task List, Admin) styled with Tailwind CSS.
- Client Auth & State: Client-side session and data management in localStorage (no backend API).
- Task Management: In-browser CRUD operations for tasks.
- Admin Section: User management interface for administrator role.

## How they connect

- UI events update local state and browser storage directly without an external API.

## Data

- Stored in browser localStorage (user accounts, current session, tasks list).

## What does not belong here

How to start the project (docs/dev-environment.md) and why a choice was made
(docs/decisions.md).
