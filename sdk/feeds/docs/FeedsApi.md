# FeedsApi

All URIs are relative to *https://api.rixl.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getFeedsFeedId**](FeedsApi.md#getfeedsfeedid) | **GET** /feeds/{feedId} | List posts in a feed |
| [**getFeedsFeedIdCreatorsCreatorId**](FeedsApi.md#getfeedsfeedidcreatorscreatorid) | **GET** /feeds/{feedId}/creators/{creatorId} | List posts by creator |
| [**getFeedsFeedIdPostId**](FeedsApi.md#getfeedsfeedidpostid) | **GET** /feeds/{feedId}/{postId} | Get a post |



## getFeedsFeedId

> PaginationPaginatedResponsePost getFeedsFeedId(feedId, limit, offset)

List posts in a feed

Retrieve posts in a feed, with pagination.

### Example

```ts
import {
  Configuration,
  FeedsApi,
} from '@rixl/sdk-typescript-feeds';
import type { GetFeedsFeedIdRequest } from '@rixl/sdk-typescript-feeds';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-feeds SDK...");
  const api = new FeedsApi();

  const body = {
    // string | Feed ID
    feedId: feedId_example,
    // number | Maximum number of items to return in a single request. <br> **Default:** `25` (optional)
    limit: 56,
    // number | Starting point of the result set. <br>To get page 2 with a limit of 25, set `offset` to `25`. <br> **Default:** `0` (optional)
    offset: 56,
  } satisfies GetFeedsFeedIdRequest;

  try {
    const data = await api.getFeedsFeedId(body);
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
| **feedId** | `string` | Feed ID | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of items to return in a single request. &lt;br&gt; **Default:** &#x60;25&#x60; | [Optional] [Defaults to `25`] |
| **offset** | `number` | Starting point of the result set. &lt;br&gt;To get page 2 with a limit of 25, set &#x60;offset&#x60; to &#x60;25&#x60;. &lt;br&gt; **Default:** &#x60;0&#x60; | [Optional] [Defaults to `0`] |

### Return type

[**PaginationPaginatedResponsePost**](PaginationPaginatedResponsePost.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid feed ID or query parameters |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getFeedsFeedIdCreatorsCreatorId

> PaginationPaginatedResponsePost getFeedsFeedIdCreatorsCreatorId(feedId, creatorId, limit, offset)

List posts by creator

Retrieve posts in a feed by a specific creator, with pagination.

### Example

```ts
import {
  Configuration,
  FeedsApi,
} from '@rixl/sdk-typescript-feeds';
import type { GetFeedsFeedIdCreatorsCreatorIdRequest } from '@rixl/sdk-typescript-feeds';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-feeds SDK...");
  const api = new FeedsApi();

  const body = {
    // string | Feed ID
    feedId: feedId_example,
    // string | Creator ID
    creatorId: creatorId_example,
    // number | Maximum number of items to return in a single request. <br> **Default:** `25` (optional)
    limit: 56,
    // number | Starting point of the result set. <br>To get page 2 with a limit of 25, set `offset` to `25`. <br> **Default:** `0` (optional)
    offset: 56,
  } satisfies GetFeedsFeedIdCreatorsCreatorIdRequest;

  try {
    const data = await api.getFeedsFeedIdCreatorsCreatorId(body);
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
| **feedId** | `string` | Feed ID | [Defaults to `undefined`] |
| **creatorId** | `string` | Creator ID | [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of items to return in a single request. &lt;br&gt; **Default:** &#x60;25&#x60; | [Optional] [Defaults to `25`] |
| **offset** | `number` | Starting point of the result set. &lt;br&gt;To get page 2 with a limit of 25, set &#x60;offset&#x60; to &#x60;25&#x60;. &lt;br&gt; **Default:** &#x60;0&#x60; | [Optional] [Defaults to `0`] |

### Return type

[**PaginationPaginatedResponsePost**](PaginationPaginatedResponsePost.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Invalid feed ID, creator ID, or query parameters |  -  |
| **500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getFeedsFeedIdPostId

> Post getFeedsFeedIdPostId(feedId, postId)

Get a post

Retrieve a post from feed by its ID

### Example

```ts
import {
  Configuration,
  FeedsApi,
} from '@rixl/sdk-typescript-feeds';
import type { GetFeedsFeedIdPostIdRequest } from '@rixl/sdk-typescript-feeds';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript-feeds SDK...");
  const api = new FeedsApi();

  const body = {
    // string | Feed ID
    feedId: feedId_example,
    // string | Post ID
    postId: postId_example,
  } satisfies GetFeedsFeedIdPostIdRequest;

  try {
    const data = await api.getFeedsFeedIdPostId(body);
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
| **feedId** | `string` | Feed ID | [Defaults to `undefined`] |
| **postId** | `string` | Post ID | [Defaults to `undefined`] |

### Return type

[**Post**](Post.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **400** | Bad Request |  -  |
| **404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

