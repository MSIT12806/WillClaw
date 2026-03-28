# Repository Memory  

## Stable Context  
- **Issue‑driven工作流程**：所有需求、決策與任務皆以 GitHub Issue 為唯一原始資料來源。  
- **手動長期筆記 (`shared/manual.md`)**：保存 **穩定規則、長期決策、常見限制、repo 習慣**，供 `compact‑memory` 工作流讀取，且 **不會被自動覆寫**。  
- **Issue 模板建議**：  
  1. **Title**（簡潔描述）  
  2. **Background**（問題背景與動機）  
  3. **Goal / Objective**（期望達成的結果）  
  4. **Acceptance Criteria**（驗收條件）  
  5. **Constraints**（相關限制或前置條件）  
- **標籤與指派機制**：每個 Issue 應在建立時即設定 **適當的 label**（如 `feature`, `bug`, `question`）與 **負責人**，以提升可見性與追蹤效率。  
- **溝通渠道統一**：若 Issue 需要補充說明，建議使用 **Telegram / Slack** 作為即時討論平台，並在 Issue 中加入 **討論連結或摘要**。  
- **每日快照 (`daily/*.json`)**：由一群「龍蝦」 agents 依當天活躍的 Issue 產出，內容僅作為 **記憶蒸餾**，不會直接寫入 repo。  

## Recent Themes  
| 主題 | 觀察次數 (最近 7 天) | 具體描述 |
|------|-------------------|----------|
| 資訊缺口 / 需求
