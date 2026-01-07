# GIV Theory Website

## Geometric Impedance of the Vacuum - A Cross-Scale Phenomenological Framework

This website houses the research and papers of K. T. Niedzwiecki on the GIV (Geometric Impedance of the Vacuum) theory.

## How to View the Website

### Method 1: Open Directly in Browser (Easiest!)

1. Navigate to the `GIV_Website` folder
2. Double-click `index.html`
3. It will open in your default web browser
4. Browse freely! All links work locally.

### Method 2: Using Python's Built-in Server

If you want a more "website-like" experience:

1. Open Anaconda PowerShell
2. Navigate to the website folder:
   ```
   cd GIV_Website
   ```
3. Start a local server:
   ```
   python -m http.server 8000
   ```
4. Open your browser and go to: `http://localhost:8000`
5. Press Ctrl+C in the terminal to stop the server when done

## Website Structure

```
GIV_Website/
├── index.html              # Home page - start here!
├── about.html              # About the researcher and method
│
├── framework/              # Core theoretical framework
│   └── index.html
│
├── applications/           # Applications across scales
│   ├── quantum-matter/
│   ├── particle-physics/   # Meson decay (Γ/m ∝ m^-3.71)
│   ├── cosmology/          # Temporal Echo, DDO 154 prediction
│   └── astrobiology/       # Homochirality via CISS
│
├── papers/                 # Published papers and preprints
│   └── index.html
│
└── css/                    # Styling (clean academic look)
    └── style.css
```

## Next Steps

### To Add Your PDFs:

1. Copy your PDF files from `GIV_Theory` folder to `GIV_Website/papers/`
2. The links in the Papers page already point to them!

### To Publish Online (Future):

#### Option A: GitHub Pages (Recommended - Free!)

1. Create a GitHub account (if you don't have one)
2. Create a new repository called `giv-theory`
3. Upload all the files from GIV_Website
4. Enable GitHub Pages in repository settings
5. Your site will be live at: `yourusername.github.io/giv-theory`

#### Option B: Custom Domain

1. Buy a domain (e.g., `giv-theory.org`)
2. Use GitHub Pages with custom domain, or
3. Use a hosting service like Netlify (also free for static sites)

## Customization

- **Colors:** Edit `css/style.css` - look for the `:root` section at the top
- **Content:** All pages are simple HTML - edit any text directly
- **Add pages:** Copy an existing page, modify content, add link in navigation

## Built With

- Pure HTML5 and CSS3
- No JavaScript required (works everywhere!)
- Clean academic styling
- Fully responsive (works on mobile too!)
- All content cross-referenced

---

**Created:** January 2026
**Theory Development:** K. T. Niedzwiecki with AI collaborators (Gemini, GPT-5, Kimi, Claude)
**Website Built:** Claude Code CLI

*"Life crystallizes along the grain of the vacuum. So does knowledge."*
