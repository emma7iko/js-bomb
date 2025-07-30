# 🧨 JavaScript Crawler Trap

This is a **HTML+JS-based crawler trap** designed to **overwhelm unethical or overly-aggressive crawlers** that scrape websites without consent. It uses deep DOM nesting and large in-memory attributes to consume RAM and CPU, potentially freezing or crashing headless browsers and bots.

> ⚠️ This is a **defensive tool**. It does not exploit any vulnerability, contains no malware, and does not attack any specific system. **Please use responsibly**. Do not attempt to hyperlink the page to any of the client accessible pages on your project. **Again, please use responsibly.**
---

## 💡 What It Does

- Creates tens of thousands of nested `<div>` elements
- Each `<div>` carries a massive `data-bomb` attribute (100MB+)
- Result: **browser/crawler memory exhaustion**

Real browsers may freeze with large settings. Headless crawlers using Puppeteer, Selenium, etc., will almost certainly crash.

---

## 📁 Files

- `index.html` – the main bomb page
- *(Optional)*: `generate_bomb.js` – for dynamic bomb generation (coming soon)

---

## 🚀 Getting Started

I strongly recommend using **google chrome** browser for this, use any other am not responsible for the aftermaths, you can serve it with **no dependencies**:

```bash
git clone https://github.com/emma7iko/js-bomb.git
cd bomb
python3 -m http.server 8080
