
# Image


## Properties

Name | Type
------------ | -------------
`attachedToVideo` | boolean
`file` | any
`height` | number
`id` | string
`thumbhash` | string
`width` | number

## Example

```typescript
import type { Image } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "attachedToVideo": false,
  "file": null,
  "height": 1080,
  "id": PS5IMKoFLm,
  "thumbhash": 1QcSHQRnh493V4dIh4eXh1h4kJUI,
  "width": 1920,
} satisfies Image

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Image
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


