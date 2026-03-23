
# InternalImagesHandlerInitResponse


## Properties

Name | Type
------------ | -------------
`imageId` | string
`presignedUrl` | string
`uploadExpires` | number

## Example

```typescript
import type { InternalImagesHandlerInitResponse } from '@rixl/sdk-typescript-images'

// TODO: Update the object below with actual values
const example = {
  "imageId": PS5IMKoFLm,
  "presignedUrl": https://images.rixl.com/Bq4y3QB38S/PS5IMKoFLm?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAEXAMPLE%2F20250831%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250831T103000Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=b228dbec8c1008c80c162e1210e4503dceead1e4d4751b4d9787314fd6da4d55,
  "uploadExpires": 1640995200,
} satisfies InternalImagesHandlerInitResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as InternalImagesHandlerInitResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


