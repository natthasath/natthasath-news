# 🎉 natthasath-news

Automated Thai news digest, published as a static site on GitHub Pages. Scheduled Claude Code cloud routines collect, cross-validate, and summarize news across 10 categories, write self-contained HTML reports directly into this repository, and keep each category's archive page up to date — no manual publishing step required.

![license](https://img.shields.io/github/license/natthasath/natthasath-news)
![stars](https://img.shields.io/github/stars/natthasath/natthasath-news)
![last-commit](https://img.shields.io/github/last-commit/natthasath/natthasath-news)
![issues](https://img.shields.io/github/issues/natthasath/natthasath-news)

### ✨ Features

- Sources are tiered per category routine (Tier 1 Official / Tier 2 Trusted Media / Tier 3 Trend-only)
- Each report is a fully self-contained HTML file (inline CSS, no external stylesheet)
- Each category's `index.html` archive is updated automatically on every new report (idempotent — reruns within the same day/week replace rather than duplicate)
- Commits and pushes to `main` automatically — no manual publishing step
- Site theme supports both light/dark, following system preference

### 📅 Categories & Schedule

| Folder | Frequency | Category | Live Page |
|---|---|---|---|
| [`ai/`](ai/) | Daily | AI & Technology | [Open](https://natthasath.github.io/natthasath-news/ai/) |
| [`economics/`](economics/) | Daily | Economics | [Open](https://natthasath.github.io/natthasath-news/economics/) |
| [`football/`](football/) | Weekly | Premier League | [Open](https://natthasath.github.io/natthasath-news/football/) |
| [`software/`](software/) | Weekly | Software Releases | [Open](https://natthasath.github.io/natthasath-news/software/) |
| [`ratchakitcha/`](ratchakitcha/) | Weekly | Royal Gazette | [Open](https://natthasath.github.io/natthasath-news/ratchakitcha/) |
| [`sales/`](sales/) | Weekly | Sales & Promotions | [Open](https://natthasath.github.io/natthasath-news/sales/) |
| [`jobs-government/`](jobs-government/) | Weekly | Government Jobs | [Open](https://natthasath.github.io/natthasath-news/jobs-government/) |
| [`jobs-private/`](jobs-private/) | Weekly | Private Sector Jobs | [Open](https://natthasath.github.io/natthasath-news/jobs-private/) |
| [`f1/`](f1/) | Weekly | Formula 1 | [Open](https://natthasath.github.io/natthasath-news/f1/) |
| [`gov-projects/`](gov-projects/) | Weekly | Government Projects | [Open](https://natthasath.github.io/natthasath-news/gov-projects/) |

### 🚀 Setup

No build step or dependencies — pure static HTML. View it live at the links above, or preview locally with:

```shell
git clone https://github.com/natthasath/natthasath-news.git
cd natthasath-news
python -m http.server 8000
```

### 🏆 Usage

Open [https://natthasath.github.io/natthasath-news/](https://natthasath.github.io/natthasath-news/) as the landing page — pick a category from the grid. Each category has an archive page (`index.html`) linking to every report, newest first.

Report filenames follow the `{YYYY-MM-DD}-{slug}-report.html` pattern so they sort chronologically and same-run overwrites are easy to detect.

### 📜 License

This project is licensed under the MIT License.
