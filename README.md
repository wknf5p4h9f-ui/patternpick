# PatternPick – Web Scraper: Table & List to CSV/Excel

[![Chrome Web Store](https://img.shields.io/badge/Chrome%20Web%20Store-Install%20free-6d28d9?logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/dijbhfpcmdnhfigiaopepeaoagmehkhi)
![Price](https://img.shields.io/badge/price-free-16a34a)
![Data](https://img.shields.io/badge/data-100%25%20local-2563eb)

Turn any list, grid or table on a web page into a clean spreadsheet in three clicks — no code, no account, no cloud.
Every run ends with an **accuracy report**, so you know your data is complete before you use it.

**[➜ Install from the Chrome Web Store](https://chromewebstore.google.com/detail/dijbhfpcmdnhfigiaopepeaoagmehkhi)** · [Homepage](https://wknf5p4h9f-ui.github.io/patternpick/) · [Privacy policy](https://wknf5p4h9f-ui.github.io/patternpick/privacy.html)

---

## How it works

1. Open a page with a list, product grid or table and click the **PatternPick** icon.
2. Click **Auto-detect** — or **Pick fields** and click a title, price or image.
3. Choose how to collect:
   - **This page only** (it scrolls once so lazy-loaded items are included)
   - **Infinite scroll**
   - **Click a "Load more" / "Next" button**
   - **I'll scroll myself (live capture)** — for sites that only load more when a real person scrolls
4. **Download CSV**, **JSON**, or **Copy for Sheets** (paste into Google Sheets or Excel).

## Why PatternPick

| | |
|---|---|
| **Accuracy report** | Rows collected vs items seen, duplicates removed, empty items skipped, completeness of every column. Weak columns are flagged. |
| **Works where formulas give up** | `IMPORTHTML` / `IMPORTXML` and Power Query can't read data loaded with JavaScript. PatternPick reads what your browser actually shows. |
| **Clean columns** | Junk columns removed, readable names (title, price, rating…), full text when a site shortens it, split prices merged. |
| **Clean exports** | Absolute URLs, real image URLs (not lazy-load placeholders), UTF-8 that opens correctly in Excel, formula-injection protection. |
| **Privacy built in** | Emails and phone numbers are detected and masked on export by default. |
| **100% local** | No servers, no analytics, no sign-up, no remote code. Your data never leaves your browser. |
| **Polite** | At least 1 second between page loads, plus page and row limits. |

Available in English, 简体中文, 繁體中文, Bahasa Melayu, Bahasa Indonesia, Español and Português.

## FAQ

**Why does `IMPORTXML` / `IMPORTHTML` return `#N/A` or "Imported content is empty"?**
Those functions only read the page's initial HTML. Many sites load their lists afterwards with JavaScript (infinite scroll, "Load more", single-page apps), so the formula sees an empty page. PatternPick runs inside your browser and reads the page after it has loaded.

**Does PatternPick send my data anywhere?**
No. Everything runs in your browser. Collected rows are saved only in local extension storage so a reload doesn't lose your work; you can delete them from the Options page.

**What permissions does it use?**
`activeTab` and `scripting` (run only on the tab where you click the icon), `storage` and `unlimitedStorage` (save your progress locally). An optional host permission is requested only if you enable multi-page mode.

**Can I use it on any website?**
Use it on data you are permitted to collect. Respect each website's Terms of Service and privacy laws such as the PDPA and GDPR.

## Feedback & bug reports

Found a page where detection is wrong or rows are missing? [Open an issue](https://github.com/wknf5p4h9f-ui/patternpick/issues/new) with the page URL (if public), what you expected, and a screenshot of the accuracy report.
