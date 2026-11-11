# Decisions

Why things are the way they are. Read this before reopening a decision.
Newest first. One entry per decision; do not rewrite old entries, add a new
one that replaces them.

## Entry format

```
## YYYY-MM-DD: short title
Decision: what was decided, in one sentence.
Why: the reason, and what it costs.
Rejected: the alternatives considered and why they lost.
```

## Entries

## 2026-11-11: Client-side architecture without API
Decision: Build the application entirely client-side without a backend API or complex build tooling.
Why: Lightweight, runs directly in the browser, fast to iterate for course exercises.
Rejected: Backend server/API setup (unnecessary complexity for the current scope).

## 2026-11-11: Styling with Tailwind CSS
Decision: Use Tailwind CSS for interface styling.
Why: Rapid UI prototyping with consistent design directly in markup.
Rejected: Plain custom CSS (harder to maintain consistency) and heavy component libraries.
