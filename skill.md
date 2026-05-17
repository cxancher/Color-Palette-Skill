---
name: Color Palette Skill
description: 1052+ professional color palettes covering 50+ countries, 100+ industries, 40+ tech stacks, 18 categories. Break free from blue-purple gradients. Auto-activate when frontend development, UI design, web color scheme, or brand design is needed.
version: 3.0.0
tags: [color, palette, design, frontend, ui, css, theme, brand]
---

# 🎨 Color Palette Skill - 配色大师

<p align="center">
  <strong>1052+ Professional Color Palettes for AI-Driven Design</strong><br>
  <em>Break free from blue-purple gradients. Cover every platform, industry, style, and culture.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/palettes-1052+-blue" alt="1052+ Palettes">
  <img src="https://img.shields.io/badge/categories-18-green" alt="18 Categories">
  <img src="https://img.shields.io/badge/countries-50+-orange" alt="50+ Countries">
  <img src="https://img.shields.io/badge/industries-100+-red" alt="100+ Industries">
  <img src="https://img.shields.io/badge/version-3.0.0-purple" alt="v3.0.0">
</p>

---

> **Version**: 3.0.0 | **Last Updated**: 2026-05-08
> **Trigger**: Auto-activate when frontend development, UI design, web color scheme, or brand design is needed.

---

## 📋 Table of Contents

- [Core Directives](#-core-directives)
- [Palette Categories](#-palette-categories-18-categories)
- [Data Format](#-data-format)
- [Usage Methods](#-usage-methods)
- [Smart Recommendation](#-smart-recommendation)
- [Color禁忌](#-color-taboos)
- [Data Files Index](#-data-files-index)
- [Changelog](#-changelog)

---

## ⚡ Core Directives

### Decision Flow

```
User Request → Analyze Scene/Industry → Match Palette → Apply to Code
```

### Decision Tree

| Priority | Condition | Action |
|----------|-----------|--------|
| 1 | User specified brand/platform | Use exact brand palette |
| 2 | User specified industry | Use industry-recommended palette |
| 3 | User specified design style | Match closest style palette |
| 4 | User unspecified | Smart-recommend 2-3 options based on project type |

### ⚠️ First Rule

> **NEVER default to blue-purple gradients (`#667eea → #764ba2`)**. Always select a context-appropriate palette from this library.

---

## 🗂️ Palette Categories (18 Categories)

| # | Category | Count | File | Coverage |
|---|----------|-------|------|----------|
| 1 | 🇨🇳 China Platforms | 12 | `china-platforms.json` | Taobao, Douyin, WeChat, Bilibili, Meituan, JD, PDD, Xiaohongshu, Baidu, NetEase, 360, IQiyi |
| 2 | 🌏 Asia Platforms | 40 | `asia-platforms.json` | Japan (LINE, Rakuten, Mercari), Korea (NAVER, Kakao, Coupang, Toss), India (Flipkart, Swiggy, Paytm), SEA (Grab, Gojek, Shopee) |
| 3 | 🌍 Western Platforms | 41 | `western-platforms.json` | Google, Apple, Meta, Amazon, Netflix, Spotify, Slack, Notion, Figma, Stripe, Airbnb, Uber, Twitter/X |
| 4 | 🌐 Global Brands | 62 | `global-brands.json` | Nike, Adidas, Samsung, Sony, BMW, Mercedes, Tesla, Coca-Cola, Pepsi, Starbucks, McDonald's, IKEA, Lego |
| 5 | 🖥️ Dev Frameworks | 40 | `dev-frameworks.json` | React, Vue, Angular, Svelte, Next.js, Nuxt, Remix, Astro, SvelteKit, Qwik, Solid, htmx, Alpine, Three.js, D3.js |
| 6 | 🏭 Global Industries | 116 | `global-industries.json` | Finance, Healthcare, Education, Real Estate, Legal, Automotive, Aviation, Hospitality, Telecom, Energy, Luxury, FMCG |
| 7 | 🎨 Design Styles | 31 | `design-styles.json` | Minimalist, Brutalist, Cyberpunk, Retro, Nordic, Japanese, Art Deco, Bauhaus, Glassmorphism, Neumorphism |
| 8 | 🌍 Cultural Palettes | 31 | `cultural-palettes.json` | Japan, Korea, India, Brazil, Russia, Germany, France, UK, Southeast Asia, Middle East, Africa |
| 9 | 💭 Emotion Palettes | 53 | `emotion-palettes.json` | Trust, Energy, Calm, Passion, Innovation, Luxury, Playful, Professional, Warm, Cool |
| 10 | 🇨🇳 Industry Extra | 12 | `industry-palettes-extra.json` | Legal, Fitness, Gaming, Pet, Logistics, Agriculture, Insurance, Media, Auto, Pharma, Architecture, NGO |
| 11 | 🎭 Style Palettes | 10 | `style-palettes.json` | Retro, Cyberpunk, Nordic, Japanese, Dark Luxury, Bohemian, Corporate Warm, Neon, Earth, Macaron |
| 12 | 🌈 Color Palettes Extra | 8 | `color-palettes-extra.json` | Teal, Brown, Gold, Coral, Mint, Lavender, Indigo, Salmon |
| 13 | 📝 WordPress Themes | 3 | `wordpress-themes.json` | Flavor, Avada, Enfold |
| 14 | 🎨 Design Systems | 5 | `design-systems.json` | Material, Ant Design, Fluent, Human Interface, Carbon |
| 15 | 📦 Extra Palettes | 140 | `extra-palettes.json` | 27 WP themes, 15 design systems, 40 tech industries, 20 styles, 30 color families |
| 16 | 🚀 Batch 3 Palettes | 430 | `batch3-palettes.json` | 60 regional platforms, 50 CMS templates, 40 UI kits, 30 gaming, 30 Web3, 30 AI, 60 industries, 30 styles, 30 colors, 30 cultures, 30 emotions |
| 17 | 🌐 Regional Platforms | (in batch3) | — | 60 platforms across Japan, Korea, India, SEA, Brazil, Russia, Middle East, Europe, Africa, LatAm |
| 18 | 🤖 AI/Web3/Gaming | (in batch3) | — | 30 AI platforms, 30 Web3/crypto, 30 gaming platforms |

**Total: 1052+ palettes across 18 categories, covering 50+ countries, 100+ industries, all major tech stacks.**

---

## 📐 Data Format

Each palette follows this standard schema:

```jsonc
{
  "id": "unique-identifier",
  "name": "Palette Name",
  "category": "category-key",
  "tags": ["tag1", "tag2", "tag3"],
  "style": "Design style description",
  "colors": {
    "primary": "#HEX",       // Main brand color
    "secondary": "#HEX",     // Supporting color
    "accent": "#HEX",        // Highlight/CTA color
    "background": "#HEX",    // Page background
    "surface": "#HEX",       // Card/container background
    "text": "#HEX",          // Primary text
    "textSecondary": "#HEX", // Secondary text
    "border": "#HEX",        // Border color
    "success": "#HEX",       // Success state
    "warning": "#HEX",       // Warning state
    "error": "#HEX"          // Error state
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

### Category Values

```
china-platform | asia-platform | western-platform | global-brand
dev-framework | global-industry | design-style | cultural-palette
emotion-palette | industry-extra | style-palette | color-palette-extra
wordpress-theme | design-system | cms-template | regional-platform
ui-component | gaming | web3 | ai-platform
industry-detail | style-detail | color-detail | cultural-detail | emotion-detail
```

---

## 🔧 Usage Methods

### Method 1: CSS Variables (Recommended)

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

/* Dark mode */
[data-theme="dark"] {
  --color-background: #0D0D0D;
  --color-surface: #1A1A1A;
  --color-text: #F5F5F5;
  --color-text-secondary: #A3A3A3;
  --color-border: #333333;
}
```

### Method 2: Tailwind CSS

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

### Method 3: Design Tokens

```json
{
  "color": {
    "primary": { "value": "#FF5000" },
    "secondary": { "value": "#FF4400" },
    "accent": { "value": "#FF0036" }
  }
}
```

### Method 4: SCSS Variables

```scss
$color-primary: #FF5000;
$color-secondary: #FF4400;
$color-accent: #FF0036;
$color-background: #F5F5F5;
$color-surface: #FFFFFF;
$color-text: #333333;
```

---

## 🧠 Smart Recommendation

### By Project Type

| Project Type | Recommended Palette | Reason |
|-------------|-------------------|--------|
| E-commerce | Taobao / Tmall / Shopee / Rakuten | Orange-red stimulates purchasing |
| Social App | WeChat / LINE / Kakao / Discord | Green/purple friendly & social |
| Enterprise | Ant Design / IBM Carbon / SAP Fiori | Blue professional & reliable |
| SaaS Product | Linear / Vercel / Stripe | Dark modern feel |
| Content Platform | Notion / Ghost / WordPress | Minimal content-first |
| Short Video | Douyin / TikTok / YouTube | Dark immersive |
| Food/Delivery | Meituan / Swiggy / iFood | Warm stimulates appetite |
| Finance/Payment | Alipay / Nubank / Wise | Blue security & trust |
| Education | EdTech / BYJU'S / Duolingo | Blue/purple knowledge |
| Healthcare | HealthTech / Zocdoc | Green cleanliness |
| Legal | Deep Navy / Law Firm palette | Navy authority |
| Gaming | Steam / PlayStation / Valorant | Neon cyberpunk |
| Fitness | Fluorescent green / Nike | Energy & breakthrough |
| Real Estate | Zillow / PropTech | Blue trust |
| Travel | Booking / Airbnb / Traveloka | Blue exploration |
| AI/ML Tool | OpenAI / Hugging Face / Cursor | Modern tech feel |
| Crypto/Web3 | Bitcoin / Ethereum / OpenSea | Brand-specific |
| Government | Deep blue / neutral gray | Authority & neutrality |
| News/Media | Deep red / black & white | Serious & authoritative |
| Luxury Brand | Black & gold / Art Deco | Premium & exclusive |
| Children/Kids | Pastel / Macaron | Soft & friendly |
| Eco/Green | GreenTech / Solarpunk | Sustainability |

### By Emotion/Tone

| Emotion | Color Family | Example Palettes |
|---------|-------------|-----------------|
| Energy & Passion | Red, Orange | Taobao, Netflix, YouTube |
| Trust & Professional | Blue | LinkedIn, IBM, Banks |
| Innovation & Tech | Purple, Cyan | Figma, Twitch, AI platforms |
| Calm & Serene | Light Blue, Mint | Healthcare, Meditation |
| Luxury & Premium | Black, Gold | Chanel, Rolex, Dark Luxury |
| Playful & Fun | Pink, Yellow | TikTok, Snapchat, Duolingo |
| Nature & Organic | Green, Brown | Whole Foods, Agriculture |
| Minimal & Clean | White, Gray | Apple, Notion, Muji |
| Warm & Cozy | Orange, Brown | Coffee shops, Bakeries |
| Bold & Edgy | Black, Neon | Gaming, Cyberpunk |

---

## 🚫 Color Taboos

### ❌ Absolutely Forbidden

- Defaulting to blue-purple gradients (`#667eea → #764ba2`)
- Using the same palette for every project
- Ignoring industry characteristics and brand tone
- Primary/background contrast ratio below WCAG AA (4.5:1)
- Using more than 5 colors in a single design system

### ✅ Best Practices

- Select palette based on project context and industry
- Maintain clear hierarchy: primary > secondary > accent
- Always provide dark mode support
- Reference successful products' color choices
- Test contrast ratios with accessibility tools
- Use `cssVariables` field directly from palette data

---

## 📁 Data Files Index

| File | Palettes | Description |
|------|----------|-------------|
| `data/china-platforms.json` | 12 | 🇨🇳 Chinese platform brand colors |
| `data/asia-platforms.json` | 40 | 🌏 Asian platform brand colors |
| `data/western-platforms.json` | 41 | 🌍 Western platform brand colors |
| `data/global-brands.json` | 62 | 🌐 Global consumer brand colors |
| `data/dev-frameworks.json` | 40 | 🖥️ Developer framework colors |
| `data/global-industries.json` | 116 | 🏭 Global industry colors |
| `data/design-styles.json` | 31 | 🎨 Design style palettes |
| `data/cultural-palettes.json` | 31 | 🌍 Cultural color preferences |
| `data/emotion-palettes.json` | 53 | 💭 Emotion-based palettes |
| `data/industry-palettes-extra.json` | 12 | 🏢 Extended industry palettes |
| `data/style-palettes.json` | 10 | 🎭 Design style palettes |
| `data/color-palettes-extra.json` | 8 | 🌈 Extended color families |
| `data/wordpress-themes.json` | 3 | 📝 WordPress theme palettes |
| `data/design-systems.json` | 5 | 🎨 Design system palettes |
| `data/extra-palettes.json` | 140 | 📦 Supplementary palettes (WP, DS, tech, style, color) |
| `data/batch3-palettes.json` | 430 | 🚀 Major expansion (regional, CMS, UI, gaming, Web3, AI, industry, style, color, culture, emotion) |

---

## 📝 Changelog

### v3.0.0 (2026-05-08)

**Major expansion: 68 → 1052+ palettes**

#### New Categories (10 new)
- 🌏 Asia Platforms (40) — Japan, Korea, India, Southeast Asia
- 🌍 Western Platforms (41) — US, Europe tech giants
- 🌐 Global Brands (62) — Nike, Samsung, BMW, Starbucks, etc.
- 🖥️ Dev Frameworks (40) — React, Vue, Svelte, Next.js, etc.
- 🏭 Global Industries (116) — Aviation, hospitality, telecom, luxury, FMCG, etc.
- 🎨 Design Styles (31) — Glassmorphism, Brutalism, Art Deco, etc.
- 🌍 Cultural Palettes (31) — Japan, Korea, India, Brazil, Russia, etc.
- 💭 Emotion Palettes (53) — Trust, Energy, Calm, Passion, etc.

#### Batch 3 Expansion (430 new)
- 🌐 Regional Platforms (60) — 50+ countries: Japan, Korea, India, SEA, Brazil, Russia, Middle East, Europe, Africa, LatAm
- 📦 CMS Templates (50) — Shopify, Wix, Squarespace, Webflow, Ghost, Hugo, Gatsby, Next.js, etc.
- 🧩 UI Components (40) — Ant Design, Element Plus, Vuetify, Chakra UI, shadcn/ui, Mantine, etc.
- 🎮 Gaming (30) — Steam, PlayStation, Xbox, Nintendo, Riot, Discord, Twitch, etc.
- ⛓️ Web3/Crypto (30) — Bitcoin, Ethereum, Solana, OpenSea, MetaMask, Coinbase, etc.
- 🤖 AI Platforms (30) — OpenAI, Anthropic, Hugging Face, Midjourney, Cursor, etc.
- 🏢 Industry Detail (60) — Coworking, bakery, gym, yoga, museum, cinema, esports, etc.
- 🎨 Style Detail (30) — Glassmorphism, Neumorphism, Cottagecore, Cyberpunk v2, etc.
- 🌈 Color Detail (30) — Monochrome, Analogous, Complementary, Pastel, Neon, etc.
- 🌍 Cultural Detail (30) — Thailand, Vietnam, Egypt, Nigeria, Colombia, etc.
- 💭 Emotion Detail (30) — Serenity, Nostalgia, Wonder, Freedom, Dreamy, etc.

#### Improvements
- Reformatted skill.md for GitHub-style display
- Added badges, table of contents, and structured sections
- Comprehensive smart recommendation tables
- Full tech stack coverage (React, Vue, Angular, Svelte, Flutter, SwiftUI, Jetpack Compose, etc.)
- Full CMS coverage (WordPress, Shopify, Ghost, Webflow, Squarespace, Wix, etc.)
- Full geographic coverage (50+ countries across all continents)

### v2.0.0 (2026-05-05)
- Added 30 palettes (total 68)
- New categories: industry-extra, style, color-palette-extra
- Fixed color distribution imbalance

### v1.0.0 (2026-05-05)
- Initial release with 38 palettes
- 5 categories: China platforms, International platforms, Design systems, WordPress themes, Industries
- CSS Variables, Tailwind CSS, Design Tokens output formats

---

## 📄 License

MIT License — Free to use in any project.

---

<p align="center">
  <sub>Built with ❤️ for designers and developers who believe in the power of color.</sub>
</p>
