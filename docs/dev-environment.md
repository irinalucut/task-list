# Development environment

How to start the project. This is the page the agent must find when asked
"how do I start the project?".

Write commands exactly as they are typed. If a command differs on Windows,
give both versions.

## Requirements

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Optional: a simple local static server (e.g. VS Code Live Server or `npx serve`)

## Start

Open `index.html` or `login.html` directly in the browser:

```sh
open login.html
```

On Windows:

```cmd
start login.html
```

Or using any static HTTP server:

```sh
npx serve .
```

## Stop

Close the browser tab or press `Ctrl + C` in the static server terminal.

## Common problems

- Styles not loading offline: ensure an active internet connection if Tailwind CDN is used.
