# Development environment

How to start the project. This is the page the agent must find when asked
"how do I start the project?".

Write commands exactly as they are typed. If a command differs on Windows,
give both versions.

## Requirements

- Docker and Docker Compose (e.g. Docker Desktop)
- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Note: Node and Yarn are not installed on the host; they run only in the container.

## Start

Start the application container in the background:

```sh
docker compose up -d
```

On Windows (cmd / PowerShell):

```cmd
docker compose up -d
```

Or run in the foreground to view logs directly:

```sh
docker compose up
```

The application is available at:

http://localhost:5173

## Stop

Stop the application container:

```sh
docker compose down
```

On Windows (cmd / PowerShell):

```cmd
docker compose down
```

(Or press `Ctrl + C` if running in the foreground).

## Running Yarn commands

Node and Yarn run only inside the container. To run any Yarn command, use `docker compose exec app`:

```sh
docker compose exec app yarn <command>
```

On Windows (cmd / PowerShell):

```cmd
docker compose exec app yarn <command>
```

Examples:

```sh
docker compose exec app yarn build
docker compose exec app yarn install
```

## Common problems

- Port 5173 is already in use: ensure no other process or container is using port 5173.
- Docker daemon is not running: start Docker Desktop before running compose commands.
