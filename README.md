# AI 台灣旅遊情報員 × 智慧行程推薦網站

以每週台灣旅遊情報吸引親子、情侶與熟齡旅客，依出遊條件提供可解釋的行程建議。網站使用示範品牌「島旅相談所」。

## 開啟網站

用瀏覽器開啟 [index.html](index.html)。本機可離線進行推薦，週報與官方來源連結需要連網。選擇旅客類型、每人整趟的新台幣預算、天數與旅遊風格，再按「匹配行程」。勾選「雨天旅遊」可優先比較有室內參觀安排的方案，結果可複製成諮詢摘要。

網站只用 HTML、CSS 與原生 JavaScript。景點和活動沿用已查核資料，示範行程與價格均有標示。公開模式會隱藏模擬方案。正式方案、估價及聯絡窗口由旅行社提供，網站不儲存或傳送旅客表單內容。

## 專案檔案

| 內容 | 位置 |
| --- | --- |
| 六個工作角色、查證及交接規則 | [AGENTS.md](AGENTS.md) |
| 網站規劃與需求 | [CCI](docs/CCI.md)、[SIPOC](docs/SIPOC.md)、[PRD](docs/PRD.md)、[網站交接](website/README.md) |
| 研究資料與來源 | [travel-data.json](research/travel-data.json)、[sources.md](research/sources.md) |
| 2026-W48 週報 | [週報](docs/weekly-report.md)、[圖文新版](docs/weekly-report-2026-w48-illustrated-v2.md) |
| 簡報 | [8 張 HTML](slides.html)、[8 張 PowerPoint](slides.pptx)、[8 張大綱](docs/slides-outline.md)、[10 張圖文 HTML](weekly-report-10-slides.html)、[10 張大綱](docs/weekly-report-10-slides-outline.md) |
| 30 秒宣傳影片與企劃 | [MP4](video/taiwan-travel-30s.mp4)、[分鏡](video/storyboard.md)、[影片提示詞](video/prompts.md) |
| 各階段範本 | [研究](research/template.md)、[週報](newsletter/template.md)、[簡報](presentation/template.md)、[影片](video/template.md)、[驗收](qa/template.md) |

週報與簡報的 AI 生成照片存於 `docs/images/`，圖文中已標明合成示意。

## 更新與驗收

1. 查核景點、活動、來源及查詢日，記錄「待確認」欄位。
2. 用同一 ISO 週次串接研究、週報、簡報與影片企劃。
3. 網站更新資料時核對內嵌資料和研究 JSON，確認每筆推薦可回溯來源。
4. 驗收三類旅客、預算邊界、活動日期、雨天優先、無結果與複製摘要。以 320、768、1280 px 核對版型。
5. 依 [AGENTS.md](AGENTS.md) 覆核對外發布內容。先確認遠端儲存庫和提交清單，帳密、API Key、環境檔與真實客戶資料留在版本控制之外。

下載用的 `weekly-report-10-slides.zip` 和本機匯出檔由 `.gitignore` 排除。
