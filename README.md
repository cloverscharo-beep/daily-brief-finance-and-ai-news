<div align="center">

# 📰 每日资讯站 · Daily Brief

**AI 每日资讯 + 财经每日资讯 · 双刊自动更新**
**Daily AI News & Finance Digest — auto-published every day**

</div>

---

## 这是什么 / What is this?

一个**每天自动更新的个人资讯站**:每晚自动检索全球 AI 与财经要闻,精选 **10 条/刊**,混合**公司官方披露**与**博主/媒体解读**,每条附**原文出处链接**,沉淀为可检索的档案。

A personal news site that updates itself daily: it scans global AI & finance headlines every evening, curates **10 items per edition**, mixing **official company disclosures** with **blogger/media analysis**, and links every item back to the **original source**. Editions are archived and searchable.

| 📰 AI 每日资讯 | 📊 财经每日资讯 |
| --- | --- |
| 模型发布 · 安全政策 · 开源生态 · 国产模型 | 宏观政策 · A股/港股/美股 · 大宗 · 外汇 |
| Model releases · safety & policy · open-source · CN models | Macro & policy · CN/HK/US markets · commodities · FX |

## 🌐 在线访问 / Live sites

| Platform | URL |
| --- | --- |
| GitHub Pages | https://cloverscharo-beep.github.io/daily-brief-ten-finance-and-ai-news/ |
| Cloudflare Pages | https://daily-brief-4u7.pages.dev |

> 两个平台互为备份,任一网络环境打不开时换另一个试试。
> Both platforms mirror each other — if one is unreachable in your network, try the other.

## ✨ 特点 / Features

- **双刊结构** — AI 与财经各自成刊,报纸式排版,亮/暗色自动适配,手机友好
  Two editions in a newspaper-style layout; light/dark auto-adapt; mobile-friendly
- **来源可溯** — 每条要闻标注出处,点击直达原文
  Every item is cited — click through to the original article
- **自动流水线** — 每天早晚双版:早间版 8:50 成稿 → 9:00 上线(隔夜要闻),晚间版 20:50 成稿 → 21:00 上线(当日要闻,不与早间重复),全程无人值守
  Automated: two editions a day — morning (8:50 curate → 09:00 publish, overnight news) & evening (20:50 → 21:00, daytime news, no repeats)
- **沉淀可检索** — 每天一期存成 Markdown 归档(Obsidian 知识库),网页为阅读版
  Each edition is archived as Markdown in an Obsidian vault; the web is the reading layer

## 🛠 技术栈 / How it works

```
Obsidian 知识库(每日 Markdown 笔记)
        │  定时任务:搜索 → 精选 10 条 → 成稿
        ▼
digest_site.py(纯 Python 标准库静态站生成器)
        │  每日 21:00 自动重建
        ▼
静态 HTML 站点 ──► Cloudflare Pages
        └──► GitHub Pages(git 推送)
```

- 生成器:`digest_site.py` — 零依赖,解析 Markdown → 生成首页 + 每期详情页
- 托管:Cloudflare Pages(直接上传)+ GitHub Pages(仓库分支部署)

## 📄 许可 / License

内容为公开新闻的摘要汇编,仅供学习参考,**不构成投资建议**;各条目版权归原作者,完整内容见原文链接。

This is a digest of publicly available news for reference only and is **not investment advice**. Copyright of each item belongs to its original author — see the linked sources.

---

*Made with ❤️ by ChaRo · 每日 20:50 自动成稿,21:00 自动上线*
