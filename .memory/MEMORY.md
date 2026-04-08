# Repository Memory  

## Stable Context  
- **Issue 管理規範**：所有 GitHub Issue 必須在建立後即提供完整的需求說明、目標與驗收標準，並指派負責人或至少加上適當的標籤，以便後續追蹤與排程。  
- **Agent 工作流程**：  
  1. 每日由一群「龍蝦」 agents 讀取 `.memory/agents/*.json`，彙整當天的 Issue 狀態。  
  2. 產出 daily snapshot（JSON）並寫入 `daily/YYYY-MM-DD.json`。  
  3. 若發現資訊缺口，於 **Open Loops** 中標註，等待主人補充。  
  4. `shared/manual.md` 為人類手動維護的長期記憶，僅供參考，不會被 agents 覆寫。  
- **Repo 習慣**：  
  - 只追蹤最近 30 天內的 Issue（上限 100 件）。  
  - 以「資訊缺口」作為跨 Issue 主題的第一層警示。  
  - 決策只能在需求明確後由主人或指定決策者下達，agents 只負責記錄與提醒。  

## Recent Themes  
- **資訊缺口持續出現**：過去 7 天的 daily snapshots 均只看到 Issue #1，且內容全為空白，導致 agents 無法進行任何實作或決策。  
- **需求澄清需求**：每一天都重複提醒主人補充 Issue #1 的目標、需求、類別（新功能 / Bug / 其他）。  
- **缺乏指派與標籤**：沒有任何負責人或標籤資訊，影響後續的工作分配與優先級排序。  
- **決策停滯**：因需求未明，所有「Decisions」欄位皆顯示「無」或「未記錄」。  

## Constraints  
1. **資訊完整性**：在缺乏需求說明前，agents 不得自行推測 Issue 類別或產生執行計畫。  
2. **不
