
# Subtitle


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`id` | string
`label` | string
`languageCode` | string
`name` | string
`size` | number
`url` | string
`videoId` | string

## Example

```typescript
import type { Subtitle } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "createdAt": 2025-12-21T12:00:00Z,
  "id": 5m9k8p2v7q,
  "label": English,
  "languageCode": en-US,
  "name": english_subs.srt,
  "size": 1024,
  "url": https://cdn.rixl.io/subtitles/project_id/video_id/en-US-5m9k8p2v7q.srt,
  "videoId": x8n2p5v9k7,
} satisfies Subtitle

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Subtitle
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


