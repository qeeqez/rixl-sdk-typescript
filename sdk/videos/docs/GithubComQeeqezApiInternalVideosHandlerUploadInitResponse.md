
# GithubComQeeqezApiInternalVideosHandlerUploadInitResponse


## Properties

Name | Type
------------ | -------------
`posterId` | string
`posterPresignedUrl` | string
`uploadExpires` | number
`videoId` | string
`videoPresignedUrl` | string

## Example

```typescript
import type { GithubComQeeqezApiInternalVideosHandlerUploadInitResponse } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "posterId": PS5IMKoFLm,
  "posterPresignedUrl": https://images.rixl.com/Bq4y3QB38S/PS5IMKoFLm?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAEXAMPLE%2F20250831%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250831T103000Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=b228dbec8c1008c80c162e1210e4503dceead1e4d4d55,
  "uploadExpires": 1640995200,
  "videoId": VI9VXQxWXQ,
  "videoPresignedUrl": https://videos.rixl.com/Bq4y3QB38S/VI9VXQxWXQ?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAEXAMPLE%2F20250831%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250831T103000Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=b228dbec8c1008c80c162e1210e4503dceead1e4d4d55,
} satisfies GithubComQeeqezApiInternalVideosHandlerUploadInitResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GithubComQeeqezApiInternalVideosHandlerUploadInitResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


