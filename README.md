# Obsidian Starter Vault｜奶油白 × 鼠尾草绿的极简知识工作台

> 一套基于 Obsidian 的浅色系知识库配置模板：柔和的奶油白编辑区、低饱和鼠尾草绿界面、圆角分栏布局，以及可按需启用的 AI 对话与知识管理插件。

<img width="1440" height="828" alt="image" src="https://github.com/user-attachments/assets/b4594961-135a-4c66-8c22-f66d6424219b" />


> **截图说明**：提供的截图展示了浅色主题、左侧文件导航、中间编辑工作区，以及右侧 AI 对话面板。

## 01｜项目简介

**Obsidian Starter Vault** 是一套可复用的 Obsidian 工作区配置，重点不是提供大量预制笔记，而是将主题、CSS 样式、插件及常用界面设置整理为一个开箱可用、方便二次定制的起点。

当前界面采用**奶油白与灰绿色**的低饱和配色。左侧为文件与功能导航，中间为主要笔记编辑区，右侧展示 AI 对话面板。大面积留白、圆角容器和相对克制的图标配色，让写作、检索和 AI 辅助工作可以在同一个窗口中进行。

本仓库适合希望快速搭建个人知识库、课程笔记空间、项目文档库，或喜欢浅色、柔和视觉风格的 Obsidian 用户。

## 02｜界面设计

### 奶油白与鼠尾草绿

截图中的主编辑区与侧栏以温暖的奶油白为底色，外层界面使用灰绿色作为视觉衬托；标题、图标和控件采用低饱和配色，避免强对比造成的视觉负担。整体设计更接近安静、轻量的个人知识工作台，而非密集的信息仪表盘。

### 三栏工作布局

| 区域         | 截图中的表现                                               | 适用场景                           |
| ------------ | ---------------------------------------------------------- | ---------------------------------- |
| 左侧导航     | 文件树、常用操作图标及功能侧边栏                           | 管理笔记、切换工作区               |
| 中间工作区   | 大面积浅色编辑区，独立圆角面板                             | Markdown 写作、阅读与整理          |
| 右侧 AI 面板 | OpenCode 对话入口、模型选择、Recent Chats / Relevant Notes | 对话、辅助构思与结合笔记提供上下文 |

右侧 AI 面板的实际模型、可用命令及笔记上下文能力取决于所安装插件的版本与用户自己的配置；截图本身不代表已完成任何特定模型或服务的授权。

### 自定义 CSS

仓库包含以下七个 CSS 片段，可在 Obsidian 的 **设置 → 外观 → CSS 代码片段** 中分别启用：

| CSS 文件                    | 用途                           |
| --------------------------- | ------------------------------ |
| `custom-accent.css`         | 自定义整体强调色及相关界面配色 |
| `custom-rainbow-colors.css` | 补充多色层级视觉样式           |
| `floating-search-bar.css`   | 搜索栏的浮动式视觉处理         |
| `floating-status-bar.css`   | 状态栏的浮动式视觉处理         |
| `hide-collapse-arrow.css`   | 调整或隐藏折叠箭头显示         |
| `home-dashboard.css`        | 为首页仪表盘提供专用样式       |
| `minimal-cards.css`         | 简洁圆角卡片样式               |

不同主题、Obsidian 版本或插件可能影响 CSS 的最终效果。如果某个片段与现有主题冲突，可以单独关闭，不必停用整套模板。

## 03｜主题与插件

### 主题

仓库包含 **AnuPpuccin** 和 **Velocity** 两套主题文件。当前截图呈现的是柔和的浅色工作区效果；实际显示效果还受到 Obsidian 外观设置、主题参数和 CSS 片段共同影响。

### 随仓库整理的插件

| 插件目录                  | 主要用途                                             |
| ------------------------- | ---------------------------------------------------- |
| `dataview`                | 根据笔记元数据生成动态列表和查询结果                 |
| `obsidian-icon-folder`    | 为文件夹或文件设置更直观的图标                       |
| `obsidian-style-settings` | 在设置界面调整受支持的主题和 CSS 参数                |
| `chatting-with-ai`        | 在 Obsidian 中提供 AI 对话相关功能                   |
| `copilot`                 | 提供另一种 AI 辅助工作入口；具体功能依版本与配置而定 |

截图右侧显示的 OpenCode 对话面板应以实际安装和启用的插件为准。模板中的插件程序文件不等于已经配置好可直接使用的 AI 账号或 API 服务。

**隐私提醒：** 仓库刻意不提供 `chatting-with-ai/data.json` 等个人 AI 配置文件。下载者需要自行登录或配置所使用的服务，切勿将访问令牌、API Key、聊天记录或私人笔记提交到公开仓库。

## 04｜文件结构

```text
obsidian-starter-vault/
├── .obsidian/
│   ├── app.json
│   ├── appearance.json
│   ├── community-plugins.json
│   ├── core-plugins.json
│   ├── graph.json
│   ├── plugins/
│   │   ├── chatting-with-ai/
│   │   ├── copilot/
│   │   ├── dataview/
│   │   ├── obsidian-icon-folder/
│   │   └── obsidian-style-settings/
│   ├── snippets/
│   │   ├── custom-accent.css
│   │   ├── custom-rainbow-colors.css
│   │   ├── floating-search-bar.css
│   │   ├── floating-status-bar.css
│   │   ├── hide-collapse-arrow.css
│   │   ├── home-dashboard.css
│   │   └── minimal-cards.css
│   └── themes/
│       ├── AnuPpuccin/
│       └── Velocity/
├── .gitignore
└── README.md
```

以上为目前整理的主要配置目录；个人数据文件和系统生成的临时文件不属于需要公开分享的模板内容。

## 05｜安装与使用

### 方法一：下载为 ZIP

1. 打开本仓库，点击绿色的 **Code → Download ZIP**。
2. 解压后，将文件夹放到你希望保存知识库的位置。
3. 在 Obsidian 中选择 **打开本地仓库文件夹**，选中解压后的目录。
4. 根据 Obsidian 的安全提示决定是否启用社区插件；建议先检查插件列表和版本。
5. 进入 **设置 → 外观**，选择喜欢的主题，并启用所需的 CSS 片段。

### 方法二：使用 Git 克隆

```bash
git clone git@github.com:shenjianlu2-crypto/obsidian-starter-vault.git
```

如果尚未配置 GitHub SSH，也可以使用 HTTPS：

```bash
git clone https://github.com/shenjianlu2-crypto/obsidian-starter-vault.git
```

然后使用 Obsidian 打开克隆后的目录。

### 应用于已有知识库

建议先备份已有知识库的 `.obsidian` 文件夹，再有选择地复制 `snippets/`、`themes/` 和需要的插件配置。不要直接覆盖现有 `.obsidian`，否则可能改变原有快捷键、外观、插件和工作区设置。

## 06｜推荐使用方式

**学习笔记：** 使用文件夹组织课程内容，配合 Dataview 汇总最近更新或指定标签的笔记。

**项目文档：** 为每个项目建立独立目录，使用统一的笔记命名方式记录需求、进展、技术方案与复盘。

**AI 辅助写作：** 在右侧 AI 面板中进行思路整理、草稿讨论或问题拆解。涉及私密资料时，先确认所使用 AI 服务的数据处理方式及插件权限。

**个性化首页：** 使用 `home-dashboard.css` 和 Dataview 自行搭建工作、学习、项目及日常记录入口。此仓库包含首页样式，但是否包含完整可直接运行的首页笔记，应以实际仓库文件为准。

## 07｜个性化调整

- **修改整体颜色：** 从 `custom-accent.css` 入手，按自己的审美调整强调色和背景色。
- **调整卡片与留白：** 修改 `minimal-cards.css`，或按需停用某些 CSS 片段。
- **更换主题：** 在 AnuPpuccin 和 Velocity 之间切换，观察现有 CSS 是否需要适配。
- **减少界面干扰：** 按需折叠左侧文件栏或关闭右侧 AI 面板，将空间留给当前笔记。

建议每次只调整一类样式，并保留原文件副本，方便回退。

## 08｜隐私与维护

本项目旨在分享**工作区配置**，不包含作者的私人笔记、AI 登录凭证或个人聊天数据。公开提交前，应特别检查 `.obsidian/plugins/` 下的 `data.json`、本地日志和其他可能包含 Token 的文件。

插件和主题由各自开发者维护；模板提供的是当前整理的配置快照。后续升级 Obsidian 或社区插件时，建议先备份再验证兼容性。

## 09｜项目地址

GitHub：[shenjianlu2-crypto/obsidian-starter-vault](https://github.com/shenjianlu2-crypto/obsidian-starter-vault)

欢迎根据自己的使用习惯调整主题、布局、CSS 与插件，构建适合自己的知识工作台。
