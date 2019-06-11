[android-components](../../index.md) / [mozilla.components.feature.downloads.manager](../index.md) / [AndroidDownloadManager](index.md) / [download](./download.md)

# download

`fun download(download: `[`Download`](../../mozilla.components.browser.session/-download/index.md)`, refererUrl: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, cookie: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/feature/downloads/src/main/java/mozilla/components/feature/downloads/manager/AndroidDownloadManager.kt#L56)

Overrides [DownloadManager.download](../-download-manager/download.md)

Schedule a download through the [AndroidDownloadManager](index.md).

### Parameters

`download` - metadata related to the download.

`refererUrl` - the url from where this download was referred.

`cookie` - any additional cookie to add as part of the download request.

**Return**
the id reference of the scheduled download.
