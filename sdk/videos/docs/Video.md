
# Video


## Properties

Name | Type
------------ | -------------
`bitrate` | number
`chapters` | [Array&lt;Chapter&gt;](Chapter.md)
`codec` | string
`duration` | number
`file` | any
`framerate` | string
`hdr` | boolean
`height` | number
`id` | string
`planType` | [GithubComQeeqezApiDbSqlcPlanType](GithubComQeeqezApiDbSqlcPlanType.md)
`poster` | [Image](Image.md)
`width` | number

## Example

```typescript
import type { Video } from '@rixl/sdk-typescript-videos'

// TODO: Update the object below with actual values
const example = {
  "bitrate": null,
  "chapters": null,
  "codec": null,
  "duration": null,
  "file": null,
  "framerate": null,
  "hdr": null,
  "height": null,
  "id": null,
  "planType": null,
  "poster": null,
  "width": null,
} satisfies Video

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Video
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


