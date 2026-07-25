# 2607南京用友出行 專案協作規則

## 執行位置閘門（優先規則）

- 唯一可編輯與執行的專案路徑：`C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行`。
- Version Git root：`C:\Users\user\Documents\Codex\2026Claude`；remote：`https://github.com/scotthcliu-jpg/my-agent-2026.git`；branch：`main`。
- Google Drive 專案路徑只作為 Knowledge／legacy source；禁止在 G 槽編輯、測試、建立 Git repo 或 commit。
- 「開工／接續」一律使用 `project-startup`；舊 `project-kickoff` 已刪除。
- `handoff_ready` 不是 `yes`、工作樹不乾淨或 local HEAD 不等於 remote HEAD 時，必須停止並回報 `blocked`。

## 專案定位
本檔案是此專案的 AI Agent 協作入口，供 Claude Code 與 Codex 共用。若本專案另有更細的需求文件、會議紀錄或規格文件，執行前需先讀取並以最新明確指示為準。

## 工作原則
- 回覆優先使用繁體中文，語氣簡潔、白話、專業。
- 先用 BLUF 說結論，再補充必要背景、風險與下一步。
- 未確認前，不刪除、不覆蓋、不搬移重要檔案。
- 涉及外部系統、雲端文件、GitHub、Google Workspace、MCP 或部署時，先確認目標與權限。
- 對具體數據、法規、價格、時程、政策與外部事實，需查證來源；資料不足時直接說明「資料不足，無法確認」。

## 執行流程
1. 先確認目前工作目錄、專案根目錄與是否有 Git 狀態。
2. 讀取本專案的 `CLAUDE.md` / `AGENTS.md` 及相關 context 文件。
3. 釐清使用者要求的交付物、範圍與不可動的檔案。
4. 若是程式或文件修改，先盤點現況，再進行最小必要變更。
5. 完成後回報修改內容、驗證結果與尚未處理的風險。

## Claude Code / Codex 同步規則
- `CLAUDE.md` 與 `AGENTS.md` 應保持內容一致。
- 修改其中一份時，需同步更新另一份。
- `CLAUDE.md` 供 Claude Code 使用；`AGENTS.md` 供 Codex 使用。
- 不同步 session 歷史，只沉澱可重複使用的規則、決策、偏好與流程。

## 專案備註
- 專案名稱：2607南京用友出行
- 建立日期：2026-07-13
- 待補充：專案目標、主要資料來源、常用指令、驗證方式、重要限制。
