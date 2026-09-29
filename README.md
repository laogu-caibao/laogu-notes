# 调研纪要解读

`laogu-notes`

机构调研/电话会纪要解读 skill：输入纪要文本或链接，结构化提炼核心问答、关键数字、边际变化与未回答点。

## 一键安装

仓库地址（点击复制）：

`https://github.com/laogu-caibao/laogu-notes`

**方式一：克隆**

```bash
git clone https://github.com/laogu-caibao/laogu-notes.git
```

**方式二：下载 ZIP**

https://github.com/laogu-caibao/laogu-notes/archive/refs/heads/main.zip

**导入使用**

- Claude Code / Muse：把仓库中的 `SKILL.md` 放到 `~/.claude/skills/laogu-notes/` 下即可调用。
- 豆包智能体 / Workbuddy 等：按各平台的 skill 上传流程导入 `SKILL.md`。
- 扣子 Coze：扣子编程 → 技能面板 → 创建技能 → 本地上传，上传本仓库打包的 zip（仓库根目录已有 SKILL.md，直接压缩仓库文件夹即可）；如页面要求 `.skill` 后缀，由扣子导入后自动生成，不要只改扩展名。
- Trae：设置 → 技能 → 上传技能，上传同上 zip；或手动放到 `~/.trae/skills/laogu-notes/`（项目级用 `.trae/skills/laogu-notes/`）。Trae 也支持 MCP：把 `uvx laogu-mcp` 配进 MCP 设置即可获得 16 个工具（skill 负责流程指导、MCP 负责工具调用）。
- 一次装好全部 16 个：用 [laogu-mcp](https://github.com/laogu-caibao/laogu-mcp)，`uvx laogu-mcp` 一键安装。
## 文件结构

- `SKILL.md` — 主流程（平台中立，需用户输入纪要文本/链接，不设自动运行）
- `references/sources.md` — 数据源：纪要搜索模板、互动易/e互动官方渠道

## 输出结构

- 基本信息：公司、调研时间、调研方式、主要参与机构、管理层出席
- 核心问答 3-5 条：问题 → 管理层口径原话引用 → 一句话白话转译
- 关键数字与指引：产能/订单/毛利率/资本开支等，标注边际变化
- 边际变化一句话：本次相对上次最大的变化
- 分歧与未回答点：管理层回避或模糊的问题、"原文未披露"项、口径与市场预期的分歧

## 使用示例

- 「这是宁德时代9月调研纪要全文：……」→ 输出结构化解读
- 「宁德时代9月调研纪要」→ 先按搜索模板找纪要内容，搜不到则列缺失要素

---
## 出品

**老谷拆财报** —— 以数据为刃，剖市场真相

- 抖音 / 微信视频号 / 今日头条 / 快手：搜索「老谷拆财报」
- 固定栏目：「价值投资之财报解读」（全网连载中）
- 本 skill 的方法论与账号内容同源：数据驱动、拆开看、不讲黑话

### 扫码关注

| 微信视频号 | 抖音 |
|---|---|
| ![视频号二维码](docs/qrcode-shipinhao.jpg) | ![抖音二维码](docs/qrcode-douyin.png) |
| 扫一扫，关注视频号 | 抖音号：gubaobao22 |

> 作者声明：个人观点，仅供参考，不构成投资建议。
