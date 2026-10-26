# Adaptive Liquid Glass UI

面向 Codex 的界面设计 Skill：根据背景、品牌色和内容层级，构建克制、可读、具备降级方案的 Liquid Glass UI。

[阅读 Skill](adaptive-liquid-glass-ui/SKILL.md) · [材质与 Token 参考](adaptive-liquid-glass-ui/references/adaptive-liquid-glass.md)

## 适合解决什么问题

- 判断导航、卡片、控件与弹层是否适合使用玻璃材质。
- 为明暗模式、品牌色和图片背景推导不同的材质 Token。
- 区分材质层级，避免所有内容变成相同的半透明卡片。
- 补齐 hover、focus-visible、pressed、disabled 等状态。
- 检查移动端、键盘可达性、对比度和 reduced-transparency 降级。

## 如何使用

这是设计工作协议与参考资料，不是组件库、应用或 npm 包。

1. 打开 [`adaptive-liquid-glass-ui/SKILL.md`](adaptive-liquid-glass-ui/SKILL.md)，将其作为设计或前端改造任务的工作指引。
2. 提供现有界面、品牌色、目标尺寸与交互要求，先检查宿主背景和信息层级。
3. 按流程推导 Token、分配材质角色，再实现交互与无障碍状态。
4. 在深色、浅色和至少一种品牌色或图片背景上验证，同时检查移动端与无透明效果的回退。

## 工作流程

```text
检查宿主界面 → 分类背景 → 推导 Token → 构建材质层 → 匹配 UI 角色 → 补齐状态 → 验证
```

| 内容 | 入口 |
| --- | --- |
| 工作协议、反模式与交付检查 | [SKILL.md](adaptive-liquid-glass-ui/SKILL.md) |
| 自适应 Token、CSS 材质结构与上下文示例 | [参考文档](adaptive-liquid-glass-ui/references/adaptive-liquid-glass.md) |

## 设计取舍

内容优先，透明度克制。长文和密集表格通常应保持不透明；重要控件不能只靠背景模糊来保证可读性。

玻璃效果需要随宿主背景变化，而非固定使用一层蓝灰色。关闭 blur 或透明效果后，界面仍应清晰、稳定，并属于同一套设计系统。

## 使用边界

Skill 提供设计方法和检查项，不保证自动满足无障碍标准，也不将 CSS 背景模糊描述为真实光学折射。采用材质行为时，应保留自身品牌、布局与素材，不复制 Apple 的专有界面或资源。
