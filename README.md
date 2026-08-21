# Adaptive Liquid Glass UI

一个可复用的界面设计 Skill（设计工作协议），用于构建克制、内容优先、能适应背景与品牌色的 Liquid Glass UI。

## What this skill is for

- 评估玻璃材质是否真的服务信息层级
- 根据背景、品牌色、明暗模式推导材质 Token
- 设计导航、卡片、控件、弹层的材料层级
- 补齐 hover、focus-visible、pressed、disabled 与 reduced-transparency 状态
- 检查移动端、可读性、键盘可达性与降级方案

## Package

完整指令位于 [adaptive-liquid-glass-ui/SKILL.md](adaptive-liquid-glass-ui/SKILL.md)。

它包含：

- Host context（背景上下文）分类
- Adaptive tokens（自适应 Token）推导
- Material hierarchy（材质层级）
- Interaction and accessibility states（交互与无障碍状态）
- Anti-patterns（反模式）
- 交付前视觉与响应式检查清单

## Design stance

玻璃不是默认视觉主题，而是一种与背景、内容、光线和交互状态的关系。内容优先，透明度克制；当 blur 或透明效果不可用时，界面仍然需要清晰、稳定并保持同一设计系统。
