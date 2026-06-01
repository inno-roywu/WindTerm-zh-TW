# WindTerm 繁體中文（台灣習慣用語）優化語系檔

本專案是針對開源終端機工具 [kingToolbox/WindTerm](https://github.com/kingToolbox/WindTerm)（最新 Release v2.7.0）所優化編譯的繁體中文（台灣地區習慣用語）語系檔。

> [!NOTE]
> **聲明：** 本專案為獨立語系優化專案，並非官方 Fork 的程式碼庫，主要提供 WindTerm 繁體中文介面本土化的修正。

---

## 💡 為什麼需要本專案？（我們做了哪些改動）

WindTerm 官方最新 Release 雖內建了正體中文選項，但其翻譯內容存在大量直接簡轉繁或滑稽的機器直譯，極度影響使用體驗。

本專案針對官方 `zh-CN.locale`（包含 1,414 個翻譯項目）進行了全量中文化本土校正，主要改動包括：
* ⌨️ **修正嚴重直譯笑話**：
  * 修正 `Waiting for more keys`：舊版直譯為「等待更多**鑰匙** 🔑」 ➡️ 修正為「等待更多**按鍵** ⌨️」。
  * 修正 `Attempt pageant authentication`：舊版直譯為「嘗試**選美**認證 👸」 ➡️ 修正為「嘗試 **Pageant** 驗證 🔒」（Pageant 為 PuTTY 的密鑰代理程式）。
  * 修正 `Blink` / `blinking line`：舊版直譯為「**眨眼** 👀」 ➡️ 修正為「**閃爍** / 閃爍垂直線 ✨」。
  * 修正 `Block` / `block`：舊版直譯為「**堵塞** 🚫」 ➡️ 修正為「**方塊** ⏹️」游標。
  * 修正 `Bold`：舊版直譯為「**膽大** 💪」 ➡️ 修正為「**粗體** 🅰️」字型。
  * 修正 `Bars`：舊版直譯為「**酒吧** 🍺」 ➡️ 修正為「**欄/列** 📊」介面元素。
* 🇹🇼 **台灣地區習慣用語校正**：
  * 「文件」 ➡️ 「檔案」（對應 File）。
  * 「文件夾」 ➡️ 「資料夾」（對應 Folder）。
  * 「會話」 ➡️ 「工作階段」 / 「連線」（對應 Session）。
  * 「網絡」 ➡️ 「網路」。
  * 「本地」 / 「遠程」 ➡️ 「本機」 / 「遠端」。
  * 「配置」 ➡️ 「設定」（對應 Configure/Settings）。
  * 「保存」 ➡️ 「儲存」（對應 Save）。
  * 「窗口」 ➡️ 「視窗」。
  * 「鼠標」 ➡️ 「滑鼠」。
  * 「快捷鍵」 ➡️ 「快速鍵」。
  * 「菜單」 ➡️ 「選單」。
  * 「工具欄」 / 「狀態欄」 ➡️ 「工具列」 / 「狀態列」。
  * 「標籤頁」 / 「標籤」 ➡️ 「分頁」（對應 Tab）。
  * 「重新加載」 / 「撤消」 ➡️ 「重新載入」 / 「復原」。
  * 「運行」 / 「調試」 ➡️ 「執行」 / 「偵錯」。
  * 「波特率」 / 「數據位」 ➡️ 「鮑率」 / 「資料位元」。
  * 「數據包」 ➡️ 「封包」。

---

## 🚀 搭配官方 Release 軟體套用教學

如果您已經從 [WindTerm 官方 Release 頁面](https://github.com/kingToolbox/WindTerm/releases) 下載並安裝了官方版本，而**只想替換為本專案的繁體中文翻譯**，請按照以下步驟使用：

### 📥 步驟 1：下載語系檔
* 您可以直接點擊 [zh-TW.locale](https://raw.githubusercontent.com/inno-roywu/WindTerm-zh-TW/main/zh-TW.locale)（滑鼠右鍵點擊連結並選擇「另存連結為...」）。
* 或者，前往本儲存庫的 [Releases 頁面](https://github.com/inno-roywu/WindTerm-zh-TW/releases) 下載最新發佈的 `zh-TW.locale` 檔案。

### 📂 步驟 2：覆蓋官方語系檔
將下載的 `zh-TW.locale` 檔案放入您 WindTerm 安裝目錄下的 `global/locales` 資料夾中（直接覆蓋原本不正確的繁體中文語系檔）。
* 預設路徑通常為：`WindTerm_2.7.0/global/locales/zh-TW.locale`

### ⚙️ 步驟 3：於 GUI 介面套用
1. 啟動（或重新啟動）WindTerm。
2. 點擊頂部選單的 **`Settings` (設定)** -> **`Language` (語言)**。
3. 選擇 **`Chinese (Traditional) - 正體中文 (繁體)`**。
4. 介面將會立刻載入由本專案優化台灣化的繁體中文！

---

## 📄 授權與貢獻
* 本語系檔基於 WindTerm 的官方語系結構重新編譯。
* 歡迎提交 Issue 或是 Pull Request 一同改善翻譯品質！
