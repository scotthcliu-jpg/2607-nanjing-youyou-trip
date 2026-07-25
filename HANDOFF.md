# HANDOFF

## 目前做到哪

Day 7（8/8）行程已改為官方確認時刻表（07:15集合→高鐵G7611南京南→杭州東→阿里雲谷參訪→餐敘→專家交流→15:30返程），並新增「📋 追蹤待辦」區塊記錄已知參訪台商名單與 8/7–8/8 用友ERP評估交流待辦。已部署上線並 push GitHub。

## 目前狀態

- clean（本專案工作樹乾淨，local HEAD = remote HEAD）

## 接手狀態

- handoff_ready: yes
- session start commit: `3ba277b9ed65e454916e45e76ba7526582b3f557`
- expected branch: `main`
- expected remote: `https://github.com/scotthcliu-jpg/my-agent-2026.git`
- last sync verification: 見本次收工回報的 commit hash（fresh `git ls-remote` 已確認 local HEAD = remote HEAD）
- last updater: `Claude Code @ TZNB1169`
- next Agent rule: 可接手，先在本機 NTFS 路徑執行唯讀 `project-startup`；任何閘門失敗即停止。

## 下一步

1. 向用友Tina／自行確認杭州東→上海虹橋高鐵確切車次與時刻，補進 `2026-07-08_南京行程.html`，並用 `netlify deploy --prod --dir=<暫存目錄含 index.html/map.html> --site=8f7231c2-e5c7-4d62-88df-2926d3529026` 重新部署。
2. 8/7–8/8 與台商（太古汽車、旺旺、訊威、華新麗華、老子鍋、中華汽車、大世科）交流用友ERP評估，安排/結論確定後補進行程頁「追蹤待辦」區塊。
3. 逐一核對 Day 1–6 行程內容是否為最新版本。

## 注意事項

- 部署前務必把 `index.html`（=行程主頁）與 `map.html`（=地圖頁）放進暫存目錄再 `netlify deploy`，暫存目錄本身不進 Git；`.netlify/` 已在根目錄 `.gitignore` 排除。
- 行程、票務、住宿、Tina 對接、參訪台商名單等內容含商業機敏性質，不要不必要外傳。
- 本機共用 monorepo checkout 常有其他並行 Agent session 同時在別的專案資料夾下操作；commit 時務必用明確 pathspec（`git commit -- <path>`）只提交本專案檔案，勿用裸 `git commit -m` 吞掉別人 staged 的異動。push 前一定要先 `git fetch` 並確認 `origin/main` 是 `HEAD` 的祖先（fast-forward 安全）才 push。
- 本機 Bash 工具偶爾會出現 coreutils（mkdir/cp/ls）找不到的狀況，此時改用 PowerShell 執行檔案操作與 git 指令即可。

## 同步狀態

| 層級 | 狀態 |
|---|---|
| Execution 本機 NTFS | clean |
| Version GitHub | 已 commit 並 push，local HEAD = remote HEAD（見最終回報 commit hash） |
| Knowledge Google Drive | unchanged（本次未回寫 G 槽，G 槽仍為唯讀 legacy 來源） |
| Obsidian | 已更新 `G:\我的雲端硬碟\第二大腦\Projects\2607南京用友出行.md` |
| Netlify | 已部署，production URL 與內容一致 |

## 最後更新

- 時間：2026-07-24
- 更新者：Claude Code @ TZNB1169
