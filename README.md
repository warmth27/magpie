# magpie

所有 Agent 的模型，一处搞定。

magpie 是一个本地网关，把 Claude Code、Codex、Gemini CLI、OpenCode 等 Agent 的模型配置集中到一处管理：在列表里选择后，任意 Agent 都能使用任意 provider 的模型，并且只修改配置中该改的键，保留原有注释和格式。它支持 API key、本地模型，以及 Claude、ChatGPT、Copilot、Gemini、Grok 等订阅；当账号额度用尽时，会自动切换到下一个账号或路由组，Agent 不会看到报错。开启隐私脱敏后，密钥、密码和邮箱在请求离开电脑前就被遮蔽，收到回复时再还原。

magpie 适合同时使用多个 Agent、多个 provider 或多个账号的人。每个 Agent 可以维护独立的模型列表，Profiles 能把整套配置保存为一个名字，一键切换；命令行、TUI 和 Web 界面都能完成同样的操作。所有请求都经过本机网关，额度、账号和路由状态可以统一查看。它支持 macOS、Windows、Linux，也可运行在 Docker 和 Termux 上。

安装：`curl -fsSL https://usemagpie.ai/install.sh | sh`，更多信息见 [usemagpie.ai](https://usemagpie.ai)。
