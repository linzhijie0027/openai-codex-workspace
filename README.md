# openai-codex-workspace

供 OpenAI Codex 编写、运行和管理代码的工作仓库。

这是一个可直接运行的 Node.js 起步项目，可在后续需求中扩展成网站、工具或其他应用。

## 运行

需要 Node.js 22 或更高版本。当前没有第三方依赖，无需安装依赖或配置 API 密钥。

```sh
npm start
```

预期输出：

```text
你好，Codex！
代码运行成功，可以开始在这个仓库中开发你的项目。
```

也可以传入名字：

```sh
npm start -- 小林
```

检查代码语法：

```sh
npm run check
```

## 在 Codex 云端使用

仓库文件准备好后，还需要在 Codex 中完成云端环境设置；提交代码本身不会自动完成连接。

1. 在 ChatGPT 网页或桌面端选择云端工作模式，创建或选择云端环境。
2. 选择 GitHub 仓库 `linzhijie0027/openai-codex-workspace`；如有提示，完成 GitHub 连接。
3. 让 Codex 检查项目。运行时需要 Node.js 22 或更高版本，当前无需安装第三方依赖。
4. 使用 `npm run check` 检查语法，再用 `npm start` 验证示例运行。
5. 检查环境设置和验证结果，保存并发布环境，然后开始任务。

可发送的第一个任务：

> 请阅读 README.md 和 AGENTS.md，运行基础示例并检查语法，报告结果。

官方说明：[Codex Cloud](https://learn.chatgpt.com/docs/cloud)

## 文件说明

- `src/index.js`：可运行的示例入口。
- `package.json`：启动和语法检查命令。
- `AGENTS.md`：Codex 在此仓库中的工作说明。
- `.gitignore`：忽略依赖、构建产物和本地敏感配置。

这是开发工作仓库；实际应用功能可以通过后续任务添加。
