# 综述写作工作流skill

这是一个独立的 Claude Code skill/plugin 仓库，用于把“从选题到定稿”的综述写作流程沉淀为可复用方法，而**不覆盖原始综述项目**。

## 它能做什么

本仓库将综述写作过程中的通用环节标准化为一个可调用 skill：

- 选题与范围界定
- 检索方案设计
- 候选文献池搭建
- 文献筛选与标签化
- 证据抽取与事实核查
- 提纲设计与图表规划
- 正文起草与修订
- 模拟审稿与回复
- Word 成稿整理

## 仓库结构

```text
综述写作工作流skill/
├─ .claude-plugin/
│  └─ plugin.json
├─ .gitignore
├─ CHANGELOG.md
├─ LICENSE
├─ README.md
├─ 发布与安装说明.md
└─ skills/
   └─ review-workflow/
      ├─ SKILL.md
      ├─ references/
      ├─ examples/
      └─ scripts/
```

## 设计原则

1. **不覆盖原项目**：本仓库是独立 skill 仓库，不直接修改原始综述工程。
2. **模板化复用**：仅提炼通用流程、模板、检查表与说明。
3. **GitHub 友好**：目录干净、文件职责明确，便于后续上传与维护。
4. **案例与模板分离**：案例项目只作为 examples 参考，不与 skill 主逻辑耦合。

## 核心文件

### 主 skill
- [skills/review-workflow/SKILL.md](skills/review-workflow/SKILL.md)

### 通用模板
- [skills/review-workflow/references/](skills/review-workflow/references/)

### 案例与提示词示例
- [skills/review-workflow/examples/](skills/review-workflow/examples/)

### 发布说明
- [发布与安装说明.md](发布与安装说明.md)

## 推荐使用方式

当你希望 Claude 帮你：
- 从零开始搭建综述项目
- 把已有文献整理成证据中台
- 生成提纲、初稿、修改稿
- 做引文编号化、审稿回复和 Word 成稿整理
- 把一次真实综述流程沉淀成模板化方法

就可以让 Claude 调用这个 skill。

## GitHub 上传前你需要知道的事

“初始化 git” 的意思是：
把当前文件夹变成一个 Git 仓库，之后才能方便地提交版本和推送到 GitHub。

最基本命令是：

```bash
git init
git add .
git commit -m "init review workflow skill"
```

更完整说明见：
- [发布与安装说明.md](发布与安装说明.md)

## 后续可扩展方向

- 把检索、证据抽取、Word 排版拆成多个子 skill
- 为不同学科增加专门的 references
- 增加与 CSV / BibTeX / JSON 的更强联动脚本
- 增加 skill eval 与触发词优化
- 后续把通用自动化脚本迁移到 `scripts/` 目录中
