---
name: 配色大师技能
description: 1052+ 专业配色方案，覆盖 50+ 国家、100+ 行业、40+ 技术栈、18 大分类。告别千篇一律的蓝紫渐变。当前端开发、UI 设计、网页配色或品牌设计需求时自动激活。
version: 3.0.0
tags: [配色, 色板, 设计, 前端, UI, CSS, 主题, 品牌]
---

# 🎨 配色大师技能 - Color Palette Skill

<p align="center">
  <strong>1052+ 专业配色方案，赋能 AI 驱动设计</strong><br>
  <em>告别千篇一律的蓝紫渐变。覆盖全平台、全行业、全风格、全文化。</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/palettes-1052+-blue" alt="1052+ Palettes">
  <img src="https://img.shields.io/badge/categories-18-green" alt="18 Categories">
  <img src="https://img.shields.io/badge/countries-50+-orange" alt="50+ Countries">
  <img src="https://img.shields.io/badge/industries-100+-red" alt="100+ Industries">
  <img src="https://img.shields.io/badge/version-3.0.0-purple" alt="v3.0.0">
</p>

---

> **版本**: 3.0.0 | **最后更新**: 2026-05-08
> **触发条件**: 当涉及前端开发、UI 设计、网页配色或品牌设计时自动激活。

---

## 📋 目录

- [核心指令](#-核心指令)
- [配色分类](#-配色分类-18-大类)
- [数据格式](#-数据格式)
- [使用方法](#-使用方法)
- [智能推荐](#-智能推荐)
- [Color 禁忌](#-color-禁忌)
- [数据文件索引](#-数据文件索引)
- [更新日志](#-更新日志)

---

## ⚡ 核心指令

### 决策流程

```
用户请求 → 分析场景/行业 → 匹配配色方案 → 应用到代码
```

### 决策树

| 优先级 | 条件 | 操作 |
|--------|------|------|
| 1 | 用户指定了品牌/平台 | 使用对应品牌配色 |
| 2 | 用户指定了行业 | 使用行业推荐配色 |
| 3 | 用户指定了设计风格 | 匹配最接近的风格配色 |
| 4 | 用户未指定 | 根据项目类型智能推荐 2-3 个方案 |

### ⚠️ 第一原则

> **绝不默认使用蓝紫渐变（`#667eea → #764ba2`）**。始终从本库中选取符合上下文的配色方案。

---

## 🗂️ 配色分类（18 大类）

| # | 分类 | 数量 | 文件 | 覆盖范围 |
|---|------|------|------|----------|
| 1 | 🇨🇳 中国平台 | 12 | `china-platforms.json` | 淘宝、抖音、微信、B站、美团、京东、拼多多、小红书、百度、网易、360、爱奇艺 |
| 2 | 🌏 亚洲平台 | 40 | `asia-platforms.json` | 日本（LINE、Rakuten、Mercari）、韩国（NAVER、Kakao、Coupang、Toss）、印度（Flipkart、Swiggy、Paytm）、东南亚（Grab、Gojek、Shopee） |
| 3 | 🌍 欧美平台 | 41 | `western-platforms.json` | Google、Apple、Meta、Amazon、Netflix、Spotify、Slack、Notion、Figma、Stripe、Airbnb、Uber、Twitter/X |
| 4 | 🌐 全球品牌 | 62 | `global-brands.json` | Nike、Adidas、Samsung、Sony、BMW、Mercedes、Tesla、Coca-Cola、Pepsi、Starbucks、McDonald's、IKEA、Lego |
| 5 | 🖥️ 开发框架 | 40 | `dev-frameworks.json` | React、Vue、Angular、Svelte、Next.js、Nuxt、Remix、Astro、SvelteKit、Qwik、Solid、htmx、Alpine、Three.js、D3.js |
| 6 | 🏭 全球行业 | 116 | `global-industries.json` | 金融、医疗、教育、房地产、法律、汽车、航空、酒店、电信、能源、奢侈品、快消品 |
| 7 | 🎨 设计风格 | 31 | `design-styles.json` | 极简主义、粗野主义、赛博朋克、复古、北欧、日式、装饰艺术、包豪斯、玻璃拟态、新拟态 |
| 8 | 🌍 文化配色 | 31 | `cultural-palettes.json` | 日本、韩国、印度、巴西、俄罗斯、德国、法国、英国、东南亚、中东、非洲 |
| 9 | 💭 情感配色 | 53 | `emotion-palettes.json` | 信任、活力、平静、热情、创新、奢华、趣味、专业、温暖、冷静 |
| 10 | 🇨🇳 行业扩展 | 12 | `industry-palettes-extra.json` | 法律、健身、游戏、宠物、物流、农业、保险、媒体、汽车、制药、建筑、公益 |
| 11 | 🎭 风格配色 | 10 | `style-palettes.json` | 复古、赛博朋克、北欧、日式、暗黑奢华、波西米亚、企业暖色、霓虹、大地色、马卡龙 |
| 12 | 🌈 色系扩展 | 8 | `color-palettes-extra.json` | 青色、棕色、金色、珊瑚色、薄荷色、薰衣草色、靛蓝色、鲑鱼色 |
| 13 | 📝 WordPress 主题 | 3 | `wordpress-themes.json` | Flavor、Avada、Enfold |
| 14 | 🎨 设计系统 | 5 | `design-systems.json` | Material、Ant Design、Fluent、Human Interface、Carbon |
| 15 | 📦 扩展配色 | 140 | `extra-palettes.json` | 27 个 WP 主题、15 个设计系统、40 个科技行业、20 种风格、30 个色系 |
| 16 | 🚀 第三批配色 | 430 | `batch3-palettes.json` | 60 个区域平台、50 个 CMS 模板、40 个 UI 组件库、30 个游戏、30 个 Web3、30 个 AI、60 个行业、30 种风格、30 个色系、30 种文化、30 种情感 |
| 17 | 🌐 区域平台 |（含于第三批） | — | 覆盖日本、韩国、印度、东南亚、巴西、俄罗斯、中东、欧洲、非洲、拉美的 60 个平台 |
| 18 | 🤖 AI/Web3/游戏 |（含于第三批） | — | 30 个 AI 平台、30 个 Web3/加密货币、30 个游戏平台 |

**总计：18 大类共 1052+ 套配色方案，覆盖 50+ 国家、100+ 行业、所有主流技术栈。**

---

## 📐 数据格式

每套配色遵循以下标准结构：

```jsonc
{
  "id": "唯一标识符",
  "name": "配色方案名称",
  "category": "分类键值",
  "tags": ["标签1", "标签2", "标签3"],
  "style": "设计风格描述",
  "colors": {
    "primary": "#HEX",       // 主品牌色
    "secondary": "#HEX",     // 辅助色
    "accent": "#HEX",        // 强调/CTA 色
    "background": "#HEX",    // 页面背景色
    "surface": "#HEX",       // 卡片/容器背景色
    "text": "#HEX",          // 主文本色
    "textSecondary": "#HEX", // 次要文本色
    "border": "#HEX",        // 边框色
    "success": "#HEX",       // 成功状态色
    "warning": "#HEX",       // 警告状态色
    "error": "#HEX"          // 错误状态色
  },
  "darkMode": {
    "background": "#HEX",
    "surface": "#HEX",
    "text": "#HEX"
  },
  "cssVariables": ":root { --color-primary: #HEX; ... }",
  "tailwindConfig": "module.exports = { theme: { extend: { colors: { ... } } } }"
}
```

### 分类值

```
china-platform | asia-platform | western-platform | global-brand
dev-framework | global-industry | design-style | cultural-palette
emotion-palette | industry-extra | style-palette | color-palette-extra
wordpress-theme | design-system | cms-template | regional-platform
ui-component | gaming | web3 | ai-platform
industry-detail | style-detail | color-detail | cultural-detail | emotion-detail
```

---

## 🔧 使用方法

### 方法一：CSS 变量（推荐）

```css
:root {
  --color-primary: #FF5000;
  --color-secondary: #FF4400;
  --color-accent: #FF0036;
  --color-background: #F5F5F5;
  --color-surface: #FFFFFF;
  --color-text: #333333;
  --color-text-secondary: #666666;
  --color-border: #E5E5E5;
  --color-success: #10B981;
  --color-warning: #F59E0B;
  --color-error: #EF4444;
}

/* 暗色模式 */
[data-theme="dark"] {
  --color-background: #0D0D0D;
  --color-surface: #1A1A1A;
  --color-text: #F5F5F5;
  --color-text-secondary: #A3A3A3;
  --color-border: #333333;
}
```

### 方法二：Tailwind CSS

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: '#FF5000',
        secondary: '#FF4400',
        accent: '#FF0036',
        surface: '#FFFFFF',
      }
    }
  }
}
```

### 方法三：Design Tokens

```json
{
  "color": {
    "primary": { "value": "#FF5000" },
    "secondary": { "value": "#FF4400" },
    "accent": { "value": "#FF0036" }
  }
}
```

### 方法四：SCSS 变量

```scss
$color-primary: #FF5000;
$color-secondary: #FF4400;
$color-accent: #FF0036;
$color-background: #F5F5F5;
$color-surface: #FFFFFF;
$color-text: #333333;
```

---

## 🧠 智能推荐

### 按项目类型

| 项目类型 | 推荐配色 | 推荐理由 |
|----------|----------|----------|
| 电商 | 淘宝 / 天猫 / Shopee / Rakuten | 橙红色刺激购买欲 |
| 社交应用 | 微信 / LINE / Kakao / Discord | 绿色/紫色亲切且社交感强 |
| 企业级 | Ant Design / IBM Carbon / SAP Fiori | 蓝色专业可靠 |
| SaaS 产品 | Linear / Vercel / Stripe | 暗色现代感 |
| 内容平台 | Notion / Ghost / WordPress | 极简内容优先 |
| 短视频 | 抖音 / TikTok / YouTube | 暗色沉浸感 |
| 美食/外卖 | 美团 / Swiggy / iFood | 暖色刺激食欲 |
| 金融/支付 | 支付宝 / Nubank / Wise | 蓝色安全可信 |
| 教育 | EdTech / BYJU'S / Duolingo | 蓝紫色知识感 |
| 医疗健康 | HealthTech / Zocdoc | 绿色洁净感 |
| 法律 | 深海军蓝 / 律所配色 | 海军蓝权威感 |
| 游戏 | Steam / PlayStation / Valorant | 霓虹赛博朋克 |
| 健身 | 荧光绿 / Nike | 活力与突破感 |
| 房地产 | Zillow / PropTech | 蓝色信任感 |
| 旅行 | Booking / Airbnb / Traveloka | 蓝色探索感 |
| AI/ML 工具 | OpenAI / Hugging Face / Cursor | 现代科技感 |
| 加密货币/Web3 | Bitcoin / Ethereum / OpenSea | 品牌专属色 |
| 政府/政务 | 深蓝 / 中性灰 | 权威与中立 |
| 新闻/媒体 | 深红 / 黑白 | 严肃权威 |
| 奢侈品牌 | 黑金 / 装饰艺术 | 高端与专属 |
| 儿童/亲子 | 粉彩 / 马卡龙 | 柔和友好 |
| 环保/绿色 | GreenTech / Solarpunk | 可持续发展 |

### 按情感/基调

| 情感 | 色系 | 示例配色 |
|------|------|----------|
| 活力与热情 | 红色、橙色 | 淘宝、Netflix、YouTube |
| 信任与专业 | 蓝色 | LinkedIn、IBM、银行 |
| 创新与科技 | 紫色、青色 | Figma、Twitch、AI 平台 |
| 平静与宁静 | 浅蓝、薄荷 | 医疗、冥想 |
| 奢华与高端 | 黑色、金色 | Chanel、Rolex、暗黑奢华 |
| 趣味与活泼 | 粉色、黄色 | TikTok、Snapchat、Duolingo |
| 自然与有机 | 绿色、棕色 | Whole Foods、农业 |
| 极简与干净 | 白色、灰色 | Apple、Notion、Muji |
| 温暖与舒适 | 橙色、棕色 | 咖啡店、面包店 |
| 大胆与前卫 | 黑色、霓虹 | 游戏、赛博朋克 |

---

## 🚫 Color 禁忌

### ❌ 绝对禁止

- 默认使用蓝紫渐变（`#667eea → #764ba2`）
- 每个项目都使用同一套配色
- 忽略行业特征和品牌调性
- 主色与背景对比度低于 WCAG AA 标准（4.5:1）
- 单个设计系统中使用超过 5 种颜色

### ✅ 最佳实践

- 根据项目上下文和行业选择配色
- 保持清晰的层级关系：主色 > 辅助色 > 强调色
- 始终提供暗色模式支持
- 参考成功产品的色彩选择
- 使用无障碍工具测试对比度
- 直接使用配色数据中的 `cssVariables` 字段

---

## 📁 数据文件索引

| 文件 | 配色数量 | 说明 |
|------|----------|------|
| `data/china-platforms.json` | 12 | 🇨🇳 中国平台品牌色 |
| `data/asia-platforms.json` | 40 | 🌏 亚洲平台品牌色 |
| `data/western-platforms.json` | 41 | 🌍 欧美平台品牌色 |
| `data/global-brands.json` | 62 | 🌐 全球消费品牌色 |
| `data/dev-frameworks.json` | 40 | 🖥️ 开发框架色 |
| `data/global-industries.json` | 116 | 🏭 全球行业色 |
| `data/design-styles.json` | 31 | 🎨 设计风格配色 |
| `data/cultural-palettes.json` | 31 | 🌍 文化色彩偏好 |
| `data/emotion-palettes.json` | 53 | 💭 基于情感的配色 |
| `data/industry-palettes-extra.json` | 12 | 🏢 扩展行业配色 |
| `data/style-palettes.json` | 10 | 🎭 设计风格配色 |
| `data/color-palettes-extra.json` | 8 | 🌈 扩展色系 |
| `data/wordpress-themes.json` | 3 | 📝 WordPress 主题配色 |
| `data/design-systems.json` | 5 | 🎨 设计系统配色 |
| `data/extra-palettes.json` | 140 | 📦 补充配色（WP、DS、科技、风格、色系） |
| `data/batch3-palettes.json` | 430 | 🚀 大规模扩展（区域、CMS、UI、游戏、Web3、AI、行业、风格、色系、文化、情感） |

---

## 📝 更新日志

### v3.0.0 (2026-05-08)

**大规模扩展：68 → 1052+ 套配色**

#### 新增分类（10 个）
- 🌏 亚洲平台（40）—— 日本、韩国、印度、东南亚
- 🌍 欧美平台（41）—— 美国、欧洲科技巨头
- 🌐 全球品牌（62）—— Nike、Samsung、BMW、Starbucks 等
- 🖥️ 开发框架（40）—— React、Vue、Svelte、Next.js 等
- 🏭 全球行业（116）—— 航空、酒店、电信、奢侈品、快消品等
- 🎨 设计风格（31）—— 玻璃拟态、粗野主义、装饰艺术等
- 🌍 文化配色（31）—— 日本、韩国、印度、巴西、俄罗斯等
- 💭 情感配色（53）—— 信任、活力、平静、热情等

#### 第三批扩展（430 个新增）
- 🌐 区域平台（60）—— 50+ 国家：日本、韩国、印度、东南亚、巴西、俄罗斯、中东、欧洲、非洲、拉美
- 📦 CMS 模板（50）—— Shopify、Wix、Squarespace、Webflow、Ghost、Hugo、Gatsby、Next.js 等
- 🧩 UI 组件库（40）—— Ant Design、Element Plus、Vuetify、Chakra UI、shadcn/ui、Mantine 等
- 🎮 游戏（30）—— Steam、PlayStation、Xbox、Nintendo、Riot、Discord、Twitch 等
- ⛓️ Web3/加密货币（30）—— Bitcoin、Ethereum、Solana、OpenSea、MetaMask、Coinbase 等
- 🤖 AI 平台（30）—— OpenAI、Anthropic、Hugging Face、Midjourney、Cursor 等
- 🏢 行业细分（60）—— 共享办公、烘焙店、健身房、瑜伽、博物馆、电影院、电竞等
- 🎨 风格细分（30）—— 玻璃拟态、新拟态、田园风、赛博朋克 v2 等
- 🌈 色系细分（30）—— 单色、类似色、互补色、粉彩、霓虹等
- 🌍 文化细分（30）—— 泰国、越南、埃及、尼日利亚、哥伦比亚等
- 💭 情感细分（30）—— 宁静、怀旧、惊奇、自由、梦幻等

#### 改进
- 重新格式化 skill.md 以适配 GitHub 风格展示
- 新增徽章、目录和结构化章节
- 完善的智能推荐表格
- 全技术栈覆盖（React、Vue、Angular、Svelte、Flutter、SwiftUI、Jetpack Compose 等）
- 全 CMS 覆盖（WordPress、Shopify、Ghost、Webflow、Squarespace、Wix 等）
- 全地理覆盖（50+ 国家，横跨各大洲）

### v2.0.0 (2026-05-05)
- 新增 30 套配色（总计 68 套）
- 新增分类：行业扩展、风格、色系扩展
- 修复色彩分布不均衡问题

### v1.0.0 (2026-05-05)
- 首次发布，包含 38 套配色
- 5 个分类：中国平台、国际平台、设计系统、WordPress 主题、行业
- 支持 CSS Variables、Tailwind CSS、Design Tokens 输出格式

---

## 📄 许可证

MIT 许可证 —— 可自由用于任何项目。

---

<p align="center">
  <sub>用 ❤️ 为相信色彩力量的设计师和开发者而建。</sub>
</p>
