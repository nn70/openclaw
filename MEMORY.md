# MEMORY.md - 書童的長期記憶

## 2026-03-14

- **關閉 Control UI 的 Device Auth:** 將 `gateway.controlUi.dangerouslyDisableDeviceAuth` 從 `true` 設定為 `false`。
- **更新 Telegram Bot Token:** 將 Telegram Bot Token `8701429158:AAGqVS_Oaqt2ECuCQVavWK8XShs9esOyEMc` 設定到 `channels.telegram.accounts.default.botToken`。
- **Gateway 重啟失敗:** 嘗試重啟 gateway 以應用設定，但重啟失敗並顯示了一些關於 Telegram `groupPolicy` 的警告。具體警告是 `channels.telegram.groupPolicy` 設為 `allowlist` 但 `groupAllowFrom` 為空，這會導致群組訊息被靜默丟棄。
- **模型切換:** 將當前 session 的模型從 `anthropic/claude-sonnet-4-20250514` 切換到 `openrouter/minimax/minimax-m2.5`。預設模型已設定為 `openrouter/minimax/minimax-m2.5`。

## 2026-03-15

- **Homebrew 安裝問題:** 嘗試安裝 Homebrew 但因 `elevated` 權限限制未能直接執行。告知 Tim 需手動執行或調整 OpenClaw 設定。
- **Google Calendar 整合:** 確認 OpenClaw 目前沒有內建 Google Calendar 整合，主要透過 Android 設備配對。
- **Android 配對指引:** 提供 Android 設備配對的 LAN 模式資訊 (`ws://192.168.0.18:18789`)，並詢問 Tim 的網路情況以提供進一步協助。
- **Python 安裝確認:** 確認 Python 3.12.3 已安裝。
- **gog Skill 啟用與 OAuth 設定:**
    - 確認 "gog" skill 已安裝，但 `gog` CLI 工具一開始不在 PATH。
    - 找到 `brew` 位於 `/home/linuxbrew/.linuxbrew/bin/brew`，`gog` CLI 位於 `/home/linuxbrew/.linuxbrew/opt/gogcli/bin/gog`。
    - 指導 Tim 關於 `gog` OAuth 認證設定，包括如何從 Google Cloud Console 下載 `client_secret.json`。
