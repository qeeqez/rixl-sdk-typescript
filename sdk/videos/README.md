# @rixl/sdk-typescript-videos@2.0.0

A TypeScript SDK client for the api.rixl.com API.

## Usage

First, install the SDK from npm.

```bash
npm install @rixl/sdk-typescript-videos --save
```

Next, try it out.


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


## Documentation

### API Endpoints

All URIs are relative to *https://api.rixl.com*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*VideosApi* | [**deleteVideosVideoIdAudioTracks**](docs/VideosApi.md#deletevideosvideoidaudiotracks) | **DELETE** /videos/{videoId}/audio-tracks | Delete all audio tracks
*VideosApi* | [**deleteVideosVideoIdAudioTracksLangCode**](docs/VideosApi.md#deletevideosvideoidaudiotrackslangcode) | **DELETE** /videos/{videoId}/audio-tracks/{lang_code} | Delete audio track by language
*VideosApi* | [**deleteVideosVideoIdAudioTracksTrackId**](docs/VideosApi.md#deletevideosvideoidaudiotrackstrackid) | **DELETE** /videos/{videoId}/audio-tracks/{trackId} | Delete audio track
*VideosApi* | [**deleteVideosVideoIdChapters**](docs/VideosApi.md#deletevideosvideoidchapters) | **DELETE** /videos/{videoId}/chapters | Delete video chapters
*VideosApi* | [**deleteVideosVideoIdDelete**](docs/VideosApi.md#deletevideosvideoiddelete) | **DELETE** /videos/{videoId}/delete | Delete video
*VideosApi* | [**deleteVideosVideoIdSubtitles**](docs/VideosApi.md#deletevideosvideoidsubtitles) | **DELETE** /videos/{videoId}/subtitles | Delete all subtitles
*VideosApi* | [**deleteVideosVideoIdSubtitlesLangCode**](docs/VideosApi.md#deletevideosvideoidsubtitleslangcode) | **DELETE** /videos/{videoId}/subtitles/{lang_code} | Delete subtitle by language
*VideosApi* | [**deleteVideosVideoIdSubtitlesSubtitleId**](docs/VideosApi.md#deletevideosvideoidsubtitlessubtitleid) | **DELETE** /videos/{videoId}/subtitles/{subtitleId} | Delete subtitle
*VideosApi* | [**getVideos**](docs/VideosApi.md#getvideos) | **GET** /videos | List videos for a project
*VideosApi* | [**getVideosLanguages**](docs/VideosApi.md#getvideoslanguages) | **GET** /videos/languages | List available subtitle languages
*VideosApi* | [**getVideosVideoId**](docs/VideosApi.md#getvideosvideoid) | **GET** /videos/{videoId} | Get a video
*VideosApi* | [**postVideosUploadComplete**](docs/VideosApi.md#postvideosuploadcomplete) | **POST** /videos/upload/complete | Upload: Mark as complete
*VideosApi* | [**postVideosUploadInit**](docs/VideosApi.md#postvideosuploadinit) | **POST** /videos/upload/init | Upload: Init
*VideosApi* | [**postVideosVideoIdAudioTracks**](docs/VideosApi.md#postvideosvideoidaudiotracks) | **POST** /videos/{videoId}/audio-tracks | Bulk upsert video audio tracks
*VideosApi* | [**postVideosVideoIdSubtitles**](docs/VideosApi.md#postvideosvideoidsubtitles) | **POST** /videos/{videoId}/subtitles | Bulk upsert video subtitles
*VideosApi* | [**putVideosVideoIdAudioTracksLangCode**](docs/VideosApi.md#putvideosvideoidaudiotrackslangcode) | **PUT** /videos/{videoId}/audio-tracks/{lang_code} | Upsert video audio track
*VideosApi* | [**putVideosVideoIdChapters**](docs/VideosApi.md#putvideosvideoidchapters) | **PUT** /videos/{videoId}/chapters | Update video chapters
*VideosApi* | [**putVideosVideoIdSubtitlesLangCode**](docs/VideosApi.md#putvideosvideoidsubtitleslangcode) | **PUT** /videos/{videoId}/subtitles/{lang_code} | Upsert video subtitle
*VideosApi* | [**putVideosVideoIdThumbnail**](docs/VideosApi.md#putvideosvideoidthumbnail) | **PUT** /videos/{videoId}/thumbnail | Update video thumbnail


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
- [Image](docs/Image.md)
- [InternalVideosHandlerSubtitlesLanguageResponse](docs/InternalVideosHandlerSubtitlesLanguageResponse.md)
- [ModelFile](docs/ModelFile.md)
- [PaginationPaginatedResponseVideo](docs/PaginationPaginatedResponseVideo.md)
- [PaginationPagination](docs/PaginationPagination.md)
- [Subtitle](docs/Subtitle.md)
- [SubtitleDelete](docs/SubtitleDelete.md)
- [UpdateChaptersRequest](docs/UpdateChaptersRequest.md)
- [UpdateChaptersResponse](docs/UpdateChaptersResponse.md)
- [Video](docs/Video.md)
- [VideoUploadInitRequest](docs/VideoUploadInitRequest.md)

### Authorization


Authentication schemes defined for the API:
<a id="ApiKeyAuth"></a>
#### ApiKeyAuth


- **Type**: API key
- **API key parameter name**: `X-API-Key`
- **Location**: HTTP header

## About

This TypeScript SDK client supports the [Fetch API](https://fetch.spec.whatwg.org/)
and is automatically generated by the
[OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `2.0`
- Package version: `2.0.0`
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
