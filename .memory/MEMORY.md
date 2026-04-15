# Repository Memory  

## Stable Context  
- **Issue‑Driven工作流程**：所有工作皆以 GitHub Issue 為單位，原始需求、討論與決策必須寫在 Issue 的 comment 中，agents 只會根據這些資料行動。  
- **手動筆記的角色**：`shared/manual.md` 用於保存長期穩定規則、決策與 repo 習慣，agents 會在讀取時參考但不會覆寫此檔。  
- **資訊來源原則**：  
  1. **GitHub Issue / Comment** 為唯一可信的事實來源。  
  2. 任何未在 Issue 中明確說明的需求，都視為「資訊缺失」且不會觸發後續執行。  
- **Agents 的行為守則**：  
  - 只在 Issue 具備完整目標、範圍與驗收標準時開始任務拆解與追蹤。  
  - 若 Issue 內容不足，agents 會將缺口記錄為 **Open Loop**，並以「等待主人提供資訊」的方式提醒。  
- **Compact‑Memory 工作流程**：每日快照會被蒸餾成長期可重用的記憶，手動筆記不會被自動覆寫，確保穩定規則的持續可見性。  

## Recent Themes  
| 主題 | 觀察次數 (最近 30 天) | 說明 |
|------|----------------------|------|
| **需求缺失 / 資訊不明** | 7 次 (4/9‑4/15) | Issue #1 只有標題，缺乏需求說明、目標或驗收條件，導致所有 agents 無法展開工作。 |
| **等待回覆** | 7 次 | 每日快照皆顯示 agents 正在等待主人在 Issue 中提供具體
