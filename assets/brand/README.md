# huasan brand assets

> 跨 `huasanai/*` 仓库复用的品牌资产。形状固定，颜色和背景可换。

## 当前资产

| 文件 | 含义 | 视觉 |
|---|---|---|
| [`umbrella.svg`](./umbrella.svg) | 主品牌符号——抽象的伞（呼应"画伞"名字本义）。一笔画出的 stroke 动画 + 五根伞骨 + 浮动呼吸 | viewBox `0 0 250 220`，透明背景 |

## 设计原则

这套资产遵循 [animated-logo.md 里的"内容设计 ≠ 品牌设计"原则](https://github.com/huasanai/huasan-skills/blob/main/README.md)——**永不绑定具体内容**（不含 skill 数量 / 版本号 / 产品列表）。形状一旦定型，就只是颜色和背景可以换。

## 怎么用

### 用法 1：直接引用文件

```markdown
<img src="https://raw.githubusercontent.com/huasanai/huasan-skills/main/assets/brand/umbrella.svg" width="250">
```

或者把文件 copy 到你新 repo 的 `assets/brand/` 下后本地引用：

```markdown
<img src="./assets/brand/umbrella.svg" width="250">
```

### 用法 2：嵌入更大的 composite logo

如果你要做一个完整的 banner logo（左符号 + 右文字 + tagline），打开 `umbrella.svg` 把 `<g class="umb-group">` 整段 copy 到你的大 logo 的 SVG 里。注意：

- umbrella 的几何坐标基于 viewBox `0 0 250 220`
- 嵌入大 viewBox（如 `0 0 1200 380`）时，需要给所有点加上 offset
- 当前 `huasan-skills/assets/logo.svg` 就是这么做的（伞在 x=200-430、y=80-275）

参考嵌入坐标偏移：
```
dx = target_x_origin - 0
dy = target_y_origin - 0
```

## 换颜色

打开 `umbrella.svg`，搜索替换两个核心颜色：

| 当前 | 含义 | 备选调色 |
|---|---|---|
| `#00ff41` | 主笔（matrix 绿）| `#ff9f29`（暖橙）/ `#818cf8`（薰衣草）/ `#ffffff`（纯白）|
| `#5dd4f5` | 副笔 + 渐变末端 + 伞骨（青蓝）| `#ffd166`（金）/ `#c4b5fd`（淡紫）/ `#aaaaaa`（中性灰）|

具体替换位置（文件里清晰标注在顶部注释里）：

- `linearGradient` 的两个 `stop-color`
- canopy `underside` 弧线的 `stroke`
- ribs 的 `stroke`
- tip `circle` 的 `fill`

## 换背景

`umbrella.svg` **默认透明背景**。在嵌入大 logo 时由 host 提供背景：

```svg
<svg viewBox="0 0 1200 380">
  <!-- 你的背景 -->
  <rect width="1200" height="380" fill="url(#yourBackground)"/>
  
  <!-- 嵌入伞 -->
  <g transform="translate(200, 80)">
    <!-- paste umbrella geometry here, or use <image> -->
  </g>
  
  <!-- 你的文字 / 其他元素 -->
</svg>
```

## 几何锚点（嵌入参考）

| 锚点 | 坐标（umbrella.svg 内部）|
|---|---|
| Canopy 起点（左边缘）| (10, 114) |
| Canopy 终点（右边缘）| (240, 114) |
| Tip（最高点）| (125, 14) |
| 中心（中心 rib 起点）| (125, 19) |
| Shaft 起点 | (125, 92) |
| Shaft 终点 / Handle 起点 | (125, 182) |
| Handle 末端 | (100, 206) |

伞的总尺寸：**230 × 192**（不含 padding）

## 来源

第一次出现：[huasan-skills v0.2 logo](../logo.svg)（2026-05-14）

设计动机：v0.1 logo 硬编码了 11 个 skill chip + 5 类别色，每加 skill 都要重画。v0.2 抽象为符号 + 文字 + 稳定 tagline，无论 skill 增减都不需要修改。

伞符号选择理由：
- "画伞"名字两个字一同视觉化——"画"（drawn / stroke 动画）+ "伞"（umbrella / shelter）
- 隐喻：在 AI 信息洪流中，画伞作为撑伞的人——shelter, then ship
- 几何极简，跨尺寸（favicon → banner）都能 work
