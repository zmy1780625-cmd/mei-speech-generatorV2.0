# 🎙️ 梅总 · 演讲稿生成器

基于 **shimei-perspective** Skill（石梅视角认知蒸馏）+ **GLM-4-Plus** 大模型，自动生成石梅风格的教育科技演讲稿。

> 石梅：腾讯云副总裁、腾讯教育负责人

## ✨ 特性

- 🧠 **真AI生成** — 接入智谱 GLM-4-Plus 大模型，非模板拼接
- 🧬 **Skill 驱动** — 4篇石梅原始演讲稿全文（~5000字）+ 完整表达DNA规则作为 System Prompt 注入，Few-shot 级语感对齐
- 📡 **流式输出** — SSE Stream 实时打字效果
- 🎯 **4种场合** — 全球大会 / 伙伴大会 / 高校发布会 / 学术研讨会
- 📝 **5种结构** — 政策呼应 / 成果回顾 / 产品发布 / 合作描述 / 战略展望
- 🎚️ **字数控制** — 600-2000字滑块调节
- 📤 **一键导出** — 复制全文 / 导出 .md / 导出 .txt
- 🔒 **Key 本地存储** — API Key 保存在浏览器 localStorage，不上传服务器
- 🚀 **零依赖部署** — 单个 HTML 文件，双击即可运行

## 📁 项目结构

```
shimei-speech-generator/
├── index.html                          # 演讲稿生成器（主文件，含GLM API集成）
├── skill/
│   ├── SKILL.md                        # 石梅视角 Skill v2.0（核心认知框架）
│   └── references/
│       ├── research/
│       │   ├── 01-writings.md          # 著作与系统思考调研
│       │   ├── 02-interviews.md        # 访谈与演讲调研
│       │   ├── 03-expression-dna.md    # 表达DNA深度分析
│       │   ├── 04-books-papers.md      # 书籍与研究报告
│       │   ├── 05-critics.md           # 批评视角与争议
│       │   └── 06-timeline.md          # 人生时间线
│       └── sources/
│           └── speeches-original.md    # 4篇原始演讲稿存档
├── README.md
├── LICENSE
└── .gitignore
```

## 🚀 快速开始

### 1. 获取 GLM API Key

前往 [智谱AI开放平台](https://open.bigmodel.cn/) 注册并获取 API Key。

### 2. 运行

```bash
# 方式一：直接双击打开
open index.html

# 方式二：用本地服务器
npx http-server -p 8080
```

### 3. 首次使用

点击「生成演讲稿」时，页面会弹窗要求输入 API Key（格式：`xxxxxxxx.yyyyyyyy`）。输入后自动保存到浏览器本地。

## 🧬 Skill 说明

`skill/SKILL.md` 是石梅视角的核心认知框架，基于 [nuwa-skill](https://github.com/alchaincyf/nuwa-skill) 方法论蒸馏而成：

| 模块 | 内容 |
|------|------|
| **5个心智模型** | All in AI 双轮驱动、LACC学用创赛、科技助教边界、倒推式产教融合、通用→学科递进 |
| **表达DNA** | 开场三部曲、标准自我介绍、三句九字、政策先行、数据驱动 |
| **固定表达** | "用户为本，科技向善"、"科技助教、连接兴学、专业为育"、"All in AI, AI in All" |
| **案例库** | 7个产品案例 + 4个高校合作案例（含精确数据） |
| **反模式** | 6条"石梅绝不会做的事" |

**一手资料来源**：4篇原始致辞稿（2025-2026年）

## 🛠️ 技术栈

- **前端**：纯 HTML + CSS + JavaScript（零框架依赖）
- **UI**：毛玻璃效果 + 渐变色 + [Lucide Icons](https://lucide.dev/)
- **AI**：[智谱 GLM-4-Plus](https://open.bigmodel.cn/)（OpenAI 兼容格式）
- **Skill方法论**：[nuwa-skill](https://github.com/alchaincyf/nuwa-skill)

## 📄 License

MIT License

## 🙏 致谢

- [nuwa-skill](https://github.com/alchaincyf/nuwa-skill) — 花叔的认知蒸馏方法论
- [智谱AI](https://open.bigmodel.cn/) — GLM-4-Plus 大模型
- [Lucide](https://lucide.dev/) — 线性图标库
