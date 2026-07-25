# PROJECT.md

## 架構定位（2026-07-23）

| 角色 | 正式位置 |
|---|---|
| Execution 本機 NTFS | `C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行` |
| Version Git root | `C:\Users\user\Documents\Codex\2026Claude` |
| Version GitHub | `https://github.com/scotthcliu-jpg/my-agent-2026.git` |
| 預設 branch | `main` |
| 獨立 repo | `no` |
| Knowledge／legacy source | `G:\我的雲端硬碟\2026Claude\100_Todo\projects\active\2607南京用友出行`（唯讀，不作為 Agent workspace） |
| 架構 release | `agent-sync-v1.1.0` |

## 專案概覽

- 專案名稱：2607南京用友出行
- 工作區路徑：`C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行`
- 建立/補建時間：2026-07-21 16:14
- GitHub：monorepo `scotthcliu-jpg/my-agent-2026`（見上方架構定位）
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
- 已確認 GitHub：monorepo `scotthcliu-jpg/my-agent-2026`（非獨立 repo）。

## Netlify 部署

- Production URL：`https://scott-nanjing-trip-202608.netlify.app/`
- Site ID：`8f7231c2-e5c7-4d62-88df-2926d3529026`（帳號 Scott.hcliu Liu，team TzuChi）
- 部署方式：`netlify deploy --prod --dir=<暫存目錄含 index.html/map.html> --site=8f7231c2-e5c7-4d62-88df-2926d3529026`
  （`2026-07-08_南京行程.html` → `index.html`；`2026-07-08_南京行程地圖.html` → `map.html`；暫存目錄用完即刪，不進版控）
- 每次改完本機 HTML 都要重新跑上述指令部署，否則網站不會更新。
- 本機 Node.js 於 2026-07-24 重新安裝（v24.18.0），Netlify CLI（26.1.0）授權沿用既有 `~/.netlify/config`。
- `.netlify/`（CLI 於專案內產生的機器專屬設定）已加入根目錄 `.gitignore`，不進版控。

## 目前狀態

- 2026-07-24：8/2–8/8 南京行程 HTML（含地圖版）已從 Google Drive legacy 來源複製進本機工作區、加入 Git，並部署上線至 Netlify。
- 2026-07-24：標題列加上「最新修改日期」紅字標籤（桌面版釘右、手機版置中），與頁尾更新日期同步。
- 2026-07-24：Day 7（8/8）行程改為官方確認時刻表——「阿里雲谷參訪・返程」：07:15 南京酒店集合搭大巴 → 08:46 高鐵 G7611 南京南→杭州東（10:08 抵達，第二批次：台灣／新加坡／泰國）→ 接駁車前往阿里雲谷 → 11:10–12:00 參觀 → 12:00–13:30 餐敘 → 13:30–15:30 專家分享與交流 → 15:30 結束搭車返杭州東站 → 杭州東→上海虹橋（時刻待確認）→ 19:40 長榮飛松山。兩段高鐵車票與接駁車皆標註「由用友Tina協助購買/安排，費用回台後結算給Tina」。
- 2026-07-24：新增「📋 追蹤待辦」區塊——已知參訪台商：太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科；待辦：8/7–8/8 與台商交流、評估用友ERP使用情形。
- 出行人員、工作目的（用友商業創新大會，8/7）與其餘每日行程細節已在 HTML 內，尚待逐一核對是否為最新版本。

## 待確認

- 杭州東→上海虹橋高鐵確切車次與時刻（待用友Tina或本人確認後補上，需同步更新 index.html 並重新部署）。
- 8/7–8/8 與台商（太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科）交流用友ERP評估的具體安排與結論待後續補充。
- 其餘 Day 1–6 行程內容是否為最新版本（是否有異動未反映在此 HTML）。
- 是否需要把票務、住宿、交通、會議資料另存進專案。
