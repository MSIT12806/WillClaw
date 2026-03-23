# Repository Memory  

## Stable Context  
- **前線任務中樞**：第一隻雲蝦被確立為「需求接收與工作項目轉換」的核心角色，負責將主人於 Telegram 以 JSON 形式送出的需求即時建立為 GitHub Issue。此角色定位是所有未來 Lobster Agent 必須遵循的基礎流程。  
- **資訊同步管道**：Telegram → JSON → GitHub Issue 已成功驗證，成為跨 Agent 的可靠資料流。  
- **手動筆記的定位**：`shared/manual.md` 只保存 **穩定規則、長期決策、常見限制與 repo 習慣**，不會被自動流程覆寫；所有原始需求仍以 Issue / Comment 為唯一事實來源。  
- **Issue 管理範圍**：系統在每次快照中檢視最近 30 天、最多 100 個 Issue，僅在此窗口內進行蒐集與分析。  

## Recent Themes  
- **需求即時化**：持續出現「把 Telegram 需求即時轉為可追蹤工作項目」的需求，所有 Agent 都圍繞此核心任務展開。  
- **自動化與指派**：雲蝦的未來工作包括自動解析 JSON、產生子 Issue / Task、以及自動指派負責人，這是跨需求類型的共通挑戰。  
- **待指派工作**：目前僅有角色宣告，缺乏具體需求，顯示系統仍處於「需求入口」階段，尚未進入「執行」層面。  
- **資訊同步成功**：從 Telegram 到 GitHub 的同步已在兩天內穩定運作，為後續多 Agent 協作奠定基礎。  

## Constraints  
- **需求必須以 JSON
