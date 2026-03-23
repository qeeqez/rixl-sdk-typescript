
# PaginationPagination


## Properties

Name | Type
------------ | -------------
`limit` | number
`offset` | number
`total` | number

## Example

```typescript
import type { PaginationPagination } from '@rixl/sdk-typescript-images'

// TODO: Update the object below with actual values
const example = {
  "limit": 100,
  "offset": 50,
  "total": 1000,
} satisfies PaginationPagination

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaginationPagination
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


