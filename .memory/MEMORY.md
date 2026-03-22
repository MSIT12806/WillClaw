# Repository Memory

## Stable Context
- **Repository**: `MSIT12806/WillClaw`  
- **核心角色**：  
  - **第一隻雲蝦** 被定位為「需求接收與工作項目轉換」的前線中樞，負責將 Telegram 中的需求以 JSON 形式送入 GitHub，建立 Issue。  
- **工作流程**：  
  1. 主人在 Telegram 收到需求 → 透過 JSON 送出 → Lobster Agent 建立 GitHub Issue。  
  2. 後續將由自動化流程解析 JSON、產生子任務、並自動指派負責人。  
- **資料來源原則**：所有事實與決策必須以 GitHub Issue / Comment 為唯一原始資料來源；手動維護的 `shared/manual.md` 只作為長期規則與限制的備註，不會被覆寫。  
- **共通慣例**：  
  - 每次「需求即時化」皆以 Issue 為單位記錄。  
  - 代理人（Lobster Agents）共享同一套 repo 習慣：遵守 issue 限額、使用標籤（未來需建立）以及在 30 天窗口
