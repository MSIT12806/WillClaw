# Repository Memory

## Stable Context
- **Repository**: `MSIT12806/WillClaw`  
- **工作流程**  
  - 所有工作皆以 GitHub Issue 為單位展開。  
  - 每日由「龍蝦」agents 讀取 Issue，檢查 **標題、說明、回覆、標籤、指派** 四大要素。  
  - 若要進一步拆解任務、排程或做決策，必須先取得 **完整需求說明**（問題描述、預期成果、驗收標準）。  
- **長期規則**（來源：`shared/manual.md`）  
  1. **穩定規則**：所有 Issue 必須在建立時即填寫完整說明，缺失說明的 Issue 會被標記為 *資訊缺口*，並暫停後續處理。  
  2. **長期決策**：在需求確定後，先產出 **工作分解 (WBS)**，再依優先度排入里程碑。  
  3. **常見限制**：  
     - 未指派負責人或缺少標籤的 Issue 會被視為 **待分配**，不會自動進入執行階段。  
     - 每日 agents 只會處理 **最近 30 天內**、**狀態為 open** 的 Issue，且上限 100 件。  
  4. **Repo 習慣**：  
     - 每日結束前，agents 必須產出四段摘要：`Agent Activity`、`Cross‑Issue Themes`、`Decisions`、`Open Loops`。  
     - 任何 **Open Loop** 必須在下一次主人回覆前保持在 `MEMORY.md` 的「Open Loops」區塊，以免遺失。  

## Recent Themes
| 主題 | 出現頻率 (最近 7 天) | 觀察 |
|------|-------------------|------|
| **資訊缺口 / 需求說明缺失** | 7/7 天 | Issue #1 只有
