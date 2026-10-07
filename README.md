# Computer: Zero → Hero — installable app

Your computer-learning roadmap as a **real phone/desktop app**: home-screen icon, fullscreen, works offline, and saves progress on the device.

**304 topics · 18 stages · ~1,561 hours** — from "what is a mouse" to Python, SQL, AI, cloud, cyber security and job-ready projects.

Same engine as your maths app (so everything you already know works here), with a **new drill engine** built for computers: shortcuts, file types, IT terms, Excel formulas, scam-spotting, networking, command line, code and binary — plus a **1-minute typing test** with WPM tracking.

---

## What's inside

| File | What it is |
|---|---|
| `index.html` | The whole tracker: curriculum, drills, typing test, plan, notes + PWA shell |
| `pwa.js` / `pwa.css` | App layer: bottom nav, install flow, offline, backup to Drive |
| `manifest.webmanifest` | App name, icon, colours, fullscreen → installable |
| `sw.js` | Service worker → opens offline (cache `czh-app-v1`) |
| `icons/` | `>_` terminal icon in every size (incl. maskable) |
| `serve.py` | One-command local server (`python3 serve.py`) |
| `GITHUB-PAGES.md` | Publish it free on your own GitHub (permanent https link) |
| `../single-file/computer-zero-to-hero-app.html` | Everything in one file — easy to send on WhatsApp |

## The 18 stages

| # | Stage | Topics | What it covers |
|---|---|---|---|
| 0 | 🖥️ Absolute Beginner | 24 | The machine, mouse/keyboard, **typing**, windows, files, first real tasks |
| 1 | 🌐 Internet, Email & Everyday Online | 23 | Browsing, search, Gmail, Drive, **UPI & DigiLocker**, safety |
| 2 | 📝 Word Processing | 21 | Word/Docs: formatting, tables, **resume**, mail merge, PDF |
| 3 | 📊 Spreadsheets | 27 | Excel/Sheets: formulas, IF, VLOOKUP, pivot tables, dashboards |
| 4 | 📽️ Presentations | 12 | PowerPoint/Slides/Canva: story, design, delivering a talk |
| 5 | 🎨 Images, Video & Audio | 18 | Photos, Photopea/GIMP, CapCut, Audacity, compression |
| 6 | 🗂️ Files, Storage & Backups | 10 | File systems, 3-2-1 backups, recovery, encryption, zip/PDF |
| 7 | ⚙️ Operating Systems | 16 | Windows in depth, **Linux/Ubuntu**, macOS, Android/iOS, command line, VMs |
| 8 | 🧰 Hardware & Maintenance | 15 | Parts, buying advice, assembling, printers, BIOS, troubleshooting |
| 9 | 🛜 Networking & Wi-Fi | 12 | IP/DNS/DHCP, router setup, sharing, VPN, fixing connectivity |
| 10 | 🔐 Security, Privacy & Safety | 14 | Threats, password managers + 2FA, encryption, **Indian fraud defence**, audits |
| 11 | 🚀 Productivity & Digital Work | 12 | Notes, tasks, calendar, Workspace/365, PDFs, forms, **automation** |
| 12 | 🧠 Programming Foundations | 20 | Algorithmic thinking → **Python**, files, debugging, Git & GitHub |
| 13 | 🌍 Web Development | 15 | HTML, CSS, JS, responsiveness, APIs, **a live portfolio site** |
| 14 | 📈 Data, SQL & Analysis | 17 | Databases, **SQL**, pandas, Power BI/Tableau, stats |
| 15 | 🤖 AI & Modern Tools | 14 | How AI works, prompting, AI for study/work, agents, limits & ethics |
| 16 | 🏗️ Computer Science Core | 16 | Binary & gates, architecture, OS internals, **DSA, Big-O**, testing |
| 17 | ☁️ Cloud, Cyber, DevOps & Career | 18 | Linux power use, AWS/Azure, Docker, CI/CD, ethical hacking, mobile/game dev, **jobs & freelancing** |

Every topic has step-by-step tasks written for a real machine, a "mastered when" test you can't fake, and links to the exact free resource for that step.

## Install it on your phone

1. Publish it (see `GITHUB-PAGES.md`, or use the included `serve.py`), then open the link on your phone.
2. **Android/Chrome:** tap the **Install** button in the app → π… sorry, the **`>_` icon** lands on your home screen.
3. **iPhone/Safari:** Share □↑ → **Add to Home Screen** → Add.

Progress is stored on the device; **Settings → Save my progress** shows storage protection and last backup, with **Share backup → Drive/WhatsApp**.

## Verify the build

```bash
python3 build_computer_app.py        # rebuild from the curriculum source
python3 make_icons_computer.py       # rebuild icons
python3 build_single_computer.py     # one-file version
cd tests && node smoke_computer.mjs  # 41 assertions
```

The smoke test boots the real app in a DOM and checks: 18 stages / 304 topics load, all 10 drill banks generate questions, `Ctrl + C` is accepted for `ctrl+c`, quiz scoring works, the **typing test computes WPM and saves it**, flashcards build a 100+ card deck, the PWA shell + install cards render, progress saves to its **own storage key `czh.v1`** (so it can't collide with the maths app), and every installable asset exists.
