# PROJECT.md

## 架構定位（2026-07-23）

| 角色 | 正式位置 |
|---|---|
| Execution 本機 NTFS | `C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行` |
| Version Git root | `C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行` |
| Version GitHub | `https://github.com/scotthcliu-jpg/2607-nanjing-youyou-trip.git` |
| 預設 branch | `main` |
| 獨立 repo | `yes` |
| Knowledge／legacy source | `G:\我的雲端硬碟\2026Claude\100_Todo\projects\active\2607南京用友出行`（唯讀，不作為 Agent workspace） |
| 架構 release | `agent-sync-v1.2.3` |

## 專案概覽

- 專案名稱：2607南京用友出行
- 工作區路徑：`C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行`
- 建立/補建時間：2026-07-21 16:14
- GitHub：獨立 repo `scotthcliu-jpg/2607-nanjing-youyou-trip`（見上方架構定位）
- Obsidian：`G:\我的雲端硬碟\第二大腦\Projects\2607南京用友出行.md`

## 目標

整理南京用友出行相關行程、工作安排與待辦，讓後續可由不同 AI 接續處理。

## 目前已知資料

- 目前資料夾內已存在：
  - `AGENTS.md`
  - `CLAUDE.md`
  - `2026-07-08_南京行程.html`（8/2–8/8 行程規劃主頁，部署為 Netlify `index.html`）
  - `2026-07-08_南京行程地圖.html`（行程地圖版，部署為 Netlify `map.html`）
- 尚未看到票務、會議紀錄、報告等其他資料。
- 已確認 GitHub：獨立 repo `scotthcliu-jpg/2607-nanjing-youyou-trip`。

## GitHub Pages 部署

- Production URL：`https://scotthcliu-jpg.github.io/2607-nanjing-youyou-trip/`
- 發布來源：GitHub repository `main` branch 的根目錄。
- `index.html` 轉址至 `2026-07-08_南京行程.html`；`map.html` 轉址至 `2026-07-08_南京行程地圖.html`，保留原始中文檔名。
- 此站以公開 GitHub Pages 發布；行程內容可由任何持有網址者存取。
- 不再使用 Netlify 部署。

## 目前狀態

- 2026-07-24：8/2–8/8 南京行程 HTML（含地圖版）已從 Google Drive legacy 來源複製進本機工作區、加入 Git，並部署上線至 Netlify。
- 2026-07-24：標題列加上「最新修改日期」紅字標籤（桌面版釘右、手機版置中），與頁尾更新日期同步。
- 2026-08-01：Day 7（8/8）「阿里雲谷參訪・返程」交通已由用友 Tina 確認：G7609 南京南 08:51 → 杭州東 10:19；G7644 杭州西 15:32 → 上海虹橋 16:55。兩段車票與接駁車皆由 Tina 協助，費用回台後結算；上海虹橋抵達後銜接 19:40 長榮班機飛松山。
- 2026-07-24：新增「📋 追蹤待辦」區塊——已知參訪台商：太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科；待辦：8/7–8/8 與台商交流、評估用友ERP使用情形。
- 出行人員、工作目的（用友商業創新大會，8/7）與其餘每日行程細節已在 HTML 內，尚待逐一核對是否為最新版本。
- 2026-07-31：正式網站改為 GitHub Pages；`main` branch 根目錄成功建置，GitHub Pages Production URL 已可公開存取。
- 2026-08-01：確認公開行程頁目前包含 Day 1–6；使用者將進行內容核對。
- 2026-08-01：已安裝並實測專案提交閘門；任何行程或內容變更若未同時納入 `PROJECT.md` 與 `HANDOFF.md`，pre-commit 將拒絕提交，以避免跨 Agent 狀態漂移。

## 待確認

- 8/7–8/8 與台商（太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科）交流用友ERP評估的具體安排與結論待後續補充。
- 其餘 Day 1–6 行程內容是否為最新版本（是否有異動未反映在此 HTML）。
- 是否需要把票務、住宿、交通、會議資料另存進專案。
