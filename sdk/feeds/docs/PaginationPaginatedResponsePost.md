
# PaginationPaginatedResponsePost


## Properties

Name | Type
------------ | -------------
`data` | [Array&lt;Post&gt;](Post.md)
`pagination` | [PaginationPagination](PaginationPagination.md)

## Example

```typescript
import type { PaginationPaginatedResponsePost } from '@rixl/sdk-typescript-feeds'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "pagination": null,
} satisfies PaginationPaginatedResponsePost

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaginationPaginatedResponsePost
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


