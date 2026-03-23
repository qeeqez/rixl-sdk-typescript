
# ModelFile


## Properties

Name | Type
------------ | -------------
`createdAt` | string
`format` | string
`id` | string
`name` | string
`projectId` | string
`size` | number
`status` | [FileStatus](FileStatus.md)
`updatedAt` | string
`url` | string

## Example

```typescript
import type { ModelFile } from '@rixl/sdk-typescript-feeds'

// TODO: Update the object below with actual values
const example = {
  "createdAt": 2025-01-01T00:00:00Z,
  "format": avif,
  "id": FpvLwyDMqu,
  "name": original.jpeg,
  "projectId": Bq4y3QB38S,
  "size": 1048576,
  "status": null,
  "updatedAt": 2025-01-01T00:00:00Z,
  "url": https://images.rixl.com/Bq4y3QB38S/FpvLwyDMqu,
} satisfies ModelFile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ModelFile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


