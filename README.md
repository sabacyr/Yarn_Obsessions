# 🌙 Kamva Cove
### Saba's Knitting & Crochet Diaries
 
A Sailor Moon-inspired pixel art website for tracking knitting and crochet projects, browsing patterns, managing your yarn stash, and accessing craft tools — all in one place. Built for GitHub Pages.
 
---
 
## 📁 Repo Structure
 
```
your-repo/
├── index.html                          ← The entire site (one file!)
├── README.md                           ← This file
├── Kamva Cove Night Mode.png   ← Hero art (night)
├── Kamva Cove Day Mode.png     ← Hero art (day)
├── Bear Knit.png                       ← Bear the knit guardian
├── Rosie Crochet.png                   ← Rosie the crochet guardian
├── Mimi Stash.png                      ← Mimi the stash guardian
├── Knit/                               ← Your knitting PDF patterns
│   ├── pattern-name.pdf
│   └── ...
├── Crochet/                            ← Your crochet PDF patterns
│   ├── pattern-name.pdf
│   └── ...
└── photos/                             ← Your finished object photos
    ├── project-name.jpg
    └── ...
```
 
---
 
## 🚀 GitHub Pages Setup
 
1. Push all files to a GitHub repository
2. Go to **Settings → Pages**
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch, **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/repo-name/` within a minute or two
---
 
## ✏️ How to Edit Content
 
All content lives inside the `<script>` section near the bottom of `index.html`. Look for the clearly labelled arrays.
 
### Adding / Editing Projects
 
Find the `projects` array and add or edit entries:
 
```js
{
  name: "Project Name",
  craft: "knit",          // "knit" or "crochet"
  pattern: "Designer - Pattern Name",
  yarn: "Brand Yarn Name",
  status: "finished",     // "finished", "wip", "frogged", "trashed", "future"
  rating: 5,              // 1–5, or 0 for no rating
  notes: "Your notes here!"
}
```
 
### Adding / Editing Yarn Stash
 
Find the `stash` array:
 
```js
{
  brand: "Lion Brand",
  name: "24/7 Cotton",
  colorway: "Red",
  yardage: "186/100",
  weight: "Worsted (4)",
  fiber: "Cotton",
  skeins: "2/2",
  store: "Joann",
  color: "#CC3030"        // hex colour for the little swatch dot
}
```
 
### Adding Tutorials
 
Find the `tutorials` array and fill in the placeholder titles and creators:
 
```js
{
  title: "Your Video Title Here",
  creator: "Channel Name",
  tag: "knit",            // "knit", "crochet", or "general"
  url: "https://www.youtube.com/watch?v=..."
}
```
 
Thumbnails are pulled automatically from YouTube — no extra files needed!
 
### Adding Gallery Photos
 
1. Create a `photos/` folder in your repo
2. Upload your finished object images (jpg, png, webp)
3. Find the `galleryPhotos` array in `index.html` and add entries:
```js
{
  src: "photos/fox-plushie.jpg",
  title: "Fox Plushie",
  tag: "crochet"           // "knit" or "crochet"
}
```
 
### Linking PDF Patterns
 
Place PDFs in the `Knit/` or `Crochet/` folder. To make a pattern in the Pattern Vault clickable, add a `patternUrl` field to the matching project in the `projects` array:
 
```js
{
  name: "Purple Rain Balaclava",
  patternUrl: "Knit/Goyo-Balaclava.pdf",
  ...
}
```
 
---
 
## 🎨 Tabs Overview
 
| Tab | What's in it |
|---|---|
| **Home** | Hero art, stats, quick navigation |
| **Project Log** | All projects with search & filters |
| **Pattern Vault** | Searchable list of all referenced patterns |
| **Yarn Stash** | Full yarn inventory table |
| **Quest Board** | Future / queued projects |
| **Gallery** | Finished object photo grid |
| **Tools** | Gauge calc, row counter, needle converter & more |
| **Tutorials** | Clickable YouTube tutorial cards with search |
 
---
 
## 🐱 Cat Guardians
 
| Cat | Page | Role |
|---|---|---|
| Bear | Project Log | Knit Guardian 🩶 |
| Rosie | Pattern Vault | Crochet Guardian 🤎 |
| Mimi | Yarn Stash | Stash Guardian 🧡 |
 
---
 
## 🌙 Day / Night Mode
 
Click the toggle in the top-right corner of the nav bar to switch between night mode (deep midnight purple) and day mode (soft blush & champagne). The hero artwork swaps automatically.
 
---
 
*Made by Saba Cyr with Claude AI ✦*
