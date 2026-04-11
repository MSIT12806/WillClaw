# Repository Memory

## Stable Context
- **Repository**: `MSIT12806/WillClaw`  
- **Issue Management**  
  - 每個 Issue 必須在建立時提供完整的 **需求說明、目標、交付成果與驗收標準**。  
  - 缺乏說明的 Issue 會被標記為 *資訊缺口*，並暫停任何任務拆解或指派。  
  - 需要 **指派負責人**、**添加適當標籤**（如 `feature`、`bug`、`enhancement`）才能進入執行階段。  
- **Agent 行為準則**  
  - 龍蝦 agents 會每日掃描所有開放的 Issue，若發現資訊不足即產生 *Open Loop*，並在日誌中提醒主人。  
  - 當 Issue 具備完整資訊時，agents 會自動進行 **需求分解 → 任務排程 → 進度追蹤**。  
- **記憶工作流程**  
  - `shared/manual.md` 用於手動維護的長期記憶，僅保存 **穩定規則、長期決策、常見限制與 repo 習慣**，不會被自動覆寫。  
  - `daily/*.json` 為每日快照，供 agents 蒐集即時狀態，最終蒸餾至本文件的 **Stable Context**、**Recent Themes**、**Constraints** 與 **Open Loops**。  

## Recent Themes
- **資訊缺口持續出現**：過去 7 天的所有快照皆只看到 Issue #1，且內容僅有標題，缺乏任何需求說明。  
- **等待主人回覆**：每一天的 agents 報告均指出「等待主人提供具體需求」是唯一阻礙進度的因素。  
- **需求澄清需求**：多次提到需要主人說明 Issue #1 的 **問題描述、功能需求、預期交付與驗收標準**，才能展開任務分解。  
- **缺少標籤與指派**：在缺乏需求的同時，亦缺少對 Issue 的類別標籤與負責人指派，導致無法自動化排程。  

## Constraints
1. **必須提供完整需求說明**：Issue 內容若僅有標題，agents 視為資訊不足，所有後續流程（分解、排程、追蹤）將被擱置。  
2. **需求說明必須包含**  
   - 問題或功能的具體描述  
   - 預期交付物（程式碼、文件
