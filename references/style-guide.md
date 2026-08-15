# 拙趣奶油插画风格指南 (Style Guide)

> 本文件是 naive-cream-illustration skill 的完整视觉规范。每次生成前必须读取本文件，将规范注入上下文后再组装提示词。

---

## 一、配色体系

### 底色

| 角色 | 色值 | 用途 |
|------|------|------|
| 纸白 | `#FAF7F2` | 全局背景底色，所有画面的"画纸" |
| 暖白 | `#F5F0E8` | 次级背景/卡片底/分区底 |

### 主点缀色（每次只选 1~2 个）

| 名称 | 色值 | 气质 |
|------|------|------|
| 橄榄绿 | `#6B7B5A` | 自然、植物、日常 |
| 陶土红 | `#C97D5D` | 温暖、食物、秋天 |
| 雾霾蓝 | `#7B8FA1` | 安静、清晨、冬天 |
| 奶油黄 | `#E8C766` | 明亮、快乐、柠檬 |
| 薄荷绿 | `#9DBFA0` | 清新、春天、轻盈 |

### 辅助色

| 角色 | 色值 | 用途 |
|------|------|------|
| 炭黑 | `#2B2B2B` | 轮廓线、文字、关键描边 |
| 浅灰 | `#D9D4CE` | 分割线、次要元素、阴影暗示 |
| 奶咖 | `#B8A090` | 中性过渡、小面积平衡 |

### 配色铁律

- **低饱和**：所有颜色饱和度 ≤ 35%，明度偏高，呈"奶油化"质感。
- **少即是多**：一张图最多 2 个点缀色 + 炭黑轮廓 + 纸白底，共 4~5 色封顶。
- **禁止**：高饱和原色（纯红/纯蓝/纯绿）、荧光色、撞色对比、复杂渐变。

---

## 二、质感与笔触

| 维度 | 规范 |
|------|------|
| 线条 | 铅笔草稿感、手绘颤抖线、粗细不均、可有断点；像"不太会画画的人认真画的" |
| 填色 | 平涂为主，不做写实光影、不做渐变、不做体积感塑造 |
| 纸纹 | 画面整体叠加轻微纸张噪点纹理（颗粒度 3~5%），增加手作感 |
| 边缘 | 色块边缘可以有轻微"涂出界"的感觉，不要太干净 |
| 整体气质 | 稚拙、儿童简笔画式、放松、不费力、治愈 |

### 禁止

- ❌ 写实渲染、3D 质感、光泽反射
- ❌ 精确对称、完美几何
- ❌ 复杂透视、空间纵深
- ❌ AI 味光滑插画（矢量扁平那种干净感）

---

## 三、构图与留白

| 维度 | 规范 |
|------|------|
| 画幅 | 固定 1:1 方形 |
| 留白 | 画面 80% 以上为纸白留白，主体只占 15~25% |
| 主体位置 | 居中或略偏左/右下方，四周大量透气空间 |
| 层级 | 单一主体为主；最多 2~3 个小元素点缀（如小星星、小植物、小圆点） |
| 地平线 | 可有可无；有则是一条手绘歪歪的短线，不贯穿画面 |
| 边框 | 不加画框，画面边缘自然结束 |

---

## 四、排版规范（带文字时启用）

### 中文手写体

- 风格：圆润、略歪、字距宽松、放松不对齐——像小学生写的字但更松弛
- 不用任何标准字体（宋体/黑体/楷体都不行）
- 提示词中描述为："handwritten Chinese characters, childlike, slightly wobbly, loose letter-spacing"

### 排版结构

| 层级 | 大小 | 位置 | 示例 |
|------|------|------|------|
| 标题大字 | 画面 8~12% 高度 | 主体上方或旁边 | "秋日奶茶" |
| 小字说明 | 画面 3~5% 高度 | 标题下方或角落 | "第一杯 · 温热的" |

### 排版铁律

- 文字与主体之间要有留白，不挤在一起
- 文字颜色用炭黑 `#2B2B2B` 或主点缀色
- 最多两行文字，不堆段落
- 中英文混排可以，但保持整体手写感统一

---

## 五、提示词模板

组装生图提示词时，按以下结构拼接：

```
[主题描述]

Style: naive cream illustration, childlike hand-drawn style, wobbly pencil lines,
flat colors on warm paper-white background (#FAF7F2), 80%+ whitespace,
minimal composition with small centered subject,
[主点缀色名称] accent color at low saturation,
paper grain texture overlay, no realistic lighting, no gradients,
simple and clumsy shapes like a beginner's drawing,
healing and relaxed atmosphere.

[文字要求（如有）: Add handwritten Chinese text "[文字内容]" in wobbly childlike style,
loose letter-spacing, placed near the subject with breathing space.]

Aspect ratio: 1:1, square format.
```

### 示例组装

**输入**：主题"秋天的第一杯奶茶"，带文字"秋日奶茶"，主色陶土红

**提示词**：
```
A cup of milk tea with a few autumn leaves floating nearby, simple and cozy.

Style: naive cream illustration, childlike hand-drawn style, wobbly pencil lines,
flat colors on warm paper-white background (#FAF7F2), 80%+ whitespace,
minimal composition with small centered subject,
terracotta red (#C97D5D) accent color at low saturation,
paper grain texture overlay, no realistic lighting, no gradients,
simple and clumsy shapes like a beginner's drawing,
healing and relaxed atmosphere.

Add handwritten Chinese text "秋日奶茶" in wobbly childlike style,
loose letter-spacing, placed near the cup with breathing space.

Aspect ratio: 1:1, square format.
```

---

## 六、生成后自检清单

- [ ] 留白是否 ≥ 80%？主体是否小而透气？
- [ ] 配色是否低饱和、奶油化？有没有跑出规定色板？
- [ ] 线条是否稚拙手绘感？有没有变光滑矢量风？
- [ ] 有没有不该出现的写实光影/渐变/3D 质感？
- [ ] 文字（如有）是否可读？中文是否花到无法辨认？
- [ ] 整体氛围是否松弛治愈？

任一项不过 → 调整提示词重生成一次；两次仍不行 → 放弃文字只保留插画，告知用户。

---

## 七、参考来源说明

本风格体系提炼自用户收藏的小红书参考图（喜茶"拙趣"品牌视觉 × yomsweethome 治愈系插画）的共同视觉语言。
**不复制任何原图**：不出现喜茶 Logo、不临摹 yomsweethome 或其他任何具体画面/构图/角色。只应用风格规则。
