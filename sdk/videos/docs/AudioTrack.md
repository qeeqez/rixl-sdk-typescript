
# AudioTrack


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`format` | string
`id` | string
`label` | string
`languageCode` | string
`name` | string
`size` | number
`url` | string
`videoId` | string

## Example

```typescript
import type { AudioTrack } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "createdAt": 2025-12-21T12:00:00Z,
  "format": mp3,
  "id": 3n7v9k4m2p,
  "label": Spanish,
  "languageCode": es-ES,
  "name": spanish_audio.mp3,
  "size": 2048576,
  "url": https://cdn.rixl.io/audio_tracks/project_id/video_id/es-ES-3n7v9k4m2p.mp3,
  "videoId": x8n2p5v9k7,
} satisfies AudioTrack

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AudioTrack
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


