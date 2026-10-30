# BO2-Forever Launcher

Public distribution repository for the BO2-Forever Windows launcher.

## Download / 下載 / ダウンロード

[Download the portable launcher / 下載完整攜帶版 / 完全版をダウンロード](https://github.com/tonyjih/BO2-Forever-Launcher/releases/latest/download/BO2-Forever-Launcher.zip)

Extract the ZIP and run `GBO2-Client/Start-Client.cmd`. Existing users can extract it over their current `GBO2-Client` folder. Invitation codes, language, game paths and cached patches are preserved. Install this auto-update version manually once; subsequent updates are checked at startup.

解壓後執行 `GBO2-Client/Start-Client.cmd`。現有玩家可覆蓋到原本的 `GBO2-Client` 資料夾。邀請碼、語言、遊戲路徑與補丁快取會保留。第一次需要手動安裝支援自動更新的版本；之後每次開啟會檢查更新。

展開後 `GBO2-Client/Start-Client.cmd` を実行してください。既存の `GBO2-Client` フォルダーに上書きできます。招待コード、言語、ゲームパス、キャッシュは保持されます。初回のみ手動でインストールし、次回以降は起動時に更新を確認します。

## Release assets

- `BO2-Forever-Launcher.zip`: full Windows x64 portable launcher including Python 3.12.
- `launcher-update.zip`: small launcher-only update; existing users may extract this over the parent of their current `GBO2-Client` folder.
- `launcher.json`: update version, exact file list, sizes and SHA256 checksums.
- `SHA256SUMS.txt`: checksums for manual downloads.

Only launcher files are distributed here. Game executables, game resources, server data, invitation codes and personal settings are not included. Obtain the Steam game separately and use your existing private-server invitation.

The launcher checks this repository over HTTPS, verifies the release manifest and archive checksums, backs up its current files, and verifies startup before keeping an update. Failed or interrupted installations restore the previous version. When GitHub cannot be reached, the installed version remains available. Personal settings stay in `%LOCALAPPDATA%/GBO2-PrivateClient/client-settings.json`; legacy settings in the launcher folder are also supported.

The server and development repositories remain separate from this distribution repository.
