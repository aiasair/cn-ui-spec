# 汉界规则 · cn-ui-spec

一套独立的中文网站与应用 UI/UX 规则，以及可离线打开的 HTML 交互演示。适用于企业 SaaS、管理后台、AI 工作台、知识库、内容平台和移动应用。

[阅读技能规则](SKILL.md) · [HTML 演示文件](demo/index.html)

## 三条核心约束

- **统一字号**：桌面业务 UI 默认 14/22px，连续阅读默认 16/26px；12px 仅限低优先级辅助信息。
- **克制说明**：标题、菜单、按钮、区块不惯例性搭配解释小字。删除后不会损失必要信息的说明，应当删除。
- **统一间距**：区分文字行高、额外段距、元素间距和组件高度，使用统一的语义设计变量。

完整体系还覆盖视觉主题、组件状态、表单表格、中文格式、响应式、无障碍和 AI 产品流程。规则不绑定特定组件库或预设品牌色；示例配色也不构成所有中文界面的强制风格。

## 规则目录

| 领域 | 文件 |
| --- | --- |
| 技能入口、执行等级和适用边界 | [SKILL.md](SKILL.md) |
| 字号、字重、字体与可读性 | [typography.md](references/typography.md) |
| 克制界面说明 | [interface-copy.md](references/interface-copy.md) |
| 行高、段距、元素间距与组件高度 | [spacing.md](references/spacing.md) |
| 布局、语义色、主题、图标与动效 | [visual-system.md](references/visual-system.md) |
| 交互状态、反馈、表单与表格 | [interaction.md](references/interaction.md) |
| 中文格式、响应式与无障碍 | [localization-accessibility.md](references/localization-accessibility.md) |
| AI 产品流程与工程验收 | [ai-development.md](references/ai-development.md) |

## 在 Codex 中使用

将本仓库放入个人技能目录的 `cn-ui-spec` 文件夹，例如：

```bash
git clone https://github.com/aiasair/cn-ui-spec.git ~/.codex/skills/cn-ui-spec
```

如果目标目录已经存在，先保留现有内容，再根据自己的目录管理方式合并或更新。

在支持 Skills 的 Codex 会话中调用：

```text
请使用 $cn-ui-spec 检查并改进当前中文界面。
```

技能按任务领域读取参考文件；不因启用规则而自动授权全站重构、迁移技术栈或执行外部操作。

## 打开 HTML 演示

下载或克隆仓库后，用浏览器打开 `demo/index.html`。演示是单个 HTML 文件，无需安装依赖或连接外部服务。GitHub 的文件预览展示源码，交互需要在浏览器中打开下载后的 HTML。

演示包含七个章节，可切换黑白、蓝、绿、橙、紫、红配色，以及浅色、深色和文字放大模式。行高与间距章节提供四种可调测量：文字行高、段落额外间距、标题前后距离和组件高度，并有三档行高对比。

表单可保存到当前浏览器；AI 流程为本地模拟，不调用模型或外部工具。

## 维护约定

新增通用规则须先明确具体条款、适用范围与影响，经用户同意后纳入。项目局部例外不自动成为汉界通用规则；修改时保留必要的验证记录，未运行的检查不得声称通过。
