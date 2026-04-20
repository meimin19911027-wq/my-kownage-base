
  每次运行 Agent 时发送的初始 Prompt，明确任务目标。
  # Agent 启动指令
  **任务目标**: 同步并分析知识库内容
  **输入选项**:
  1. `sync` - 从远程 Wiki 拉取最新内容
  2. `search <关键词>` - 搜索本地缓存
  3. `edit <文件名>` - 编辑指定页面（需人工审核）

  **示例命令**:
  ```bash
  python agent.py sync  # 同步 Wiki
  python agent.py search API  # 搜索关键词

  安全提醒:
  - 所有编辑操作将记录到 agent_logs/
  - 禁止绕过权限直接推送内容！

  ---
