# OSINT Navigator

A lightning-fast, privacy-first Open Source Intelligence (OSINT) dashboard made for threat hunters, SOC analysts, and digital investigators. OSINT Navigator lets you investigate IPs, domains, URLs, hashes, emails, and more—across 100+ open-source tools, all from one modern, beautifully designed interface.

---

## ✨ Features

* 🔎 **Universal Search Bar:** Instantly query multiple OSINT tools with a single input (IP, domain, hash, email, or keyword)
* 🎯 **Rich Categories:** Over 20 categories including IP Info, Threat Intelligence, Hash Lookup, Email, Malware Analysis, Attack Surface, CVEs, Social Media, AI Tools, and more
* 🏷️ **Tag-based Filtering:** Dynamically filter tools by keyword, tag, or description
* 🧩 **Collapsible Categories:** Easily expand/collapse sections; favorites and search tools stay pinned
* 💡 **Interactive Tooltips:** Hover to get descriptions and tips for every tool and feature
* 🌗 **Auto Dark/Light Mode:** Modern theme toggle for all environments
* ⚡ **Super Fast & Fully Client-side:** No backend, no tracking, 100% privacy
* 🧠 **AI Assistant:** Integrated Chatbot assistant (top-right 🤖 button) for instant OSINT questions and workflow help
* 🔥 **Drag & Drop:** Reorder your favorite tools and categories—customize your workspace
* 🛠️ **Extensible:** Add or edit tools easily by updating the categories JSON in the HTML file

---

## 🚀 How to Use

1. **Open** `index.html` (or `LAST.html`) in your browser
2. **Type** an IP, domain, URL, hash, email, or keyword into the main search bar
3. **Click ADD** to auto-update links in all relevant tools
4. **Filter** by tool name, tags, or category
5. **Expand/collapse** categories for focused investigations
6. **Click** any tool card to open in a new tab
7. **Use the AI Assistant** (🤖 button) for tips, explanations, or threat hunting help

> **Note:** Some tools (marked with `skipSearch: true` or 🔶) work standalone and do not reflect dashboard search queries.

---

## 🧩 Example Use Cases

* Investigate suspicious IPs or domains with 50+ threat intel feeds
* Enrich indicators with WHOIS, GeoIP, reverse DNS, malware analysis, and more
* Perform passive recon with open DNS, SSL, and certificate tools
* Detect data breaches and leaks by checking email/username in breach databases
* Pivot between categories—attack surface, vulnerabilities, social media, and AI recon
* Get instant guidance or workflow help from the built-in AI assistant

---

## 🧼 Reset Layout (For New Tools or Categories)

If you add new tools or categories and they don’t show up, clear your local layout:

1. Open DevTools → Console (`F12`)
2. Paste:

   ```js
   localStorage.removeItem("osintToolOrder");
   ```
3. Refresh the page (Ctrl+Shift+R)

*The dashboard uses a versioning system (`toolConfigVersion`)—layout updates automatically when new versions are detected!*

---

## 🧩 OSINT Navigator Chrome Extension

**[🛒 Chrome Extension — Install on Chrome Web Store](https://chromewebstore.google.com/detail/osint-navigator/bejlkjkhhlbepgecabbjopdjkelfjnim?utm_source=item-share-cb)**
- [🔌 Explore the PLUGINS directory for extra integrations and tools](https://github.com/ekky19/osint/tree/main/PLUGINS)

Right-click any IP, domain, URL, or hash in Chrome and send it straight to OSINT Navigator.

### 🚀 Features

* 🔎 Right-click → investigate any observable in OSINT Navigator
* ⚡ No config, just works
* 🌐 Supports IPs, domains, hashes, URLs
* 🛡 100% client-side, privacy safe

#### 🛠 Installation (Manual)

1. Download or clone this repo : - (https://github.com/ekky19/osint/tree/main/PLUGINS)
2. Open Chrome, go to `chrome://extensions/`
3. Enable **Developer Mode**
4. Click **Load unpacked** and select the extension folder (`manifest.json`, `background.js`, `icon.png`)
5. **Done!** Right-click on any observable → OSINT Navigator

*The OSINT Favorites Chrome Extension version will also auto-trigger all links under “YOUR FAVORITES.”*

---

🐞 Known Issues
Adding a tool card to Favorites while filter is active may cause Favorites to display incorrectly or lose the newly added item.

Workaround: Clear the filter before adding tools to Favorites to avoid this bug.

This issue will be fixed in the next version!

---

## 👨‍💻 Credits

🛡️ Made for defenders, by [Ekrem O.](https://github.com/ekky19)

---

## 🛡 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license.

* **Share** — copy and redistribute the material
* **Adapt** — remix, transform, and build upon the material
  **Under these terms:**
* **Attribution** — credit the author with a link
* **NonCommercial** — you may not use for commercial purposes without permission

> For commercial use, [contact me](mailto:your@email.com) for licensing inquiries.

[🔗 View Full License](https://creativecommons.org/licenses/by-nc/4.0/)

---
