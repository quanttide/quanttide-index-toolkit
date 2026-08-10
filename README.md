# 量潮索引库（quanttide-index-toolkit）

> 统一入口（index）——方便人和 AI 从这里直接找到所有可用的库。

## 定位

quanttide-index 是量潮工具库体系的**入口库**：

- 继承 quanttide-base-toolkit 的历史（git 历史延续），但**推翻重写**
- 提供**入口功能**：从这一个库可以找到所有可用的工具库
- 以 `quanttide` 名义发布（v0.2.0 起），quanttide-* 各库作为可选插件

**重要性质**：本库不提供任何实际功能，**可以随时拆掉**——入口库的存在不构成系统依赖。

## 为什么这样设计

1. **统一入口**：人和 AI 从一个入口找到所有库，降低发现成本
2. **去中心化**：入口库只维护一个基本不动、不会错的入口功能，最大限度稳定
3. **可拆除**：不提供实际功能 → 不对系统形成单点依赖

## 与相关仓库的关系

- **quanttide-meta-toolkit**：元领域——提供标准字段/模型（storage/fields），是核心治理层
- **quanttide-toolkit**：元仓库——挂载各领域 toolkit
- **quanttide-index-toolkit**：入口库（本仓库）——继承 base 历史，推翻重写为入口

## 来源

本仓库由 quanttide-base-toolkit 改名而来（2026-08-09）。原 storage/fields 内容已迁至 quanttide-meta-toolkit，本仓库推翻重写为入口库。
