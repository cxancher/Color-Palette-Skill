# 🎨 Color Palette Skill - 配色大师

<p align="center">
  <a href="#english"><img src="https://img.shields.io/badge/English-blue" alt="English"></a>
  <a href="#中文"><img src="https://img.shields.io/badge/中文-red" alt="中文"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/palettes-1052+-blue" alt="1052+ Palettes">
  <img src="https://img.shields.io/badge/categories-18-green" alt="18 Categories">
  <img src="https://img.shields.io/badge/countries-50+-orange" alt="50+ Countries">
  <img src="https://img.shields.io/badge/industries-100+-red" alt="100+ Industries">
  <img src="https://img.shields.io/badge/tech_stacks-40+-purple" alt="40+ Tech Stacks">
  <img src="https://img.shields.io/badge/version-3.0.0-9cf" alt="v3.0.0">
  <img src="https://img.shields.io/badge/license-MIT-yellow" alt="MIT License">
</p>

---

<a id="english"></a>

## 📖 About | [中文](#中文)

**Color Palette Skill** is an AI-driven color palette library designed to eliminate the "default blue-purple gradient" problem in AI-generated frontends. With **1052+ curated palettes**, it covers:

- 🌏 **50+ countries** — China, Japan, Korea, India, Brazil, Russia, Germany, France, UK, US, SEA, Middle East, Africa, LatAm
- 🏭 **100+ industries** — Finance, Healthcare, Education, Gaming, AI, Web3, Aviation, Luxury, FMCG, and more
- 🖥️ **40+ tech stacks** — React, Vue, Angular, Svelte, Flutter, SwiftUI, Jetpack Compose, Tailwind, shadcn/ui
- 🎨 **30+ design styles** — Minimalist, Cyberpunk, Nordic, Japanese, Art Deco, Bauhaus, Glassmorphism, Brutalism
- 🎮 **Gaming & Web3** — Steam, PlayStation, Bitcoin, Ethereum, OpenSea, Discord, Twitch
- 🤖 **AI Platforms** — OpenAI, Anthropic, Hugging Face, Midjourney, Cursor, Vercel AI

### 🎯 Problem Solved

AI defaults to blue-purple gradients (`#667eea → #764ba2`) for every project. This library provides:

- ✅ Context-aware palette matching by project type, industry, and emotion
- ✅ Real brand colors from 200+ successful products
- ✅ Dark mode support for every palette
- ✅ Ready-to-use CSS Variables, Tailwind CSS, SCSS, and Design Tokens
- ✅ WCAG AA contrast compliance

---

## 🗂️ Categories

| # | Category | Count | Highlights |
|---|----------|-------|-----------|
| 1 | 🇨🇳 China Platforms | 12 | Taobao, Douyin, WeChat, Bilibili, Meituan, JD, PDD |
| 2 | 🌏 Asia Platforms | 40 | LINE, NAVER, Kakao, Coupang, Flipkart, Swiggy, Grab, Shopee |
| 3 | 🌍 Western Platforms | 41 | Google, Apple, Meta, Amazon, Netflix, Spotify, Slack, Notion, Figma |
| 4 | 🌐 Global Brands | 62 | Nike, Samsung, BMW, Tesla, Starbucks, IKEA, Lego, Coca-Cola |
| 5 | 🖥️ Dev Frameworks | 40 | React, Vue, Angular, Svelte, Next.js, Nuxt, Remix, Astro, Three.js |
| 6 | 🏭 Global Industries | 116 | Finance, Healthcare, Aviation, Hospitality, Telecom, Luxury, FMCG |
| 7 | 🎨 Design Styles | 31 | Minimalist, Cyberpunk, Nordic, Art Deco, Bauhaus, Glassmorphism |
| 8 | 🌍 Cultural Palettes | 31 | Japan, Korea, India, Brazil, Russia, Germany, France, UK, Africa |
| 9 | 💭 Emotion Palettes | 53 | Trust, Energy, Calm, Passion, Innovation, Luxury, Playful |
| 10 | 🏢 Industry Extra | 12 | Legal, Fitness, Gaming, Pet, Logistics, Agriculture, Insurance |
| 11 | 🎭 Style Palettes | 10 | Retro, Cyberpunk, Nordic, Japanese, Dark Luxury, Bohemian |
| 12 | 🌈 Color Extra | 8 | Teal, Brown, Gold, Coral, Mint, Lavender, Indigo, Salmon |
| 13 | 📝 WordPress Themes | 3 | Flavor, Avada, Enfold |
| 14 | 🎨 Design Systems | 5 | Material, Ant Design, Fluent, HIG, Carbon |
| 15 | 📦 Extra Palettes | 140 | 27 WP themes, 15 UI systems, 40 tech industries, 20 styles, 30 colors |
| 16 | 🚀 Batch 3 | 430 | Regional (60), CMS (50), UI Kits (40), Gaming (30), Web3 (30), AI (30), + more |

---

## 🚀 Quick Start

### 1. Read Palette Data

```json
{
  "id": "taobao",
  "name": "淘宝",
  "category": "china-platform",
  "tags": ["电商", "购物", "橙色"],
  "colors": {
    "primary": "#FF5000",
    "secondary": "#FF4400",
    "accent": "#FF0036",
    "background": "#F5F5F5",
    "surface": "#FFFFFF",
    "text": "#333333"
  },
  "darkMode": { "background": "#1A1A1A", "surface": "#2A2A2A", "text": "#E5E5E5" },
  "cssVariables": ":root { --color-primary: #FF5000; ... }",
  "tailwindConfig": "module.exports = { theme: { extend: { colors: { ... } } } }"
}
```

### 2. CSS Variables

```css
:root {
  --color-primary: #FF5000;
  --color-secondary: #FF4400;
  --color-accent: #FF0036;
  --color-background: #F5F5F5;
  --color-surface: #FFFFFF;
  --color-text: #333333;
}

[data-theme="dark"] {
  --color-background: #1A1A1A;
  --color-surface: #2A2A2A;
  --color-text: #E5E5E5;
}
```

### 3. Tailwind CSS

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: '#FF5000',
        secondary: '#FF4400',
        accent: '#FF0036',
      }
    }
  }
}
```

---

## 🧠 Smart Recommendation

### By Project Type

| Type | Recommended | Primary Color |
|------|------------|---------------|
| E-commerce | Taobao / Shopee / Rakuten | `#FF5000` Orange |
| Social App | WeChat / LINE / Discord | `#07C160` Green |
| Enterprise | Ant Design / IBM Carbon | `#1677FF` Blue |
| SaaS Product | Linear / Vercel / Stripe | `#5E6AD2` Indigo |
| Short Video | Douyin / TikTok / YouTube | `#FE2C55` Magenta |
| Food/Delivery | Meituan / Swiggy / iFood | `#FFC300` Yellow |
| Finance | Alipay / Nubank / Wise | `#1E40AF` Navy |
| AI/ML Tool | OpenAI / Cursor / HuggingFace | `#10A37F` Teal |
| Crypto/Web3 | Bitcoin / Ethereum / Solana | Brand-specific |
| Gaming | Steam / PlayStation / Valorant | Neon Cyberpunk |
| Healthcare | HealthTech / Zocdoc | `#0EA5E9` Sky Blue |
| Education | EdTech / BYJU'S / Duolingo | `#0284C7` Blue |
| Luxury | Black & Gold / Art Deco | `#000000` + `#D4AF37` |
| Kids/Children | Pastel / Macaron | `#B2DFDB` Mint |
| Eco/Green | GreenTech / Solarpunk | `#059669` Green |

### By Emotion

| Emotion | Colors | Examples |
|---------|--------|---------|
| 🔴 Energy & Passion | Red, Orange | Taobao, Netflix, YouTube |
| 🔵 Trust & Professional | Blue | LinkedIn, IBM, Banks |
| 🟣 Innovation & Tech | Purple, Cyan | Figma, Twitch, AI platforms |
| 🟢 Calm & Serene | Light Blue, Mint | Healthcare, Meditation |
| ⬛ Luxury & Premium | Black, Gold | Chanel, Dark Luxury |
| 🩷 Playful & Fun | Pink, Yellow | TikTok, Snapchat, Duolingo |
| 🟤 Warm & Cozy | Orange, Brown | Coffee shops, Bakeries |
| ⬜ Minimal & Clean | White, Gray | Apple, Notion, Muji |

---

## 📂 Project Structure

```
color-palette-skill/
├── README.md                           # This file (中英双语)
├── skill.md                            # Core skill instructions (English)
├── skill_CN.md                         # 核心技能指令（中文版）
├── color-palette-handbook.md           # Complete reference manual
└── data/
    ├── china-platforms.json            # 🇨🇳 12 Chinese platforms
    ├── asia-platforms.json             # 🌏 40 Asian platforms
    ├── western-platforms.json          # 🌍 41 Western platforms
    ├── global-brands.json              # 🌐 62 Global brands
    ├── dev-frameworks.json             # 🖥️ 40 Dev frameworks
    ├── global-industries.json          # 🏭 116 Global industries
    ├── design-styles.json              # 🎨 31 Design styles
    ├── cultural-palettes.json          # 🌍 31 Cultural palettes
    ├── emotion-palettes.json           # 💭 53 Emotion palettes
    ├── industry-palettes-extra.json    # 🏢 12 Extended industries
    ├── style-palettes.json             # 🎭 10 Design styles
    ├── color-palettes-extra.json       # 🌈 8 Color families
    ├── wordpress-themes.json           # 📝 3 WordPress themes
    ├── design-systems.json             # 🎨 5 Design systems
    ├── extra-palettes.json             # 📦 140 Supplementary palettes
    └── batch3-palettes.json            # 🚀 430 Major expansion
```

---

## 🚫 Color Taboos

### ❌ Never

- Default to blue-purple gradients (`#667eea → #764ba2`)
- Use the same palette for every project
- Ignore industry characteristics
- Use contrast ratios below WCAG AA (4.5:1)

### ✅ Always

- Match palette to project context
- Maintain clear color hierarchy
- Provide dark mode support
- Reference successful products
- Use semantic color tokens

---

## 🤝 Contributing

Contributions welcome! Please follow these standards:

1. Complete `colors` object (primary, secondary, accent, background, surface, text)
2. Provide `darkMode` values
3. Include `cssVariables` and `tailwindConfig` snippets
4. Ensure WCAG AA contrast (4.5:1)
5. Use standard 6-digit HEX format

---

## 📜 Changelog

### v3.0.0 (2026-05-08)

**Major expansion: 68 → 1052+ palettes**

- 🌏 +40 Asian platforms (Japan, Korea, India, SEA)
- 🌍 +41 Western platforms (Google, Apple, Meta, Amazon, etc.)
- 🌐 +62 Global brands (Nike, Samsung, BMW, Starbucks, etc.)
- 🖥️ +40 Dev frameworks (React, Vue, Svelte, Next.js, etc.)
- 🏭 +116 Global industries (Aviation, Hospitality, Telecom, Luxury, etc.)
- 🎨 +31 Design styles (Glassmorphism, Brutalism, Art Deco, etc.)
- 🌍 +31 Cultural palettes (50+ countries)
- 💭 +53 Emotion palettes
- 📦 +140 Extra palettes (WP, CMS, UI kits, tech industries)
- 🚀 +430 Batch 3 (Regional, CMS, Gaming, Web3, AI, more industries/styles/colors)
- 📝 GitHub-style skill.md with badges, TOC, structured sections
- 🇨🇳 Added skill_CN.md (Chinese version)

### v2.0.0 (2026-05-05)

- +30 palettes (total 68)
- New categories: industry-extra, style, color-palette-extra
- Fixed color distribution imbalance

### v1.0.0 (2026-05-05)

- Initial release: 38 palettes, 5 categories

---

## 📄 License

[MIT](LICENSE) — Free to use in any project.

---

<p align="center">
  <sub>Built with ❤️ to help AI break free from blue-purple gradients.</sub>
</p>

---
---

<a id="中文"></a>

## 📖 简介 | [English](#english)

**Color Palette Skill（配色大师）** 是一款专为 AI 前端开发设计的配色技能库。拥有 **1052+ 套精选配色方案**，覆盖：

- 🌏 **50+ 国家/地区** — 中国、日本、韩国、印度、巴西、俄罗斯、德国、法国、英国、美国、东南亚、中东、非洲、拉美
- 🏭 **100+ 行业** — 金融、医疗、教育、游戏、AI、Web3、航空、奢侈品、快消等
- 🖥️ **40+ 技术栈** — React、Vue、Angular、Svelte、Flutter、SwiftUI、Jetpack Compose、Tailwind、shadcn/ui
- 🎨 **30+ 设计风格** — 极简、赛博朋克、北欧、日式、装饰艺术、包豪斯、玻璃拟态、粗野主义
- 🎮 **游戏与 Web3** — Steam、PlayStation、Bitcoin、Ethereum、OpenSea、Discord、Twitch
- 🤖 **AI 平台** — OpenAI、Anthropic、Hugging Face、Midjourney、Cursor、Vercel AI

### 🎯 解决什么问题？

AI 在开发前端时，往往默认使用蓝紫色渐变（`#667eea → #764ba2`），导致所有项目千篇一律。本技能库提供：

- ✅ 根据项目类型、行业、情感智能匹配配色
- ✅ 200+ 成功产品的真实品牌色值
- ✅ 每套方案均提供深色模式支持
- ✅ 即用型 CSS 变量、Tailwind CSS、SCSS、Design Tokens
- ✅ 符合 WCAG AA 对比度标准

---

## 🗂️ 配色分类

| # | 分类 | 数量 | 代表方案 |
|---|------|------|----------|
| 1 | 🇨🇳 国内平台 | 12 | 淘宝、抖音、微信、B站、美团、京东、拼多多 |
| 2 | 🌏 亚洲平台 | 40 | LINE、NAVER、Kakao、Coupang、Flipkart、Swiggy、Grab、Shopee |
| 3 | 🌍 西方平台 | 41 | Google、Apple、Meta、Amazon、Netflix、Spotify、Slack、Notion、Figma |
| 4 | 🌐 全球品牌 | 62 | Nike、Samsung、BMW、Tesla、Starbucks、IKEA、Lego、Coca-Cola |
| 5 | 🖥️ 开发框架 | 40 | React、Vue、Angular、Svelte、Next.js、Nuxt、Remix、Astro、Three.js |
| 6 | 🏭 全球行业 | 116 | 金融、医疗、航空、酒店、电信、奢侈品、快消 |
| 7 | 🎨 设计风格 | 31 | 极简、赛博朋克、北欧、装饰艺术、包豪斯、玻璃拟态 |
| 8 | 🌍 文化配色 | 31 | 日本、韩国、印度、巴西、俄罗斯、德国、法国、英国、非洲 |
| 9 | 💭 情感配色 | 53 | 信任、活力、平静、热情、创新、奢华、俏皮 |
| 10 | 🏢 扩展行业 | 12 | 法律、健身、游戏、宠物、物流、农业、保险 |
| 11 | 🎭 风格配色 | 10 | 复古、赛博朋克、北欧、日式、暗黑奢华、波西米亚 |
| 12 | 🌈 色系补充 | 8 | 青色、棕色、金色、珊瑚、薄荷、薰衣草、靛蓝、鲑鱼粉 |
| 13 | 📝 WordPress 主题 | 3 | Flavor、Avada、Enfold |
| 14 | 🎨 设计系统 | 5 | Material、Ant Design、Fluent、HIG、Carbon |
| 15 | 📦 扩展配色 | 140 | 27 WP主题、15 UI系统、40科技行业、20风格、30色系 |
| 16 | 🚀 批量扩展 | 430 | 区域平台(60)、CMS模板(50)、UI组件(40)、游戏(30)、Web3(30)、AI(30) 等 |

---

## 🚀 快速开始

### 1. 读取配色数据

```json
{
  "id": "taobao",
  "name": "淘宝",
  "category": "china-platform",
  "tags": ["电商", "购物", "橙色"],
  "colors": {
    "primary": "#FF5000",
    "secondary": "#FF4400",
    "accent": "#FF0036",
    "background": "#F5F5F5",
    "surface": "#FFFFFF",
    "text": "#333333"
  },
  "darkMode": { "background": "#1A1A1A", "surface": "#2A2A2A", "text": "#E5E5E5" },
  "cssVariables": ":root { --color-primary: #FF5000; ... }",
  "tailwindConfig": "module.exports = { theme: { extend: { colors: { ... } } } }"
}
```

### 2. CSS 变量

```css
:root {
  --color-primary: #FF5000;
  --color-secondary: #FF4400;
  --color-accent: #FF0036;
  --color-background: #F5F5F5;
  --color-surface: #FFFFFF;
  --color-text: #333333;
}

[data-theme="dark"] {
  --color-background: #1A1A1A;
  --color-surface: #2A2A2A;
  --color-text: #E5E5E5;
}
```

### 3. Tailwind CSS

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: '#FF5000',
        secondary: '#FF4400',
        accent: '#FF0036',
      }
    }
  }
}
```

---

## 🧠 智能推荐

### 按项目类型

| 类型 | 推荐配色 | 主色 |
|------|---------|------|
| 电商网站 | 淘宝 / Shopee / 乐天 | `#FF5000` 橙色 |
| 社交应用 | 微信 / LINE / Discord | `#07C160` 绿色 |
| 企业官网 | Ant Design / IBM Carbon | `#1677FF` 蓝色 |
| SaaS 产品 | Linear / Vercel / Stripe | `#5E6AD2` 靛蓝 |
| 短视频 | 抖音 / TikTok / YouTube | `#FE2C55` 品红 |
| 美食/外卖 | 美团 / Swiggy / iFood | `#FFC300` 黄色 |
| 金融/支付 | 支付宝 / Nubank / Wise | `#1E40AF` 深蓝 |
| AI/ML 工具 | OpenAI / Cursor / HuggingFace | `#10A37F` 青绿 |
| 加密/Web3 | Bitcoin / Ethereum / Solana | 品牌专属色 |
| 游戏 | Steam / PlayStation / Valorant | 霓虹赛博朋克 |
| 医疗健康 | HealthTech / Zocdoc | `#0EA5E9` 天蓝 |
| 教育学习 | EdTech / BYJU'S / Duolingo | `#0284C7` 蓝色 |
| 奢侈品 | 黑金 / 装饰艺术 | `#000000` + `#D4AF37` |
| 母婴/儿童 | 马卡龙 / 柔和色 | `#B2DFDB` 薄荷 |
| 环保/绿色 | GreenTech / Solarpunk | `#059669` 绿色 |

### 按情感调性

| 情感 | 色系 | 代表方案 |
|------|------|----------|
| 🔴 活力热情 | 红色、橙色 | 淘宝、Netflix、YouTube |
| 🔵 专业信任 | 蓝色 | LinkedIn、IBM、银行 |
| 🟣 创新科技 | 紫色、青色 | Figma、Twitch、AI 平台 |
| 🟢 平静安宁 | 浅蓝、薄荷 | 医疗、冥想 |
| ⬛ 奢华高端 | 黑色、金色 | Chanel、暗黑奢华 |
| 🩷 俏皮有趣 | 粉色、黄色 | TikTok、Snapchat、Duolingo |
| 🟤 温暖舒适 | 橙色、棕色 | 咖啡店、烘焙坊 |
| ⬜ 极简干净 | 白色、灰色 | Apple、Notion、Muji |

---

## 📂 项目结构

```
color-palette-skill/
├── README.md                           # 本文件（中英双语）
├── skill.md                            # 核心技能指令（英文版）
├── skill_CN.md                         # 核心技能指令（中文版）
├── color-palette-handbook.md           # 完整配色方案参考手册
└── data/
    ├── china-platforms.json            # 🇨🇳 国内 12 大平台品牌配色
    ├── asia-platforms.json             # 🌏 亚洲 40 大平台品牌配色
    ├── western-platforms.json          # 🌍 西方 41 大平台品牌配色
    ├── global-brands.json              # 🌐 62 个全球消费品牌配色
    ├── dev-frameworks.json             # 🖥️ 40 个开发框架配色
    ├── global-industries.json          # 🏭 116 个全球行业配色
    ├── design-styles.json              # 🎨 31 种设计风格配色
    ├── cultural-palettes.json          # 🌍 31 种文化配色
    ├── emotion-palettes.json           # 💭 53 种情感配色
    ├── industry-palettes-extra.json    # 🏢 12 个扩展行业配色
    ├── style-palettes.json             # 🎭 10 种设计风格配色
    ├── color-palettes-extra.json       # 🌈 8 种色系补充配色
    ├── wordpress-themes.json           # 📝 3 个 WordPress 主题配色
    ├── design-systems.json             # 🎨 5 大设计系统配色
    ├── extra-palettes.json             # 📦 140 套补充配色
    └── batch3-palettes.json            # 🚀 430 套批量扩展配色
```

---

## 🚫 配色禁忌

### ❌ 绝对禁止

- 默认使用蓝紫色渐变（`#667eea → #764ba2`）
- 所有项目使用同一套配色
- 忽略行业特征和品牌调性
- 主色和背景色对比度低于 WCAG AA（4.5:1）

### ✅ 推荐做法

- 根据项目场景匹配配色
- 保持主色、辅色、强调色的层次分明
- 始终提供深色模式支持
- 参考成功产品的配色经验
- 使用语义化颜色令牌

---

## 🤝 贡献

欢迎贡献新的配色方案！请遵循以下规范：

1. 完整的 `colors` 对象（primary、secondary、accent、background、surface、text）
2. 提供 `darkMode` 深色模式色值
3. 包含 `cssVariables` 和 `tailwindConfig` 代码片段
4. 确保对比度满足 WCAG AA（4.5:1）
5. 使用标准 6 位 HEX 格式

---

## 📜 更新日志

### v3.0.0 (2026-05-08)

**重大扩展：68 → 1052+ 套配色方案**

- 🌏 +40 亚洲平台（日本、韩国、印度、东南亚）
- 🌍 +41 西方平台（Google、Apple、Meta、Amazon 等）
- 🌐 +62 全球品牌（Nike、Samsung、BMW、Starbucks 等）
- 🖥️ +40 开发框架（React、Vue、Svelte、Next.js 等）
- 🏭 +116 全球行业（航空、酒店、电信、奢侈品等）
- 🎨 +31 设计风格（玻璃拟态、粗野主义、装饰艺术等）
- 🌍 +31 文化配色（50+ 国家）
- 💭 +53 情感配色
- 📦 +140 补充配色（WP、CMS、UI 组件库、科技行业）
- 🚀 +430 批量扩展（区域平台、CMS模板、游戏、Web3、AI、更多行业/风格/色系）
- 📝 GitHub 风格 skill.md，含 badges、目录、结构化章节
- 🇨🇳 新增 skill_CN.md（中文版）

### v2.0.0 (2026-05-05)

- +30 套配色（总计 68 套）
- 新增分类：industry-extra、style、color-palette-extra
- 修复色系分布不均衡

### v1.0.0 (2026-05-05)

- 初始版本：38 套配色，5 大分类

---

## 📄 许可证

[MIT](LICENSE) — 自由用于任何项目。

---

<p align="center">
  <sub>用 ❤️ 构建，帮助 AI 摆脱蓝紫渐变的束缚。</sub>
</p>
