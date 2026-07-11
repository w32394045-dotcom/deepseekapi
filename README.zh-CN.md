<p align="center">
  <img src="https://img.shields.io/badge/纯前端-无需后端-4f6ef7?style=flat-square" alt="纯前端">
  <img src="https://img.shields.io/badge/Chart.js-4.4.7-ff6384?style=flat-square" alt="Chart.js">
  <img src="https://img.shields.io/badge/多语言-10种-10b981?style=flat-square" alt="多语言">
  <img src="https://img.shields.io/badge/多币种-11种-f59e0b?style=flat-square" alt="多币种">
</p>

<h1 align="center">DeepSeek API 用量与成本分析 <sub><sup>[EXP]</sup></sub></h1>

<p align="center">
  <strong>ZIP/CSV 直传 · 历史追踪 · 月度筛选 · 图表下钻</strong>
  <br>
  一键上传 DeepSeek 账单文件，自动解析、可视化分析 API 用量与费用，无需后端服务。
</p>

---

## ✨ 功能一览

| 类别 | 功能 | 说明 |
|------|------|------|
| 📂 | **ZIP/CSV 直传** | 上传 `cost-*.csv` / `amount-*.csv` 或 ZIP 压缩包，自动识别解析，支持多次追加 |
| 📈 | **月度费用趋势** | 按月展示费用变化曲线，支持交互式缩放 |
| 🔬 | **Token 明细分析** | 分别统计输出 Token、缓存命中、缓存未命中的用量与费用 |
| 📊 | **统计看板** | 总成本、总 Token 数、请求次数等关键指标一目了然 |
| 💱 | **多币种支持** | ¥ CNY · $ USD · ₩ KRW · NT$ TWD · JP¥ JPY · ₽ RUB · £ GBP · € EUR · ฿ THB · ₫ VND · Z$ ZWD |
| 🌐 | **多语言界面** | 简体中文 · 繁體中文 · 日本語 · 한국어 · English · Français · Deutsch · Русский · Tiếng Việt · ไทย |
| 💾 | **数据持久化** | 所有数据存储在浏览器 localStorage，刷新不丢失 |
| 📦 | **数据导入/导出** | 导出为 JSON/ZIP 存档，或导出完整 HTML（含全部数据） |
| 🔑 | **账户余额查询** | 配置 DeepSeek API Key 后可直接查询账户余额 |
| 🔍 | **图表下钻** | 点击趋势图可查看更详细的费用构成 |
| 🎨 | **幻镜主题 (Mirage)** | 毛玻璃质感 UI 风格，支持自定义背景图片/视频 |

---

## 🚀 快速开始

### 在线使用

直接打开 **[GitHub Pages](https://w32394045-dotcom.github.io/deepseekapi/)** 即可使用。

### 本地使用

```bash
git clone https://github.com/w32394045-dotcom/deepseekapi.git
cd deepseekapi
# 直接用浏览器打开 index.html
```

> 无需安装任何依赖，无需后端服务。

---

## 📥 数据来源

1. 登录 [DeepSeek 开放平台](https://platform.deepseek.com/)
2. 下载账单 CSV 文件
3. 将 CSV 文件或 ZIP 压缩包拖拽 / 点击上传到本工具
4. 自动解析并生成可视化分析

---

## 🧮 计算方式

```
输出成本       = Σ (output_tokens × 输出单价)
缓存命中成本   = Σ (input_cache_hit_tokens × 缓存命中单价)
缓存未命中成本 = Σ (input_cache_miss_tokens × 缓存未命中单价)
总成本         = 输出成本 + 缓存命中成本 + 缓存未命中成本
```

---

## 🛠️ 技术栈

| 类别 | 技术 |
|------|------|
| **语言** | 纯 HTML + CSS + JavaScript（零框架依赖） |
| **图表** | [Chart.js](https://www.chartjs.org/) v4.4.7 |
| **压缩** | [JSZip](https://stuk.github.io/jszip/) v3.10.1 |
| **存储** | 浏览器 localStorage |
| **托管** | GitHub Pages |

---

## 🔒 隐私说明

- 所有数据仅在浏览器本地处理，**不会上传至任何服务器**
- API Key 仅用于向 DeepSeek 官方接口查询余额，仅存储在浏览器本地
- 导出/导入功能仅用于数据备份与迁移

---

## 📄 License

MIT
