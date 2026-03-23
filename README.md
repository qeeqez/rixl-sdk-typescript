# RIXL TypeScript SDK

The RIXL TypeScript SDK provides full type safety and a modern developer experience for integrating RIXL services into your web and server-side applications.

## Services

The SDK is organized into standalone service packages:

- **@rixl/sdk-typescript-feeds**: Content and user feed management.
- **@rixl/sdk-typescript-videos**: End-to-end video lifecycle management.
- **@rixl/sdk-typescript-images**: High-speed image uploads and transformations.

## Installation

Install the desired packages using npm or yarn:

```bash
npm install @rixl/sdk-typescript-feeds @rixl/sdk-typescript-videos @rixl/sdk-typescript-images
```

## Example Usage

```typescript
import { FeedsApi } from '@rixl/sdk-typescript-feeds';

const feeds = new FeedsApi();
// const res = await feeds.getFeed();
```

## Support

Please report any issues via the GitHub Issue tracker.
