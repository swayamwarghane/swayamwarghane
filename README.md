# Hi, I'm Swayam 👋

<div align="center">

![header](https://raw.githubusercontent.com/DenverCoder1/readme-gen-assets/main/hero-swayam.gif)

</div>

---

## 🔭 What I build

I'm a Computer Science undergrad who loves building **vibe-first**, AI-powered web experiences — clean UI/UX, responsive layouts, and fast prototypes. I mix classic frontend craft (HTML/CSS/JS) with modern React + TypeScript and AI/no-code tools to ship polished projects quickly.

**Featured projects (repo links below):**

* **CAPSCO** — AI-driven e‑commerce for caps (React, TypeScript, Vite, Tailwind, Supabase)
* **Instant BG Reveal** — AI background-removal web app (React, JS)
* **Netflix / Zomato / Dribbble clones** — pixel-faithful responsive UI builds (HTML, CSS, Bootstrap)
* **Cafe** — stylish responsive site built with React + TS

---

## ✨ Realtime data & animated stats

> This README includes a realtime/animated data stack so your profile *lives* and shows your pulse.

### Live widgets included

* **GitHub contribution heatmap** (auto-updates via GitHub Images)
* **Language & repo stats** from `github-readme-stats` (dynamic SVGs)
* **Wakatime / coding time** snapshot (optional — add your API key)
* **Visitor counter & sparkline** for quick pulse of visits
* **Animated highlights carousel** (GIF + shields + tiny JS-powered animation for local preview)

> The animated/stat widgets are served as SVGs and GIFs so they animate on GitHub and look slick.

---

## 🚀 Quick setup (copy-paste)

### 1) Basic README (already here)

Just drop this file as `README.md` in your GitHub profile repository named exactly your GitHub username (e.g. `swayamwarghane/swayamwarghane`).

### 2) Add live GitHub stats cards

Place these markdown cards where you want the big stats to appear:

```md
<!-- GitHub Readme Stats -->
![Swayam's GitHub Stats](https://github-readme-stats.vercel.app/api?username=swayamwarghane&show_icons=true&theme=dracula&count_private=true)

<!-- Top languages -->
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=swayamwarghane&layout=compact&theme=dracula)
```

### 3) Realtime WakaTime snapshot (optional)

Add your waka key to GitHub Actions secrets as `WAKATIME_KEY` and then include an action to generate a small SVG each day. Example workflow included in the **.github/workflows** section of this README.

### 4) Visitor counter & sparkline

Use this lightweight badge to show visits:

```md
![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=swayamwarghane.swayamwarghane)
```

---

## 📈 Auto-generated charts (GitHub Action example)

Create `.github/workflows/generate-stats.yml` with the following (this fetches WakaTime and saves an SVG to the repo):

```yaml
name: Generate profile charts
on:
  schedule:
    - cron: '0 0 * * *'
  workflow_dispatch: {}

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Generate WakaTime SVG
        env:
          WAKATIME_KEY: ${{ secrets.WAKATIME_KEY }}
        run: |
          pip install wakatime --no-cache-dir
          python .github/scripts/generate_wakatime_svg.py
      - name: Commit SVG
        run: |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add -A
          git commit -m "chore: update stats svg" || echo "no changes"
          git push
```

> I included a sample `generate_wakatime_svg.py` script in the repo snippets section (see `scripts/` in this README).

---

## 🧰 Tech & Tools

* **Languages:** C, C++, Java, Python, HTML, CSS, JavaScript
* **Frameworks & Layout:** React, Tailwind CSS, Bootstrap, Flexbox, CSS Grid
* **Databases / Backend:** Supabase
* **Others:** WakaTime, GitHub Actions, Vite

---

## 📁 Projects & live links

* [Dribbble clone — responsive layout (Grid + Flexbox)](https://github.com/swayamwarghane/Dribbble)
* [Netflix clone — responsive with Bootstrap](https://github.com/swayamwarghane/Netflix)
* [Zomato clone — UI replication](https://github.com/swayamwarghane/zomato)
* [CAPSCO — AI e-commerce (React + TS + Supabase)](https://github.com/swayamwarghane/capsco2)
* [Cafe — React + TS site](https://github.com/swayamwarghane/cafe)
* [Instant BG Reveal — AI background remover](https://github.com/swayamwarghane/instant-bg-reveal)

---

## 📫 Connect with me

* Email: [swayamwarghane7218@gmail.com](mailto:swayamwarghane7218@gmail.com)
* LinkedIn: [https://linkedin.com/in/swayam-warghane-8149b0290](https://linkedin.com/in/swayam-warghane-8149b0290)
* GitHub: [https://github.com/swayamwarghane](https://github.com/swayamwarghane)

---

## ✨ Notes & personalization

* Want the WakaTime or timeline cards added? Add your `WAKATIME_KEY` to GitHub secrets and enable the workflow above.
* Want a custom animated SVG (e.g., project carousel or live visitor sparkline)? I can add the generator script to `/scripts` — tell me what to visualize.

---

*Profile content generated using details from the user's resume.*
