If this helped you, consider starring the repo ⭐

---

<div align="center">

# 🛡️ Server Hardening Guide · Archival Reference

**A beginner-friendly, copy-paste guide to secure your Linux server**

*Frost white · Golden accents · Bubblegum pink · Dark theme · Glassmorphism 2.0*

---

[![Live Guide](https://img.shields.io/badge/📖_Live_Guide-GitHub_Pages-gold?style=for-the-badge)](https://alexrabbit.github.io/server-hardening-guide/)
[![License](https://img.shields.io/badge/License-MIT-pink?style=for-the-badge)](LICENSE)

</div>

---

## 📌 What is this?

This repo is a **single-page reference** that walks you through securing a Linux server (Ubuntu/Debian) step by step. No jargon overload — everything is written so even someone who has never touched a server can follow.

```
┌─────────────────────────────────────────────────────────────┐
│  🔒 Your server (before)     →    🛡️ Your server (after)   │
│  • Default SSH port 22             • Custom SSH port        │
│  • No firewall                    • Firewall on            │
│  • Anyone can try to connect      • Only your IP allowed    │
│  • Unlimited login attempts       • Fail2ban + MaxAuthTries  │
└─────────────────────────────────────────────────────────────┘
```

**You get:**

- ✅ **01** — Update the system (like updating your phone)
- ✅ **02** — Change the SSH port (so bots can’t find the “door”)
- ✅ **03** — Turn on the firewall (the bouncer)
- ✅ **04** — Only allow your IP to SSH (guest list)
- ✅ **05** — Install Fail2ban (auto-block brute force)
- ✅ **06** — Limit wrong password attempts (MaxAuthTries)

Every command is in a **click-to-copy** box. Replace the pink placeholders with your real values and you’re good to go.

---

## 🌐 Live guide (GitHub Pages)

Once this repo is on GitHub and GitHub Pages is enabled, the guide lives at:

**https://alexrabbit.github.io/server-hardening-guide/**

*(Replace `server-hardening-guide` with your actual repo name if different.)*

---

## 🚀 Quick start (use the guide locally)

1. **Clone or download** this repo.
2. **Open `index.html`** in your browser (double-click or drag into Chrome/Brave/Firefox).
3. **Follow the 6 steps** on the page. Click any gray code block to copy the command.
4. **Replace placeholders** before running anything:
   - `YOUR_SERVER_IP` → your server’s IP address  
   - `YOUR_PORT` → the SSH port you chose (e.g. `22022`)  
   - `YOUR_PUBLIC_IP` → your home/office public IP (e.g. from `curl -s ifconfig.me`)

That’s it. No build step, no npm, no server — just static HTML/CSS/JS.

---

## 📦 Deploy to GitHub Pages (drag & drop)

You can host the guide for free on GitHub Pages so others can use it too.

### Option A — Deploy from a branch (recommended)

1. **Push this repo** to GitHub (e.g. `https://github.com/AlexRabbit/server-hardening-guide`).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** (or **master**) and folder **/ (root)**.
5. Click **Save**. In a minute or two your site will be at  
   `https://<username>.github.io/<repo-name>/`.

Because **`index.html`** is in the root, visiting that URL will show the guide.

### Option B — Drag & drop (static upload)

1. **Zip the folder** that contains **only** `index.html` (and optionally `README.md`, `LICENSE` — the site only needs `index.html`).
2. In your repo, go to **Settings → Pages**.
3. If your provider supports it: **drag and drop the zip** into the deployment area.  
   *(Note: Classic “drag and drop” deploy is often per-branch; if you don’t see it, use Option A.)*

Either way, the result is the same: the guide is live and shareable.

---

## 📂 Repo structure

```
server-hardening-guide/
├── index.html          ← The guide (single file, no dependencies)
├── server-hardening-guide.html   ← Same content (alternate name)
├── README.md           ← This file
└── LICENSE             ← MIT (optional)
```

**No build, no install.** Just open `index.html` or deploy the repo to GitHub Pages.

---

## 🎨 Design (Glassmorphism 2.0)

The guide page uses:

| Element | Description |
|--------|-------------|
| 🌙 **Dark theme** | Deep background so the content stands out |
| ✨ **Frost white** | Primary text and code blocks |
| 🏆 **Golden accents** | Step numbers and links |
| 💗 **Bubblegum pink** | Labels, placeholders, and “Copied!” feedback |
| 🫧 **Glassmorphism 2.0** | Frosted glass cards with blur and soft borders |
| 🫧 **Floating bubbles** | Subtle animated background shapes |
| 📜 **Editorial layout** | Numbered steps, clear hierarchy, easy to scan |

So the README matches the product: dark, structured, with a touch of gold and pink.

---

## 🔑 Placeholders cheat sheet

Before you run any command from the guide, replace these with your real values:

| Placeholder | Meaning | Example |
|-------------|---------|---------|
| `YOUR_SERVER_IP` | The public IP of your Linux server | `203.0.113.10` |
| `YOUR_PORT` | The SSH port you chose (not 22) | `22022` |
| `YOUR_PUBLIC_IP` | Your home/office IP (what the internet sees) | Run `curl -s ifconfig.me` on your PC |

⚠️ **Important:** Use your **public** IP for `YOUR_PUBLIC_IP`, not a `192.168.x.x` address (that’s only inside your network). If your home IP changes, update `hosts.allow` and fail2ban’s `ignoreip` or you may lock yourself out. Always keep **web console** or **recovery** access to the server.

---

## 🛠️ Tech stack

- **HTML5** — Semantic structure, one page
- **CSS3** — Variables, flexbox, backdrop-filter (glass), keyframe animations
- **Vanilla JS** — Click-to-copy only; no frameworks
- **No external deps** — No CDN, no fonts from the internet (system fonts only)

Fast, simple, and works offline once the page is loaded.

---

## 📜 License

This project is open source. Use it, share it, adapt it. If you keep attribution, that’s appreciated.

---

## 👤 Author & attribution

**AlexRabbit**

- 🔗 **GitHub:** [https://github.com/AlexRabbit](https://github.com/AlexRabbit)

If you use this guide or this repo in a project, a link back or a “based on Server Hardening Guide by AlexRabbit” is cool — not required, but nice.

---

<div align="center">

**If this helped you, consider starring the repo ⭐**

*Stay safe. Harden your servers.*

</div>
