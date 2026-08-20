# Replit setup

This is a React 19 + TanStack Start application built with Vite.

## Run locally on Replit

Dependencies are managed with Bun. The configured Replit workflow starts the
development server on the preview port:

```sh
bun run dev -- --host 0.0.0.0 --port 5000
```

## Useful checks

```sh
bun run build
bun run lint
```

Vite is configured to allow Replit's proxied preview hostnames.