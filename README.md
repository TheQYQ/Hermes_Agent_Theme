# Hermes Agent Theme

> Hermes Agent 终端主题合集 — 像素艺术 × 宝可梦 × 可爱小动物，YAML 一键换肤。

## 简介

本项目为 [Hermes Agent](https://hermes-agent.nousresearch.com) 的终端配色主题集合。每个主题均以像素风 banner 为视觉核心，搭配精心调配的 UI 配色（状态栏、补全菜单、diff、语法高亮等），让命令行工作也能拥有个性。

## 主题列表

| 主题 | 灵感 | 色调 | 亮点 |
|------|------|------|------|
| **kanto-team** | 初代宝可梦梦之队 | 暖金 + 深灰 | 皮卡丘/喷火龙/水箭龟等像素角色，加载语："POKEDEX LOADING" 等 7 条 |
| **gengar-shadow** | 耿鬼 | 深紫 | 幽灵系紫色终端，像素耿鬼 banner |
| **groudon-terra** | 固拉多 | 熔岩红 | 地面系红色终端，像素固拉多 |
| **kyogre-tide** | 盖欧卡 | 深海蓝 | 水系蓝色终端，像素盖欧卡 |
| **pikachu-volt** | 皮卡丘 | 暖黄 + 深底 | 电系黄色终端，像素皮卡丘 |
| **rayquaza-sky** | 烈空坐 | 墨绿 | 龙系绿色终端，像素烈空坐 |
| **bubu-dudu** | 小熊 × 小熊 | 雨夜蓝 | 两只小熊共撑一条蓝色毯子的温馨场景 |

## 主题文件结构

每个 YAML 文件定义：

- `name` — 主题标识
- `description` — 主题描述
- `colors` — 全量 UI 配色（背景、banner、状态栏、补全菜单、diff、语法高亮、voice/session 区域等）
- `spinner` — 加载动画（thinking faces/verbs、waiting faces、wings）
- `branding` — 品牌信息（agent_name、goodbye 语句等）

## 使用方式

1. 安装 Hermes Agent（[文档](https://hermes-agent.nousresearch.com/docs)）。
2. 将任一主题 YAML 复制到 Hermes 主题目录：
   ```bash
   cp kanto-team.yaml ~/.hermes/themes/
   ```
3. 在 Hermes 配置中启用该主题（参考官方文档的 Theme 配置部分）。

## 文件说明

```
.
├── README.md             本文件
├── kanto-team.yaml       初代梦之队主题
├── gengar-shadow.yaml    耿鬼紫主题
├── groudon-terra.yaml    固拉多红主题
├── kyogre-tide.yaml      盖欧卡蓝主题
├── pikachu-volt.yaml     皮卡丘黄主题
├── rayquaza-sky.yaml     烈空坐绿主题
└── bubu-dudu.yaml        小熊温馨主题
```

## License

个人创作，可自由使用与二次定制。
