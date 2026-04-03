# Repository Memory

## Stable Context
- **Issue 完整性規則**  
  - 每個 Issue 必須至少包含 **標題、描述、目標/需求**，缺一不可。  
  - 必須指派負責人或明確標示「待指派」狀態。  
  - 必須加上適當的 **Label**（如 `needs‑info`、`triage`）以利後續追蹤。  

- **資訊收集流程**  
  - 龍蝦隊伍會在每日結束時將所有 Issue 的結構寫入 `.memory/agents/issue-<id>.json`，確保每個議題都有可追溯的記錄。  
  - 若 Issue 仍屬「資訊不明」狀態，會自動標記為 **Open Loop**，等待主人提供補充資料。  

- **決策產出條件**  
  - 只有在需求說明完整、目標明確且已指派負責人後，才會產生 **Decision**（決策）與 **Execution Plan**（執行計畫）。  

- **手動筆記 (shared/manual.md) 的角色**  
  - 用於保存 **長期穩定規則、決策、常見限制與 repo 習慣**。  
  - 只作為參考，**不會被自動覆寫**，且不應直接複製 Issue 原文。  

- **系統參數**  
  - Repository: `MSIT12806/WillClaw`  
  - Issue 觀察範圍：最近 30 天、上限 100 件  
  - Daily snapshot 產出方式：`llm‑refine` 產生的 JSON 檔案  

## Recent Themes
- **資訊缺口 / 需求澄清**  
  - 連續 7 天（2026‑03‑28 至 2026‑04‑03）唯一的 Issue #1 均缺
