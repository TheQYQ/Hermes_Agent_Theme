# Hermes Agent Theme

> Hermes Agent 终端主题合集 — 像素艺术 × 宝可梦 × 一二布布，YAML 一键换肤。

## 简介

本项目为 [Hermes Agent](https://hermes-agent.nousresearch.com) 的终端配色主题集合。每个主题均以像素风 banner 为视觉核心，搭配精心调配的 UI 配色（状态栏、补全菜单、diff、语法高亮等），让命令行工作也能拥有个性。

## 主题列表

### 宝可梦系列

| 主题 | 灵感 | 色调 | 亮点 |
|------|------|------|------|
| **kanto-team** | 初代宝可梦梦之队 | 暖金 + 深灰 | 小智/皮卡丘/喷火龙/水箭龟/妙蛙花/卡比兽全员像素 banner，加载语 "POKEDEX LOADING" 等 7 条 |
| **gengar-shadow** | 耿鬼 | 深紫 | 幽灵系紫色终端，拼豆图纸 1:1 还原的像素耿鬼 |
| **groudon-terra** | 固拉多 | 熔岩红 | 地面系红色终端，像素固拉多 |
| **kyogre-tide** | 盖欧卡 | 深海蓝 | 水系蓝色终端，像素盖欧卡 |
| **pikachu-volt** | 皮卡丘 | 暖黄 + 深底 | 电系黄色终端，像素皮卡丘 |
| **rayquaza-sky** | 烈空坐 | 墨绿 | 龙系绿色终端，像素烈空坐 |

### 一二布布系列

| 主题 | 场景 | 色调 | 亮点 |
|------|------|------|------|
| **bubu-yier** | 雨夜共毯 | 雨夜蓝 | 两只小熊共撑一条蓝色毯子躲雨，毯子上还有小花 |
| **bubu-beach** | 海滩度假 | 海洋蓝 | 一二戴海鸥、布布顶海鸥，沙滩度假名场面 |
| **bubu-sunset** | 日落海滩 | 暖橙 + 暮色 | 并肩看日落，小螃蟹列队路过，海鸥站岗 |
| **bubu-wave** | 踏浪合影 | 浪蓝 + 沙金 | 海浪沙滩正面合影，粉腮红特写，海鸥群护航 |

## 主题文件结构

每个 YAML 文件定义：

- `name` — 主题标识
- `description` — 主题描述
- `colors` — 全量 UI 配色（背景、banner、状态栏、补全菜单、diff、语法高亮、voice/session 区域等）
- `spinner` — 加载动画（thinking faces/verbs、waiting faces、wings）
- `branding` — 品牌信息（agent_name、goodbye 语句、welcome 横幅等）
- `banner_logo` / `banner_hero` — 像素画横幅（Rich markup，半块字符渲染）

## 使用方式

1. 安装 Hermes Agent（[文档](https://hermes-agent.nousresearch.com/docs)）。
2. 将任一主题 YAML 复制到 Hermes 皮肤目录：
   ```bash
   # Windows
   cp bubu-wave.yaml "$env:LOCALAPPDATA\hermes\skins\"

   # Linux / macOS
   cp bubu-wave.yaml ~/.hermes/skins/
   ```
3. 在 `config.yaml` 中启用：
   ```yaml
   display:
     skin: bubu-wave
   ```
4. 重启 Hermes 会话即可看到像素 banner。

## 文件说明

```
.
├── LICENSE               MIT 许可证
├── .gitignore            忽略规则（系统/编辑器临时文件）
├── README.md             本文件
├── kanto-team.yaml       初代梦之队主题
├── gengar-shadow.yaml    耿鬼紫主题
├── groudon-terra.yaml    固拉多红主题
├── kyogre-tide.yaml      盖欧卡蓝主题
├── pikachu-volt.yaml     皮卡丘黄主题
├── rayquaza-sky.yaml     烈空坐绿主题
├── bubu-yier.yaml        一二布布 · 雨夜共毯
├── bubu-beach.yaml       一二布布 · 海滩度假
├── bubu-sunset.yaml      一二布布 · 日落海滩
└── bubu-wave.yaml        一二布布 · 踏浪合影
```

## License

[MIT](LICENSE) — 可自由使用、修改与二次分发，保留版权声明即可。

主题中的宝可梦角色名称与形象归 The Pokémon Company / Nintendo 等权利人所有，仅作个人粉丝创作与配色示意；一二布布系列同理由原作者持有形象版权。
