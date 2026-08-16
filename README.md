# 即時譯幕 Releases

這個 repository 只保存「即時譯幕」對外發佈的版本紀錄與 Apple 公證安裝檔，不包含產品原始碼。

- [產品官網](https://subtitles.ranger-huang.com)
- [下載最新版](https://ranger-instantly-translate-subtitles.web.app/download/latest)
- [隱私權說明](https://subtitles.ranger-huang.com/privacy)
- [使用條款](https://subtitles.ranger-huang.com/terms)

## 安裝檔驗證

每個 GitHub Release 都附上同一版本的 DMG。安裝檔使用 Developer ID 簽章、送交 Apple 公證，並附有可離線驗證的公證票據。

下載後可在「終端機」執行：

```bash
spctl -a -vvv -t install InstantSubtitles-2.0.0.dmg
shasum -a 256 InstantSubtitles-2.0.0.dmg
```

各版本的檔案大小、SHA-256、build number 與實際建置 commit 記錄於 [`releases/`](releases/)；改版資訊記錄於 [`release-notes/`](release-notes/)。

> 這個公開 repository 的 tag 指向對應的發佈 metadata commit。產品原始碼 repository 維持私有，因此真正用來建置 App 的 commit 另以 `sourceBuildCommit` 記錄在 provenance manifest 中。

## 授權與問題回報

即時譯幕並非開源軟體，著作權由開發者保留，安裝與使用須遵守[使用條款](https://subtitles.ranger-huang.com/terms)。如需回報問題，請使用 App 內的「回報問題」功能或來信 `ranger1214v@gmail.com`。
