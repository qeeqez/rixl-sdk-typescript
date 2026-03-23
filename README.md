# RIXL TypeScript SDKs

This repository contains the TypeScript SDK split by service instead of one flat generated client.

## Layout

- `sdk/feeds` -> package `@rixl/sdk-typescript-feeds`
- `sdk/videos` -> package `@rixl/sdk-typescript-videos`
- `sdk/images` -> package `@rixl/sdk-typescript-images`

Each service folder is a standalone generated package with its own `package.json`, `tsconfig.json`, and `src` directory.

## Build Example

Build the videos SDK:

```sh
cd sdk/videos
npm install
npm run build
```

## Regenerate

Generate all services:

```sh
./scripts/generate.sh
```

Generate one service:

```sh
./scripts/generate.sh --service videos
```

Regenerate from a fresh OpenAPI file:

```sh
./scripts/generate.sh --spec /path/to/public.swagger.json --service images
```
