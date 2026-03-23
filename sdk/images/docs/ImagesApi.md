# ImagesApi

All URIs are relative to *https://api.rixl.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**deleteImagesImageId**](ImagesApi.md#deleteimagesimageid) | **DELETE** /images/{imageId} | Delete image |
| [**getImages**](ImagesApi.md#getimages) | **GET** /images | List images for a project |
| [**getImagesImageId**](ImagesApi.md#getimagesimageid) | **GET** /images/{imageId} | Get image |
| [**postImagesUploadComplete**](ImagesApi.md#postimagesuploadcomplete) | **POST** /images/upload/complete | Upload: Mark as complete |
| [**postImagesUploadInit**](ImagesApi.md#postimagesuploadinit) | **POST** /images/upload/init | Upload: Init |



## deleteImagesImageId

> deleteImagesImageId(imageId)

Delete image

delete an image by marking it as deleted

### Example

```ts
import {
  Configuration,
  ImagesApi,
} from '@rixl/sdk-typescript-images';
import type { DeleteImagesImageIdRequest } from '@rixl/sdk-typescript-images';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-images SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ImagesApi(config);

  const body = {
    // string | Image ID
    imageId: imageId_example,
  } satisfies DeleteImagesImageIdRequest;

  try {
    const data = await api.deleteImagesImageId(body);
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
| **imageId** | `string` | Image ID | [Defaults to `undefined`] |

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
| **204** | Image deleted successfully |  -  |
| **400** | Invalid project ID or image ID |  -  |
| **401** | Unauthorized |  -  |
| **403** | Access denied |  -  |
| **404** | Image not found |  -  |
| **500** | Failed to delete image |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getImages

> PaginationPaginatedResponseImage getImages(limit, offset, sort, order)

List images for a project

Retrieve all images for a specific project, with pagination and sorting.

### Example

```ts
import {
  Configuration,
  ImagesApi,
} from '@rixl/sdk-typescript-images';
import type { GetImagesRequest } from '@rixl/sdk-typescript-images';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-images SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ImagesApi(config);

  const body = {
    // number | Maximum number of items to return in a single request. <br> **Default:** `25` (optional)
    limit: 56,
    // number | Starting point of the result set. <br>To get page 2 with a limit of 25, set `offset` to `25`. <br> **Default:** `0` (optional)
    offset: 56,
    // string | Field to sort by (created_at, name, size, updated_at) (optional)
    sort: sort_example,
    // string | Sort order (asc, desc) (optional)
    order: order_example,
  } satisfies GetImagesRequest;

  try {
    const data = await api.getImages(body);
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
| **sort** | `string` | Field to sort by (created_at, name, size, updated_at) | [Optional] [Defaults to `undefined`] |
| **order** | `string` | Sort order (asc, desc) | [Optional] [Defaults to `undefined`] |

### Return type

[**PaginationPaginatedResponseImage**](PaginationPaginatedResponseImage.md)

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


## getImagesImageId

> Image getImagesImageId(imageId)

Get image

Retrieve an image by its ID for a specific project.

### Example

```ts
import {
  Configuration,
  ImagesApi,
} from '@rixl/sdk-typescript-images';
import type { GetImagesImageIdRequest } from '@rixl/sdk-typescript-images';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-images SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ImagesApi(config);

  const body = {
    // string | Image ID
    imageId: imageId_example,
  } satisfies GetImagesImageIdRequest;

  try {
    const data = await api.getImagesImageId(body);
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
| **imageId** | `string` | Image ID | [Defaults to `undefined`] |

### Return type

[**Image**](Image.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid image ID |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Image not found |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postImagesUploadComplete

> Image postImagesUploadComplete(request)

Upload: Mark as complete

Complete the upload process and create the image record using API key authentication

### Example

```ts
import {
  Configuration,
  ImagesApi,
} from '@rixl/sdk-typescript-images';
import type { PostImagesUploadCompleteRequest } from '@rixl/sdk-typescript-images';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-images SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ImagesApi(config);

  const body = {
    // InternalImagesHandlerCompleteRequest | Upload completion request
    request: ...,
  } satisfies PostImagesUploadCompleteRequest;

  try {
    const data = await api.postImagesUploadComplete(body);
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
| **request** | [InternalImagesHandlerCompleteRequest](InternalImagesHandlerCompleteRequest.md) | Upload completion request | |

### Return type

[**Image**](Image.md)

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
| **500** | Failed to complete upload or create image |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postImagesUploadInit

> InternalImagesHandlerInitResponse postImagesUploadInit(request)

Upload: Init

Initialize a presigned URL upload for an image file using API key authentication

### Example

```ts
import {
  Configuration,
  ImagesApi,
} from '@rixl/sdk-typescript-images';
import type { PostImagesUploadInitRequest } from '@rixl/sdk-typescript-images';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-images SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new ImagesApi(config);

  const body = {
    // InternalImagesHandlerUploadInitRequest | Upload initialization request
    request: ...,
  } satisfies PostImagesUploadInitRequest;

  try {
    const data = await api.postImagesUploadInit(body);
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
| **request** | [InternalImagesHandlerUploadInitRequest](InternalImagesHandlerUploadInitRequest.md) | Upload initialization request | |

### Return type

[**InternalImagesHandlerInitResponse**](InternalImagesHandlerInitResponse.md)

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

