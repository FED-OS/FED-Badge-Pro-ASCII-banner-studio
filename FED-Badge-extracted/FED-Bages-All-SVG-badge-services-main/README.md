# ⚡ FED‑Badge Pro

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/W3T61ZU5FS)

**One‑click badge studio for your GitHub README.**  
Generate badges from **Shields.io, Badgen, Badges.ws, BadgeWind, Raw SVG, and GitHub Actions** – all in one clean interface.

[![FED‑Badge](https://img.shields.io/badge/FED--Badge-v2.0-0052cc?style=flat&labelColor=24292e)](https://github.com/Fedpromptly/fed-badge)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

[![1787528795.png](https://s8d8.turboimg.net/sp/9d961d165fc5a9c79204ac24d6a9529f/1787528795.png)](https://www.turboimagehost.com/p/126958352/1787528795.png.html)

## ✨ Features

- **🎯 Preset library** – load popular badges instantly (GitHub Sponsors, Patreon, Ko‑fi, FED‑OS, etc.)
- **🔧 All badge services** – Shields.io, Badgen.net, Badges.ws, BadgeWind, Raw SVG, GitHub Actions
- **📋 One‑click copy** – copy HTML (works in GitHub READMEs) or standard Markdown
- **📦 Bulk export** – copy all badges at once (HTML or Markdown)
- **🎨 Live preview** – see your badge as you edit
- **📖 Built‑in docs** – quick reference for every service
- **🧩 Fully offline** – runs entirely in your browser, no server required

---

## 🚀 Quick Start

1. **Open** `index.html` in your browser.
2. **Pick a preset** or fill in your own label, message, and colours.
3. **Copy** the HTML or Markdown snippet from any badge card.
4. **Paste** into your `README.md` or website.

That’s it. No installation, no dependencies.

---

## 📸 Screenshots

*(Add your own screenshots here – the tool generates a clean dark‑themed UI.)*

---

## 📦 Services Supported

| Service | URL Pattern | Notes |
| :--- | :--- | :--- |
| **Shields.io** | `https://img.shields.io/badge/...` | Full parameter support (style, logo, label colour, cache, links). |
| **Badgen.net** | `https://badgen.net/badge/...` | Simple and fast. |
| **Badges.ws** | `https://badges.ws/badge/...` | Supports style via query. |
| **BadgeWind** | `https://badgewind.vercel.app/...` | Tailwind‑styled badges. |
| **Raw SVG** | Self‑contained `<svg>` | No external requests – works offline. |
| **GitHub Actions** | `https://github.com/owner/repo/actions/workflows/.../badge.svg` | Native workflow status. |

---

<svg xmlns="http://www.w3.org/2000/svg" width="110" height="20" role="img">
  ...
</svg>

[![FED-OS: Active](https://img.shields.io/badge/FED--OS-Active-0052cc?style=flat&labelColor=24292e)](https://fedpromptly.com)

## 🛠️ Usage Examples

### HTML (works in GitHub READMEs)
```html
<a href='https://fedpromptly.com' target='_blank'>
    <img height='36' style='border:0px;height:36px;' src='https://img.shields.io/badge/FED--OS-Active-0052cc?style=flat&labelColor=24292e' border='0' alt='FED-OS: Active' />
</a>

