# photo-skill 🎨

> OpenClaw AgentSkill 合集 — 两种插画风格生成器

## Skills

### 1. naive-cream-illustration — 拙趣奶油插画风

纸白大留白 × 低饱和奶油系配色 × 稚拙手绘 × 拙拙感手写排版。1:1 方形插画。

风格灵感来自喜茶"拙趣"品牌视觉 × yomsweethome 治愈系插画。

📁 [查看详情 →](naive-cream-illustration/)

**示例：**

![cream-sample](naive-cream-illustration/samples/autumn-milk-tea.jpg)

**触发词：** `喜茶风`、`奶油风`、`拙趣风`、`治愈插画`、`小红书那种感觉`

---

### 2. minimalist-healing-art — 极简治愈风景风

极致留白 × 低饱和雾感色块 × 微缩人影 × 平涂无光影 × 安静疏离氛围。3:4 竖版插画。

风格灵感来自 ohio_ooooo 治愈系插画 × Guim Tió Zarraluki 极简风景画。

📁 [查看详情 →](minimalist-healing-art/)

**示例：**

![minimal-sample](minimalist-healing-art/samples/seaside-dusk.png)

**触发词：** `极简风景`、`治愈风`、`空旷感`、`孤独美学`、`留白插画`、`色块风景`

---

## 快速开始

### 安装

```bash
cd ~/.openclaw/workspace/skills
git clone https://github.com/chensn05/photo-skill.git
```

然后将需要的 skill 目录移动到 skills 根目录：

```bash
# 安装拙趣奶油风
cp -r photo-skill/naive-cream-illustration .

# 安装极简治愈风
cp -r photo-skill/minimalist-healing-art .

# 或两个都装
cp -r photo-skill/naive-cream-illustration photo-skill/minimalist-healing-art .
```

### 配置图片生成后端

两个 skill 都需要一个图片生成工具作为后端。详见各 skill 目录下的 README 和 SKILL.md。

### 使用

在 OpenClaw 中直接对话触发：

```
# 拙趣奶油风
画一张秋天的第一杯奶茶，喜茶风

# 极简治愈风
画一张雪原独行，冷雾蓝色系，极简风景
```

## 风格对比

| 维度 | naive-cream-illustration | minimalist-healing-art |
|------|--------------------------|------------------------|
| 画幅 | 1:1 方形 | 3:4 竖版 |
| 留白 | 80%+ | 70%+ |
| 配色 | 低饱和奶油系（明亮温暖） | 低饱和雾感色块（灰雾克制） |
| 笔触 | 稚拙手绘、铅笔草稿线 | 平涂色块、无笔触 |
| 人物 | 不画人物或小元素点缀 | 微缩人影（背影/侧影） |
| 文字 | 可选拙拙感手写中文 | 默认不带 |
| 氛围 | 松弛、治愈、日常、不费力 | 安静、疏离、孤独但自洽 |
| 灵感来源 | 喜茶拙趣 × yomsweethome | ohio_ooooo × Guim Tió Zarraluki |

## License

MIT — 详见 [LICENSE](naive-cream-illustration/LICENSE)

## Contributing

欢迎提交 Issue 或 PR 来：
- 改进风格规范
- 添加新的点缀色系
- 贡献更多示例图
- 适配更多图片生成后端
- 添加新的插画风格 skill
