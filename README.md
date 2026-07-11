<p align="center">
  <a href="README.zh-CN.md">🇨🇳 中文</a> · <a href="README.md">🇬🇧 English</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Frontend%20Only-No%20Backend-4f6ef7?style=flat-square" alt="Frontend Only">
  <img src="https://img.shields.io/badge/Chart.js-4.4.7-ff6384?style=flat-square" alt="Chart.js">
  <img src="https://img.shields.io/badge/Languages-10-10b981?style=flat-square" alt="Languages">
  <img src="https://img.shields.io/badge/Currencies-11-f59e0b?style=flat-square" alt="Currencies">
</p>

<h1 align="center">DeepSeek API Usage & Cost Analyzer <sub><sup>[EXP]</sup></sub></h1>

<p align="center">
  <strong>ZIP/CSV Upload · History Tracking · Monthly Filter · Chart Drill-Down</strong>
  <br>
  Upload DeepSeek billing files, auto-parse & visualize API usage and costs — no backend required.
</p>

---

## ✨ Features

| Icon | Feature | Description |
|------|---------|-------------|
| 📂 | **Direct Upload** | Drag & drop `cost-*.csv` / `amount-*.csv` or ZIP archives, auto-parsed, batch upload supported |
| 📈 | **Monthly Trends** | Monthly cost trend chart with interactive zoom |
| 🔬 | **Token Breakdown** | Separate stats for output tokens, cache hits & cache misses with costs |
| 📊 | **Dashboard** | Total cost, total tokens, request count — all at a glance |
| 💱 | **Multi-Currency** | ¥ CNY · $ USD · ₩ KRW · NT$ TWD · JP¥ JPY · ₽ RUB · £ GBP · € EUR · ฿ THB · ₫ VND · Z$ ZWD |
| 🌐 | **Multi-Language** | 简体中文 · 繁體中文 · 日本語 · 한국어 · English · Français · Deutsch · Русский · Tiếng Việt · ไทย (10 languages) |
| 💾 | **Local Persistence** | All data stored in browser localStorage, persists across refreshes |
| 📦 | **Import & Export** | Export as JSON/ZIP archive, or export full HTML with embedded data |
| 🔑 | **Balance Check** | Query your account balance directly via DeepSeek API Key |
| 🔍 | **Drill-Down** | Click charts to dive deeper into cost details |
| 🎨 | **Mirage Theme** | Frosted glass UI with custom wallpaper & video backgrounds |

---

## 🚀 Quick Start

### Online

Open **[GitHub Pages](https://w32394045-dotcom.github.io/deepseekapi/)** directly in your browser.

### Local

```bash
git clone https://github.com/w32394045-dotcom/deepseekapi.git
cd deepseekapi
# Open index.html in your browser
```

> No dependencies to install, no server required.

---

## 📥 Data Source

1. Sign in to the [DeepSeek Platform](https://platform.deepseek.com/)
2. Download billing CSV files
3. Drag & drop or click to upload CSV/ZIP files
4. Auto-parsed and visualized

---

## 🧮 Cost Calculation

```
Output Cost          = Σ (output_tokens × output unit price)
Cache Hit Cost       = Σ (input_cache_hit_tokens × cache hit unit price)
Cache Miss Cost      = Σ (input_cache_miss_tokens × cache miss unit price)
Total Cost           = Output Cost + Cache Hit Cost + Cache Miss Cost
```

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Language** | Vanilla HTML + CSS + JS (zero framework deps) |
| **Charts** | [Chart.js](https://www.chartjs.org/) v4.4.7 |
| **Archive** | [JSZip](https://stuk.github.io/jszip/) v3.10.1 |
| **Storage** | Browser localStorage |
| **Hosting** | GitHub Pages |

---

## 🔒 Privacy

- All data is processed locally in your browser, **never uploaded to any server**
- API Key is only used to query balances from DeepSeek's official API, stored locally only
- Export/Import is only for data backup and migration

---

## 📄 License

MIT
