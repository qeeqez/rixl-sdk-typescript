
# VideoUploadInitRequest


## Properties

Name | Type
------------ | -------------
`fileName` | string
`imageFormat` | string
`videoQuality` | [GithubComQeeqezApiDbSqlcVideoQuality](GithubComQeeqezApiDbSqlcVideoQuality.md)

## Example

```typescript
import type { VideoUploadInitRequest } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "fileName": my-video.mp4,
  "imageFormat": jpg,
  "videoQuality": null,
} satisfies VideoUploadInitRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VideoUploadInitRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


