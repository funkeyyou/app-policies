# AI翻譯助手 隱私權政策／Privacy Policy

生效日期／Effective date：2026-10-12


## 繁體中文

AI翻譯助手（以下稱「本擴充功能」）用來在 Chrome 中翻譯網頁、選取的文字、影片字幕與文件。本擴充功能的開發者**沒有架設任何伺服器，不會收集、接收、儲存或查看你的任何資料**。以下說明本擴充功能在你的電腦上處理哪些資料，以及會把哪些資料傳送到哪裡。

### 1. 為了翻譯而傳送的內容

- 當你翻譯網頁、翻譯選取的文字、翻譯文件，或開啟自動翻譯（指定網站、YouTube／Google Drive 影片字幕）時，本擴充功能會把需要翻譯的**文字**傳送到你選擇的翻譯服務。這些文字包括網頁內容、選取的文字、字幕文字、從文件擷取出的文字，以及用來統一譯名的段落摘要。
- 翻譯服務有兩種，由你選擇：
  - **你自行設定的 AI 服務**：任何 OpenAI 相容 API，例如 OpenAI、OpenRouter、Google Gemini、DeepSeek，或你自己架設的伺服器。傳送目的地就是你在「AI 服務」填寫的 Base URL。
  - **Google 翻譯**（translate.googleapis.com）：只有在你選用 Google 翻譯的方案或字幕引擎時才會使用。
- 這些服務會依照各自的隱私權政策處理收到的文字，本擴充功能無法控制。請不要翻譯你不希望交給該服務的內容。
- 文件（PDF、EPUB、Word 等）在你的電腦上解析，檔案本身不會上傳，只有擷取出來的文字會送去翻譯。
- 開啟「簡繁自動互轉」時，簡體與繁體中文之間的轉換在你的電腦上完成，不會傳送出去。
- YouTube／Google Drive 字幕自動翻譯預設關閉，你可以在設定頁「影片字幕」或影片頁的工具列面板開啟。

### 2. API Key

你在「AI 服務」填寫的 API Key 只存在這台電腦的瀏覽器（chrome.storage.local）。它不會透過 Chrome 同步到其他裝置，也不會包含在匯出的設定檔中；只有在呼叫你設定的 AI 服務時，才會放在請求標頭中傳送給該服務。

### 3. 存在你電腦上的資料

- **設定**（翻譯方案、顯示方式、自動翻譯的網站清單、翻譯指令等）存在 chrome.storage.sync。如果你開啟了 Chrome 同步，Google 會依其政策在你的裝置之間同步這些設定（不含 API Key）。
- **術語表、禁用詞清單、翻譯快取（原文與譯文）、模型清單**存在本機。
- **用量統計**：翻譯過的頁面網址與標題、使用的模型、token 數與估算費用，存在本機（IndexedDB），只用來顯示在「用量統計」頁。
- **除錯紀錄**：可能包含網址與文字片段，存在本機，只用來顯示在「除錯紀錄」頁。
- **右鍵翻譯時選取的文字**：暫存在瀏覽器工作階段（chrome.storage.session），關閉瀏覽器即清除。

這些資料都不會傳給開發者。你可以在工具列面板清除翻譯快取與累計用量、在設定頁清除用量統計與除錯紀錄，或直接移除擴充功能以刪除全部資料。

### 4. 其他連線

- **匯率**（open.er-api.com）：每天取得一次美元兌新台幣匯率，用來顯示估算費用，不含任何個人資料。
- **PDF 字型**（jimmysu0309.github.io，字型檔託管網站）：只有在把 PDF 譯成簡體中文、日文或韓文時，才會下載對應的 Noto 字型，並以 SHA-256 驗證檔案，不含任何個人資料。
- 翻譯請求與上述連線都使用 HTTPS。唯一的例外是你在 Base URL 自行填寫以 http:// 開頭的網址（例如本機的 Ollama、LM Studio）；這種連線不加密，建議只用於本機或自己的區域網路。

### 5. 我們不做的事

本擴充功能不使用任何分析或追蹤工具，不放廣告，不出售或轉讓使用者資料，不把資料用於與翻譯無關的用途，也不用於信用評估或借貸。

本擴充功能對使用者資料的使用遵守 Chrome 線上應用程式商店使用者資料政策（Chrome Web Store User Data Policy），包括其中的「有限使用」（Limited Use）規定。

### 6. 聯絡方式

對本政策有任何問題，請寫信到：funkeyyou@gmail.com

### 7. 政策變更

本政策如有變更，會更新本頁內容並修改上方的生效日期。

---

## English

AI Translation Assistant ("the extension") translates web pages, selected text, video subtitles and documents in Chrome. The developer of the extension **does not operate any server and does not collect, receive, store or view any of your data**. This policy explains what the extension handles on your computer and where data is sent.

### 1. Content sent for translation

- When you translate a page, selected text or a document, or turn on auto-translation (for specific sites or for YouTube / Google Drive subtitles), the extension sends the **text to be translated** to the translation service you choose. This includes page content, selected text, subtitle text, text extracted from documents, and short excerpts used to keep terminology consistent.
- You choose between two kinds of translation service:
  - **The AI service you configure**: any OpenAI-compatible API, such as OpenAI, OpenRouter, Google Gemini, DeepSeek or your own self-hosted server. Text is sent to the Base URL you enter under "AI service".
  - **Google Translate** (translate.googleapis.com): used only when you choose a Google Translate profile or subtitle engine.
- These services process the text under their own privacy policies, which the extension does not control. Do not translate content you do not want to share with the service you chose.
- Documents (PDF, EPUB, Word, etc.) are parsed on your computer. The files themselves are never uploaded; only the extracted text is sent for translation.
- With "Auto-convert Chinese variants" turned on, conversion between Simplified and Traditional Chinese happens on your computer and nothing is sent.
- YouTube / Google Drive subtitle auto-translation is off by default. You can enable it under Settings → Video subtitles or from the toolbar panel on a video page.

### 2. API key

The API key you enter under "AI service" is stored only in this browser on this computer (chrome.storage.local). It is not synced to other devices through Chrome Sync and is not included in exported settings. It is sent only to the AI service you configured, in the request header of each call to that service.

### 3. Data stored on your computer

- **Settings** (translation profiles, display options, the list of sites to auto-translate, translation prompts, etc.) are stored in chrome.storage.sync. If Chrome Sync is on, Google syncs these settings between your devices under its own policy (the API key is not included).
- **Glossaries, forbidden-term lists, the translation cache (original and translated text) and the model list** are stored locally.
- **Usage statistics**: the URL and title of translated pages, the model used, token counts and estimated cost are stored locally (IndexedDB) and are only shown on the "Usage" page.
- **Debug logs** may contain URLs and text snippets. They are stored locally and only shown on the "Debug log" page.
- **Right-click selections** are kept temporarily in browser session storage (chrome.storage.session) and are cleared when the browser closes.

None of this data is sent to the developer. You can clear the translation cache and totals from the toolbar popup, clear usage statistics and debug logs in Settings, or remove the extension to delete all of its data.

### 4. Other connections

- **Exchange rate** (open.er-api.com): the USD → TWD rate is fetched once a day to show cost estimates. No personal data is included.
- **PDF fonts** (jimmysu0309.github.io, where the font files are hosted): Noto fonts are downloaded, and verified with SHA-256, only when you translate a PDF into Simplified Chinese, Japanese or Korean. No personal data is included.
- Translation requests and the connections above use HTTPS. The only exception is a Base URL you enter yourself that starts with http:// (for example a local Ollama or LM Studio server). Such connections are not encrypted, so use http:// only for servers on your own computer or local network.

### 5. What we do not do

The extension uses no analytics or tracking, shows no ads, does not sell or transfer user data, does not use data for purposes unrelated to translation, and does not use data for creditworthiness or lending.

The use of information received by the extension adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements.

### 6. Contact

Questions about this policy: funkeyyou@gmail.com

### 7. Changes

If this policy changes, this page will be updated together with the effective date above.
