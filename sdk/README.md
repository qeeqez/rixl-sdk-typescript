# @rixl/sdk-typescript@2.0

A TypeScript SDK client for the localhost API.

## Usage

First, install the SDK from npm.

```bash
npm install @rixl/sdk-typescript --save
```

Next, try it out.


```ts
import {
  Configuration,
  FeedsApi,
} from '@rixl/sdk-typescript';
import type { FeedsFeedIdCreatorsCreatorIdGetRequest } from '@rixl/sdk-typescript';

async function example() {
  console.log("🚀 Testing @rixl/sdk-typescript SDK...");
  const api = new FeedsApi();

  const body = {
    // string | Feed ID
    feedId: F4edRI23XL,
    // string | Creator ID
    creatorId: C6rtRI23XL,
    // number | Maximum number of items to return in a single request. <br> **Default:** `25` (optional)
    limit: 25,
    // number | Starting point of the result set. <br>To get page 2 with a limit of 25, set `offset` to `25`. <br> **Default:** `0` (optional)
    offset: 0,
  } satisfies FeedsFeedIdCreatorsCreatorIdGetRequest;

  try {
    const data = await api.feedsFeedIdCreatorsCreatorIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```


## Documentation

### API Endpoints

All URIs are relative to *http://localhost*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*FeedsApi* | [**feedsFeedIdCreatorsCreatorIdGet**](docs/FeedsApi.md#feedsfeedidcreatorscreatoridget) | **GET** /feeds/{feedId}/creators/{creatorId} | List posts by creator
*FeedsApi* | [**feedsFeedIdGet**](docs/FeedsApi.md#feedsfeedidget) | **GET** /feeds/{feedId} | List posts in a feed
*FeedsApi* | [**feedsFeedIdPostIdGet**](docs/FeedsApi.md#feedsfeedidpostidget) | **GET** /feeds/{feedId}/{postId} | Get a post
*ImagesApi* | [**imagesGet**](docs/ImagesApi.md#imagesget) | **GET** /images | List images for a project
*ImagesApi* | [**imagesImageIdDelete**](docs/ImagesApi.md#imagesimageiddelete) | **DELETE** /images/{imageId} | Delete image
*ImagesApi* | [**imagesImageIdGet**](docs/ImagesApi.md#imagesimageidget) | **GET** /images/{imageId} | Get image
*ImagesApi* | [**imagesUploadCompletePost**](docs/ImagesApi.md#imagesuploadcompletepostoperation) | **POST** /images/upload/complete | Upload: Mark as complete
*ImagesApi* | [**imagesUploadInitPost**](docs/ImagesApi.md#imagesuploadinitpostoperation) | **POST** /images/upload/init | Upload: Init
*VideosApi* | [**videosGet**](docs/VideosApi.md#videosget) | **GET** /videos | List videos for a project
*VideosApi* | [**videosLanguagesGet**](docs/VideosApi.md#videoslanguagesget) | **GET** /videos/languages | List available subtitle languages
*VideosApi* | [**videosUploadCompletePost**](docs/VideosApi.md#videosuploadcompletepostoperation) | **POST** /videos/upload/complete | Upload: Mark as complete
*VideosApi* | [**videosUploadInitPost**](docs/VideosApi.md#videosuploadinitpostoperation) | **POST** /videos/upload/init | Upload: Init
*VideosApi* | [**videosVideoIdAudioTracksDelete**](docs/VideosApi.md#videosvideoidaudiotracksdelete) | **DELETE** /videos/{videoId}/audio-tracks | Delete all audio tracks
*VideosApi* | [**videosVideoIdAudioTracksLangCodeDelete**](docs/VideosApi.md#videosvideoidaudiotrackslangcodedelete) | **DELETE** /videos/{videoId}/audio-tracks/{lang_code} | Delete audio track by language
*VideosApi* | [**videosVideoIdAudioTracksLangCodePut**](docs/VideosApi.md#videosvideoidaudiotrackslangcodeput) | **PUT** /videos/{videoId}/audio-tracks/{lang_code} | Upsert video audio track
*VideosApi* | [**videosVideoIdAudioTracksPost**](docs/VideosApi.md#videosvideoidaudiotrackspost) | **POST** /videos/{videoId}/audio-tracks | Bulk upsert video audio tracks
*VideosApi* | [**videosVideoIdAudioTracksTrackIdDelete**](docs/VideosApi.md#videosvideoidaudiotrackstrackiddelete) | **DELETE** /videos/{videoId}/audio-tracks/{trackId} | Delete audio track
*VideosApi* | [**videosVideoIdChaptersDelete**](docs/VideosApi.md#videosvideoidchaptersdelete) | **DELETE** /videos/{videoId}/chapters | Delete video chapters
*VideosApi* | [**videosVideoIdChaptersPut**](docs/VideosApi.md#videosvideoidchaptersputoperation) | **PUT** /videos/{videoId}/chapters | Update video chapters
*VideosApi* | [**videosVideoIdDeleteDelete**](docs/VideosApi.md#videosvideoiddeletedelete) | **DELETE** /videos/{videoId}/delete | Delete video
*VideosApi* | [**videosVideoIdGet**](docs/VideosApi.md#videosvideoidget) | **GET** /videos/{videoId} | Get a video
*VideosApi* | [**videosVideoIdSubtitlesDelete**](docs/VideosApi.md#videosvideoidsubtitlesdelete) | **DELETE** /videos/{videoId}/subtitles | Delete all subtitles
*VideosApi* | [**videosVideoIdSubtitlesLangCodeDelete**](docs/VideosApi.md#videosvideoidsubtitleslangcodedelete) | **DELETE** /videos/{videoId}/subtitles/{lang_code} | Delete subtitle by language
*VideosApi* | [**videosVideoIdSubtitlesLangCodePut**](docs/VideosApi.md#videosvideoidsubtitleslangcodeput) | **PUT** /videos/{videoId}/subtitles/{lang_code} | Upsert video subtitle
*VideosApi* | [**videosVideoIdSubtitlesPost**](docs/VideosApi.md#videosvideoidsubtitlespost) | **POST** /videos/{videoId}/subtitles | Bulk upsert video subtitles
*VideosApi* | [**videosVideoIdSubtitlesSubtitleIdDelete**](docs/VideosApi.md#videosvideoidsubtitlessubtitleiddelete) | **DELETE** /videos/{videoId}/subtitles/{subtitleId} | Delete subtitle
*VideosApi* | [**videosVideoIdThumbnailPut**](docs/VideosApi.md#videosvideoidthumbnailput) | **PUT** /videos/{videoId}/thumbnail | Update video thumbnail


### Models

- [AudioTrack](docs/AudioTrack.md)
- [AudioTrackDelete](docs/AudioTrackDelete.md)
- [Chapter](docs/Chapter.md)
- [FileStatus](docs/FileStatus.md)
- [GithubComQeeqezApiDbSqlcPlanType](docs/GithubComQeeqezApiDbSqlcPlanType.md)
- [GithubComQeeqezApiDbSqlcVideoQuality](docs/GithubComQeeqezApiDbSqlcVideoQuality.md)
- [GithubComQeeqezApiInternalErrorsErrorResponse](docs/GithubComQeeqezApiInternalErrorsErrorResponse.md)
- [GithubComQeeqezApiInternalVideosHandlerUploadCompleteRequest](docs/GithubComQeeqezApiInternalVideosHandlerUploadCompleteRequest.md)
- [GithubComQeeqezApiInternalVideosHandlerUploadInitResponse](docs/GithubComQeeqezApiInternalVideosHandlerUploadInitResponse.md)
- [GithubComQeeqezApiInternalVideosTypesChapterInput](docs/GithubComQeeqezApiInternalVideosTypesChapterInput.md)
- [GithubComQeeqezApiInternalVideosVideoResponse](docs/GithubComQeeqezApiInternalVideosVideoResponse.md)
- [Image](docs/Image.md)
- [ImagesUploadCompletePostRequest](docs/ImagesUploadCompletePostRequest.md)
- [ImagesUploadInitPostRequest](docs/ImagesUploadInitPostRequest.md)
- [InternalImagesHandlerCompleteRequest](docs/InternalImagesHandlerCompleteRequest.md)
- [InternalImagesHandlerInitResponse](docs/InternalImagesHandlerInitResponse.md)
- [InternalImagesHandlerUploadInitRequest](docs/InternalImagesHandlerUploadInitRequest.md)
- [InternalVideosHandlerSubtitlesLanguageResponse](docs/InternalVideosHandlerSubtitlesLanguageResponse.md)
- [ModelFile](docs/ModelFile.md)
- [PaginationPaginatedResponseImage](docs/PaginationPaginatedResponseImage.md)
- [PaginationPaginatedResponsePost](docs/PaginationPaginatedResponsePost.md)
- [PaginationPaginatedResponseVideo](docs/PaginationPaginatedResponseVideo.md)
- [PaginationPagination](docs/PaginationPagination.md)
- [Post](docs/Post.md)
- [PostType](docs/PostType.md)
- [Subtitle](docs/Subtitle.md)
- [SubtitleDelete](docs/SubtitleDelete.md)
- [UpdateChaptersRequest](docs/UpdateChaptersRequest.md)
- [UpdateChaptersResponse](docs/UpdateChaptersResponse.md)
- [Video](docs/Video.md)
- [VideoUploadInitRequest](docs/VideoUploadInitRequest.md)
- [VideosUploadCompletePostRequest](docs/VideosUploadCompletePostRequest.md)
- [VideosUploadInitPostRequest](docs/VideosUploadInitPostRequest.md)
- [VideosVideoIdChaptersPutRequest](docs/VideosVideoIdChaptersPutRequest.md)

### Authorization


Authentication schemes defined for the API:
<a id="ApiKeyAuth"></a>
#### ApiKeyAuth


- **Type**: API key
- **API key parameter name**: `X-API-Key`
- **Location**: HTTP header
<a id="Bearer"></a>
#### Bearer


- **Type**: API key
- **API key parameter name**: `Authorization`
- **Location**: HTTP header

## About

This TypeScript SDK client supports the [Fetch API](https://fetch.spec.whatwg.org/)
and is automatically generated by the
[OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `2.0`
- Package version: `2.0`
- Generator version: `7.20.0`
- Build package: `org.openapitools.codegen.languages.TypeScriptFetchClientCodegen`

The generated npm module supports the following:

- Environments
  * Node.js
  * Webpack
  * Browserify
- Language levels
  * ES5 - you must have a Promises/A+ library installed
  * ES6
- Module systems
  * CommonJS
  * ES6 module system

For more information, please visit [https://rixl.com/support](https://rixl.com/support)

## Development

### Building

To build the TypeScript source code, you need to have Node.js and npm installed.
After cloning the repository, navigate to the project directory and run:

```bash
npm install
npm run build
```

### Publishing

Once you've built the package, you can publish it to npm:

```bash
npm publish
```

## License

[All Rights Reserved](https://rixl.com/terms-of-service)
