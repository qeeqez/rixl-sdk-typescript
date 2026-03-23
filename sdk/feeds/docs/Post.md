
# Post


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`creatorId` | string
`description` | string
`feedId` | string
`id` | string
`image` | [Image](Image.md)
`planType` | [GithubComQeeqezApiDbSqlcPlanType](GithubComQeeqezApiDbSqlcPlanType.md)
`type` | [PostType](PostType.md)
`updatedAt` | string
`video` | [GithubComQeeqezApiInternalVideosVideoResponse](GithubComQeeqezApiInternalVideosVideoResponse.md)

## Example

```typescript
import type { Post } from '@rixl/sdk-typescript-feeds'

// TODO: Update the object below with actual values
const example = {
  "createdAt": 2025-01-01T00:00:00Z,
  "creatorId": CR8y3QB38S,
  "description": My awesome post,
  "feedId": FD4y3QB38S,
  "id": PS5IMKoFLm,
  "image": null,
  "planType": null,
  "type": null,
  "updatedAt": 2025-01-01T00:00:00Z,
  "video": null,
} satisfies Post

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Post
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


