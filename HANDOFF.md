# HANDOFF

## 架構同步（2026-08-01）

- 已依 `project-init-sync` 對照已驗證架構版本：`agent-sync-v1.2.3`。

## 目前做到哪

南京行程已使用獨立 repo 管理，正式公開頁為 GitHub Pages：`https://scotthcliu-jpg.github.io/2607-nanjing-youyou-trip/`。Day 7（8/8）兩段高鐵已由用友 Tina 確認並寫入行程頁：G7609 南京南 08:51→杭州東 10:19；G7644 杭州西 15:32→上海虹橋 16:55。

## 目前狀態

- 本次同步已補正 `PROJECT.md`、`HANDOFF.md` 與 Obsidian 索引；下次接手前仍須執行 `project-startup` 重新驗證工作樹與遠端。

## 接手狀態

- handoff_ready: yes
- session start commit: `112466e16c85b96ac81a3892c94798256b437e3a`
- expected branch: `main`
- expected Git root: `C:\Users\user\Documents\Codex\2026Claude\100_Todo\projects\active\2607南京用友出行`
- expected remote: `https://github.com/scotthcliu-jpg/2607-nanjing-youyou-trip.git`
- last sync verification: `2026-08-01 18:00 +08:00 於 TZNB1169`；修改前以 fresh `git ls-remote origin refs/heads/main` 確認 `112466e16c85b96ac81a3892c94798256b437e3a` 的 local HEAD = remote HEAD。
- last updater: `Codex @ TZNB1169`
- next Agent rule: 可接手，先在本機 NTFS 路徑執行唯讀 `project-startup`；任何閘門失敗即停止。

## 下一步

1. 依使用者核對結果修正 Day 1–6 行程內容；必要時同步更新公開 GitHub Pages。
2. 8/7–8/8 與台商（太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科）交流用友ERP評估，安排／結論確定後補進行程頁「追蹤待辦」區塊。
3. 於出發前依 Tina 的出票紀錄確認座位與即時開行資訊。

## 注意事項

- 正式公開頁由 GitHub Pages 的 `main` branch 根目錄提供；`index.html` 會轉址至 `2026-07-08_南京行程.html`，`map.html` 會轉址至地圖頁。Netlify 為舊部署，勿再使用。
- 專案 pre-commit 已啟用並實測 canonical-sync guard：行程或其他內容異動必須與 `PROJECT.md`、`HANDOFF.md` 同一 commit；禁止以 `--no-verify` 繞過。Guard 安裝腳本亦已在本專案重跑驗證，會保留既有 hook。
- 行程、票務、住宿、Tina 對接、參訪台商名單等內容含商業機敏性質，不要不必要外傳。
- 本機共用 monorepo checkout 常有其他並行 Agent session 同時在別的專案資料夾下操作；commit 時務必用明確 pathspec（`git commit -- <path>`）只提交本專案檔案，勿用裸 `git commit -m` 吞掉別人 staged 的異動。push 前一定要先 `git fetch` 並確認 `origin/main` 是 `HEAD` 的祖先（fast-forward 安全）才 push。
- 本機 Bash 工具偶爾會出現 coreutils（mkdir/cp/ls）找不到的狀況，此時改用 PowerShell 執行檔案操作與 git 指令即可。

## 同步狀態

| 層級 | 狀態 |
|---|---|
| Execution 本機 NTFS | 本機 NTFS 獨立 repo；下次接手前須執行 `project-startup` |
| Version GitHub | `main` branch；下次接手前須以 fresh remote query 驗證 |
| Knowledge Google Drive | unchanged（本次未回寫 G 槽，G 槽仍為唯讀 legacy 來源） |
| Obsidian | 已更新 `G:\我的雲端硬碟\第二大腦\Projects\2607南京用友出行.md` |
| Public site | GitHub Pages：`https://scotthcliu-jpg.github.io/2607-nanjing-youyou-trip/` |

## 最後更新

- 時間：2026-08-01 18:00 +08:00
- 更新者：Codex @ TZNB1169
