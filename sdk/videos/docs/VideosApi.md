# VideosApi

All URIs are relative to *https://api.rixl.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteVideosVideoIdAudioTracks**](VideosApi.md#deletevideosvideoidaudiotracks) | **DELETE** /videos/{videoId}/audio-tracks | Delete all audio tracks |
| [**deleteVideosVideoIdAudioTracksLangCode**](VideosApi.md#deletevideosvideoidaudiotrackslangcode) | **DELETE** /videos/{videoId}/audio-tracks/{lang_code} | Delete audio track by language |
| [**deleteVideosVideoIdAudioTracksTrackId**](VideosApi.md#deletevideosvideoidaudiotrackstrackid) | **DELETE** /videos/{videoId}/audio-tracks/{trackId} | Delete audio track |
| [**deleteVideosVideoIdChapters**](VideosApi.md#deletevideosvideoidchapters) | **DELETE** /videos/{videoId}/chapters | Delete video chapters |
| [**deleteVideosVideoIdDelete**](VideosApi.md#deletevideosvideoiddelete) | **DELETE** /videos/{videoId}/delete | Delete video |
| [**deleteVideosVideoIdSubtitles**](VideosApi.md#deletevideosvideoidsubtitles) | **DELETE** /videos/{videoId}/subtitles | Delete all subtitles |
| [**deleteVideosVideoIdSubtitlesLangCode**](VideosApi.md#deletevideosvideoidsubtitleslangcode) | **DELETE** /videos/{videoId}/subtitles/{lang_code} | Delete subtitle by language |
| [**deleteVideosVideoIdSubtitlesSubtitleId**](VideosApi.md#deletevideosvideoidsubtitlessubtitleid) | **DELETE** /videos/{videoId}/subtitles/{subtitleId} | Delete subtitle |
| [**getVideos**](VideosApi.md#getvideos) | **GET** /videos | List videos for a project |
| [**getVideosLanguages**](VideosApi.md#getvideoslanguages) | **GET** /videos/languages | List available subtitle languages |
| [**getVideosVideoId**](VideosApi.md#getvideosvideoid) | **GET** /videos/{videoId} | Get a video |
| [**postVideosUploadComplete**](VideosApi.md#postvideosuploadcomplete) | **POST** /videos/upload/complete | Upload: Mark as complete |
| [**postVideosUploadInit**](VideosApi.md#postvideosuploadinit) | **POST** /videos/upload/init | Upload: Init |
| [**postVideosVideoIdAudioTracks**](VideosApi.md#postvideosvideoidaudiotracks) | **POST** /videos/{videoId}/audio-tracks | Bulk upsert video audio tracks |
| [**postVideosVideoIdSubtitles**](VideosApi.md#postvideosvideoidsubtitles) | **POST** /videos/{videoId}/subtitles | Bulk upsert video subtitles |
| [**putVideosVideoIdAudioTracksLangCode**](VideosApi.md#putvideosvideoidaudiotrackslangcode) | **PUT** /videos/{videoId}/audio-tracks/{lang_code} | Upsert video audio track |
| [**putVideosVideoIdChapters**](VideosApi.md#putvideosvideoidchapters) | **PUT** /videos/{videoId}/chapters | Update video chapters |
| [**putVideosVideoIdSubtitlesLangCode**](VideosApi.md#putvideosvideoidsubtitleslangcode) | **PUT** /videos/{videoId}/subtitles/{lang_code} | Upsert video subtitle |
| [**putVideosVideoIdThumbnail**](VideosApi.md#putvideosvideoidthumbnail) | **PUT** /videos/{videoId}/thumbnail | Update video thumbnail |



## deleteVideosVideoIdAudioTracks

> AudioTrackDelete deleteVideosVideoIdAudioTracks(videoId)

Delete all audio tracks

Remove all additional audio tracks from a video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdAudioTracksRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
  } satisfies DeleteVideosVideoIdAudioTracksRequest;

  try {
    const data = await api.deleteVideosVideoIdAudioTracks(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |

### Return type

[**AudioTrackDelete**](AudioTrackDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdAudioTracksLangCode

> AudioTrackDelete deleteVideosVideoIdAudioTracksLangCode(videoId, langCode)

Delete audio track by language

Remove an audio track for a specific language using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdAudioTracksLangCodeRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Language Code (BCP 47)
    langCode: langCode_example,
  } satisfies DeleteVideosVideoIdAudioTracksLangCodeRequest;

  try {
    const data = await api.deleteVideosVideoIdAudioTracksLangCode(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **langCode** | `string` | Language Code (BCP 47) | [Defaults to `undefined`] |

### Return type

[**AudioTrackDelete**](AudioTrackDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdAudioTracksTrackId

> AudioTrackDelete deleteVideosVideoIdAudioTracksTrackId(videoId, trackId)

Delete audio track

Remove an additional audio track from a video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdAudioTracksTrackIdRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Audio Track ID
    trackId: trackId_example,
  } satisfies DeleteVideosVideoIdAudioTracksTrackIdRequest;

  try {
    const data = await api.deleteVideosVideoIdAudioTracksTrackId(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **trackId** | `string` | Audio Track ID | [Defaults to `undefined`] |

### Return type

[**AudioTrackDelete**](AudioTrackDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |
| **500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdChapters

> UpdateChaptersResponse deleteVideosVideoIdChapters(videoId)

Delete video chapters

Remove all chapters from a video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdChaptersRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
  } satisfies DeleteVideosVideoIdChaptersRequest;

  try {
    const data = await api.deleteVideosVideoIdChapters(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |

### Return type

[**UpdateChaptersResponse**](UpdateChaptersResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized - Invalid API key |  -  |
| **403** | Access denied |  -  |
| **404** | Video not found |  -  |
| **500** | Failed to delete chapters |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdDelete

> deleteVideosVideoIdDelete(videoId)

Delete video

Delete a video by its ID within a project

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdDeleteRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
  } satisfies DeleteVideosVideoIdDeleteRequest;

  try {
    const data = await api.deleteVideosVideoIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Video deleted successfully |  -  |
| **400** | Invalid project ID or video ID |  -  |
| **401** | Unauthorized |  -  |
| **403** | Access denied |  -  |
| **404** | Video not found |  -  |
| **500** | Failed to delete video |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdSubtitles

> SubtitleDelete deleteVideosVideoIdSubtitles(videoId)

Delete all subtitles

Remove all subtitles from a video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdSubtitlesRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
  } satisfies DeleteVideosVideoIdSubtitlesRequest;

  try {
    const data = await api.deleteVideosVideoIdSubtitles(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |

### Return type

[**SubtitleDelete**](SubtitleDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdSubtitlesLangCode

> SubtitleDelete deleteVideosVideoIdSubtitlesLangCode(videoId, langCode)

Delete subtitle by language

Remove a subtitle for a specific language using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdSubtitlesLangCodeRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Language Code (BCP 47)
    langCode: langCode_example,
  } satisfies DeleteVideosVideoIdSubtitlesLangCodeRequest;

  try {
    const data = await api.deleteVideosVideoIdSubtitlesLangCode(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **langCode** | `string` | Language Code (BCP 47) | [Defaults to `undefined`] |

### Return type

[**SubtitleDelete**](SubtitleDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteVideosVideoIdSubtitlesSubtitleId

> SubtitleDelete deleteVideosVideoIdSubtitlesSubtitleId(videoId, subtitleId)

Delete subtitle

Remove a subtitle from a video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { DeleteVideosVideoIdSubtitlesSubtitleIdRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Subtitle ID
    subtitleId: subtitleId_example,
  } satisfies DeleteVideosVideoIdSubtitlesSubtitleIdRequest;

  try {
    const data = await api.deleteVideosVideoIdSubtitlesSubtitleId(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **subtitleId** | `string` | Subtitle ID | [Defaults to `undefined`] |

### Return type

[**SubtitleDelete**](SubtitleDelete.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `*/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |
| **500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getVideos

> PaginationPaginatedResponseVideo getVideos(limit, offset, sort, order)

List videos for a project

Retrieve all videos for a specific project, with pagination and sorting.

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { GetVideosRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // number | Maximum number of items to return in a single request. <br> **Default:** `25` (optional)
    limit: 56,
    // number | Starting point of the result set. <br>To get page 2 with a limit of 25, set `offset` to `25`. <br> **Default:** `0` (optional)
    offset: 56,
    // string | Field to sort by (created_at, name, size, updated_at, duration) (optional)
    sort: sort_example,
    // string | Sort order (asc, desc) (optional)
    order: order_example,
  } satisfies GetVideosRequest;

  try {
    const data = await api.getVideos(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **limit** | `number` | Maximum number of items to return in a single request. &lt;br&gt; **Default:** &#x60;25&#x60; | [Optional] [Defaults to `25`] |
| **offset** | `number` | Starting point of the result set. &lt;br&gt;To get page 2 with a limit of 25, set &#x60;offset&#x60; to &#x60;25&#x60;. &lt;br&gt; **Default:** &#x60;0&#x60; | [Optional] [Defaults to `0`] |
| **sort** | `string` | Field to sort by (created_at, name, size, updated_at, duration) | [Optional] [Defaults to `undefined`] |
| **order** | `string` | Sort order (asc, desc) | [Optional] [Defaults to `undefined`] |

### Return type

[**PaginationPaginatedResponseVideo**](PaginationPaginatedResponseVideo.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid query parameters |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getVideosLanguages

> Array&lt;InternalVideosHandlerSubtitlesLanguageResponse&gt; getVideosLanguages()

List available subtitle languages

Get list of supported languages for subtitles

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { GetVideosLanguagesRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const api = new VideosApi();

  try {
    const data = await api.getVideosLanguages();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;InternalVideosHandlerSubtitlesLanguageResponse&gt;**](InternalVideosHandlerSubtitlesLanguageResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getVideosVideoId

> Video getVideosVideoId(videoId)

Get a video

Retrieve a video by its ID for a specific project.

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { GetVideosVideoIdRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
  } satisfies GetVideosVideoIdRequest;

  try {
    const data = await api.getVideosVideoId(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |

### Return type

[**Video**](Video.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid video ID |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Video not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postVideosUploadComplete

> Video postVideosUploadComplete(request)

Upload: Mark as complete

Mark a video upload as complete after successful upload to storage using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PostVideosUploadCompleteRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // GithubComQeeqezApiInternalVideosHandlerUploadCompleteRequest | Video upload completion request
    request: ...,
  } satisfies PostVideosUploadCompleteRequest;

  try {
    const data = await api.postVideosUploadComplete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **request** | [GithubComQeeqezApiInternalVideosHandlerUploadCompleteRequest](GithubComQeeqezApiInternalVideosHandlerUploadCompleteRequest.md) | Video upload completion request | |

### Return type

[**Video**](Video.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid request body |  -  |
| **401** | Unauthorized - Invalid API key |  -  |
| **403** | Access denied |  -  |
| **404** | File not found |  -  |
| **500** | Failed to complete upload |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postVideosUploadInit

> GithubComQeeqezApiInternalVideosHandlerUploadInitResponse postVideosUploadInit(request)

Upload: Init

Initialize a video upload and get presigned URLs for video and poster using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PostVideosUploadInitRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // VideoUploadInitRequest | Video upload initialization request
    request: ...,
  } satisfies PostVideosUploadInitRequest;

  try {
    const data = await api.postVideosUploadInit(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **request** | [VideoUploadInitRequest](VideoUploadInitRequest.md) | Video upload initialization request | |

### Return type

[**GithubComQeeqezApiInternalVideosHandlerUploadInitResponse**](GithubComQeeqezApiInternalVideosHandlerUploadInitResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid request body |  -  |
| **401** | Unauthorized - Invalid API key |  -  |
| **403** | Access denied |  -  |
| **500** | Failed to initialize upload |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postVideosVideoIdAudioTracks

> Array&lt;AudioTrack&gt; postVideosVideoIdAudioTracks(videoId, files, languageCodes, labels)

Bulk upsert video audio tracks

Replace all audio tracks with the provided ones using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PostVideosVideoIdAudioTracksRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // Array<Blob> | Audio files (.mp3, .opus, .flac, .wav, .ac3, .m4a, .aac)
    files: /path/to/file.txt,
    // string | Comma-separated language codes
    languageCodes: languageCodes_example,
    // string | Comma-separated labels
    labels: labels_example,
  } satisfies PostVideosVideoIdAudioTracksRequest;

  try {
    const data = await api.postVideosVideoIdAudioTracks(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **files** | `Array<Blob>` | Audio files (.mp3, .opus, .flac, .wav, .ac3, .m4a, .aac) | |
| **languageCodes** | `string` | Comma-separated language codes | [Defaults to `undefined`] |
| **labels** | `string` | Comma-separated labels | [Defaults to `undefined`] |

### Return type

[**Array&lt;AudioTrack&gt;**](AudioTrack.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postVideosVideoIdSubtitles

> Array&lt;Subtitle&gt; postVideosVideoIdSubtitles(videoId, files, languageCodes, labels)

Bulk upsert video subtitles

Replace all subtitles with the provided ones using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PostVideosVideoIdSubtitlesRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // Array<Blob> | Subtitle files (.srt or .vtt)
    files: /path/to/file.txt,
    // string | Comma-separated language codes
    languageCodes: languageCodes_example,
    // string | Comma-separated labels
    labels: labels_example,
  } satisfies PostVideosVideoIdSubtitlesRequest;

  try {
    const data = await api.postVideosVideoIdSubtitles(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **files** | `Array<Blob>` | Subtitle files (.srt or .vtt) | |
| **languageCodes** | `string` | Comma-separated language codes | [Defaults to `undefined`] |
| **labels** | `string` | Comma-separated labels | [Defaults to `undefined`] |

### Return type

[**Array&lt;Subtitle&gt;**](Subtitle.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## putVideosVideoIdAudioTracksLangCode

> AudioTrack putVideosVideoIdAudioTracksLangCode(videoId, langCode, file, label)

Upsert video audio track

Add or replace an audio track for a specific language using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PutVideosVideoIdAudioTracksLangCodeRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Language Code (BCP 47)
    langCode: langCode_example,
    // Blob | Audio file (.mp3, .opus, .flac, .wav, .ac3, .m4a, .aac)
    file: BINARY_DATA_HERE,
    // string | Label (e.g. English) (optional)
    label: label_example,
  } satisfies PutVideosVideoIdAudioTracksLangCodeRequest;

  try {
    const data = await api.putVideosVideoIdAudioTracksLangCode(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **langCode** | `string` | Language Code (BCP 47) | [Defaults to `undefined`] |
| **file** | `Blob` | Audio file (.mp3, .opus, .flac, .wav, .ac3, .m4a, .aac) | [Defaults to `undefined`] |
| **label** | `string` | Label (e.g. English) | [Optional] [Defaults to `undefined`] |

### Return type

[**AudioTrack**](AudioTrack.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## putVideosVideoIdChapters

> UpdateChaptersResponse putVideosVideoIdChapters(videoId, request)

Update video chapters

Replace all chapters for a video (atomic PUT operation) using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PutVideosVideoIdChaptersRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // UpdateChaptersRequest | Chapters array
    request: ...,
  } satisfies PutVideosVideoIdChaptersRequest;

  try {
    const data = await api.putVideosVideoIdChapters(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **request** | [UpdateChaptersRequest](UpdateChaptersRequest.md) | Chapters array | |

### Return type

[**UpdateChaptersResponse**](UpdateChaptersResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid request body or video duration not available |  -  |
| **401** | Unauthorized - Invalid API key |  -  |
| **403** | Access denied |  -  |
| **404** | Video not found |  -  |
| **500** | Failed to update chapters |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## putVideosVideoIdSubtitlesLangCode

> Subtitle putVideosVideoIdSubtitlesLangCode(videoId, langCode, file, label)

Upsert video subtitle

Add or replace a subtitle for a specific language using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PutVideosVideoIdSubtitlesLangCodeRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // string | Language Code (BCP 47)
    langCode: langCode_example,
    // Blob | Subtitle file (.srt or .vtt)
    file: BINARY_DATA_HERE,
    // string | Label (e.g. English) (optional)
    label: label_example,
  } satisfies PutVideosVideoIdSubtitlesLangCodeRequest;

  try {
    const data = await api.putVideosVideoIdSubtitlesLangCode(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **langCode** | `string` | Language Code (BCP 47) | [Defaults to `undefined`] |
| **file** | `Blob` | Subtitle file (.srt or .vtt) | [Defaults to `undefined`] |
| **label** | `string` | Label (e.g. English) | [Optional] [Defaults to `undefined`] |

### Return type

[**Subtitle**](Subtitle.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## putVideosVideoIdThumbnail

> Video putVideosVideoIdThumbnail(videoId, thumbnail)

Update video thumbnail

Update the thumbnail image for an existing video using API key authentication

### Example

```ts
import {
  Configuration,
  VideosApi,
} from '@rixl/sdk-typescript-videos';
import type { PutVideosVideoIdThumbnailRequest } from '@rixl/sdk-typescript-videos';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-videos SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VideosApi(config);

  const body = {
    // string | Video ID
    videoId: videoId_example,
    // Blob | Thumbnail image file (max 5MB, image/_*)
    thumbnail: BINARY_DATA_HERE,
  } satisfies PutVideosVideoIdThumbnailRequest;

  try {
    const data = await api.putVideosVideoIdThumbnail(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **videoId** | `string` | Video ID | [Defaults to `undefined`] |
| **thumbnail** | `Blob` | Thumbnail image file (max 5MB, image/_*) | [Defaults to `undefined`] |

### Return type

[**Video**](Video.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Video with updated thumbnail |  -  |
| **400** | Invalid file or request |  -  |
| **401** | Unauthorized - Invalid API key |  -  |
| **403** | Access denied |  -  |
| **404** | Video not found |  -  |
| **500** | Upload or update failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

