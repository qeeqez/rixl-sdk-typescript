
# UpdateChaptersResponse


## Properties

Name | Type
------------ | -------------
`chapters` | [Array&lt;Chapter&gt;](Chapter.md)
`videoId` | string

## Example

```typescript
import type { UpdateChaptersResponse } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "chapters": null,
  "videoId": x8n2p5v9k7,
} satisfies UpdateChaptersResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UpdateChaptersResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


