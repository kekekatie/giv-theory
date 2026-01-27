# CLAUDE.md - AI Assistant Guide for GIV Theory Repository

## Project Overview

This repository contains the **Geometric Impedance of the Vacuum (GIV) Theory** website - an academic/research static website presenting independent theoretical physics research by K. T. Niedzwiecki.

**Purpose:** A phenomenological framework proposing that vacuum structure creates scale-dependent coupling impedance for physical processes, with applications spanning quantum matter, particle physics, cosmology, and astrobiology.

**Technology Stack:** Pure HTML5 and CSS3 static site (no JavaScript, no build system, no dependencies)

## Repository Structure

```
giv-theory/
├── index.html                    # Homepage - main entry point
├── about.html                    # About the researcher and methodology
├── CLAUDE.md                     # This file
├── README.md                     # User-facing documentation
│
├── css/
│   └── style.css                 # All styling (CSS variables in :root)
│
├── framework/
│   └── index.html                # Core theoretical framework explanation
│
├── applications/                 # Applications by physical scale
│   ├── index.html                # Applications overview page
│   ├── quantum-matter/
│   │   └── index.html            # E8 at quantum criticality (~10^-10 m)
│   ├── particle-physics/
│   │   └── index.html            # Meson decay scaling (~10^-15 m)
│   ├── cosmology/
│   │   └── index.html            # Temporal Echo model (~10^20 m)
│   └── astrobiology/
│       └── index.html            # CISS and homochirality (~10^-9 m)
│
├── papers/
│   ├── index.html                # Papers listing page
│   ├── Temporal_Echo_UDG_v1.pdf  # Most downloaded paper
│   ├── Cloud9_Discriminating_Test_Case.pdf
│   ├── Baryon_Decay_Paper.pdf
│   ├── Meson_Width_Scaling_v1.pdf
│   ├── Vector_Meson_Decay_Scaling.pdf
│   ├── Homochirality_CISS.pdf
│   └── Meson_Paper_Anonymous.pdf
│
├── images/                       # Figures and visualizations
│   ├── udg_zoo_cloud9.png        # UDG diversity plot with Cloud 9
│   ├── meson_scaling.png         # Vector meson decay power law
│   ├── chirality_ciss.png        # CISS effect diagram
│   ├── geometric_impedance_final.png
│   └── [other scientific figures]
│
├── drafts/                       # Work-in-progress papers (empty)
│   └── README.md
├── research-notes/               # Working notes (empty)
│   └── README.md
└── conversations/                # Key development discussions (empty)
    └── README.md
```

## Key Scientific Concepts

Understanding these concepts helps when editing content:

1. **Geometric Impedance** - Effective coupling resistance between physical processes and vacuum structure
2. **Temporal Echo** - Dark matter as accumulated gravitational wake with acceleration-dependent memory
3. **E8 Projection** - Higher-dimensional geometry projected to 4D, creating observable patterns
4. **Golden Ratio (φ)** - Appears in meson decay scaling exponent: Γ/m ∝ m^(-3.71), matching 1 + φ² = 3.618
5. **CISS (Chiral-Induced Spin Selectivity)** - Transport asymmetry explaining biological homochirality

## Development Workflow

### Local Preview

```bash
# Option 1: Open directly in browser
# Navigate to folder and double-click index.html

# Option 2: Python local server
cd /home/user/giv-theory
python -m http.server 8000
# Visit http://localhost:8000
```

### Making Changes

1. **HTML pages** - Edit directly; follow existing structure with header, nav, sections, footer
2. **Styling** - Modify `css/style.css`; use CSS variables from `:root` for consistency
3. **New papers** - Add PDF to `papers/` and update `papers/index.html`
4. **New images** - Add to `images/` directory; reference with relative paths

### Navigation Convention

All pages use consistent navigation bar:
- Home → Framework → Applications → Papers → About

Relative paths vary by depth:
- Root level: `href="framework/index.html"`
- One level deep: `href="../index.html"`
- Two levels deep: `href="../../index.html"`

## CSS Conventions

Key CSS classes from `css/style.css`:

| Class | Purpose |
|-------|---------|
| `.hero` | Gradient banner for page introductions |
| `.scale-card` | Card component with left blue border |
| `.key-result` | Yellow highlighted result box |
| `.equation` | Monospace code block for equations |
| `.paper-link` | Blue button-style link |
| `.branch-note` | Blue info box for work-in-progress notes |
| `.scale-size` | Monospace scale indicator (e.g., "10^-15 m") |

CSS Variables (in `:root`):
```css
--primary-color: #1a1a1a;
--secondary-color: #2c5aa0;  /* Main blue */
--accent-color: #4a90e2;
--background: #ffffff;
--text: #333333;
--light-gray: #f5f5f5;
--border: #dddddd;
```

## Content Guidelines

### Tone
- Academic but accessible
- Emphasize phenomenology over metaphysical claims
- Always state limitations and falsifiability
- Avoid overclaiming; this is independent research, not peer-reviewed

### Key Empirical Results to Reference
- DDO 154 rotation: 49 km/s predicted, 45-50 km/s observed (zero parameters)
- Meson decay: Γ/m ∝ m^(-3.71±0.15), R² = 0.98
- UDG correlation: Spearman ρ = 0.692, p = 0.0061
- CISS asymmetry: ~10^-4, 10^13 times stronger than parity violation

### Scientific Notation in HTML
Use `<sup>` tags for exponents: `10<sup>-15</sup>` renders as 10^-15

## Common Tasks

### Adding a New Paper
1. Place PDF in `papers/` directory
2. Edit `papers/index.html`:
   - Add new `<div class="scale-card">` block
   - Include title, author, date, description, key results, download link
3. Update any application pages that reference the paper

### Adding a New Application Section
1. Create directory under `applications/`
2. Create `index.html` following existing structure
3. Update `applications/index.html` with new card
4. Update main `index.html` if appropriate
5. Add navigation links

### Updating Figures
1. Add image to `images/` directory
2. Reference with appropriate relative path
3. Include `<figure>` or styled `<div>` with caption
4. Use `style="max-width: 100%"` for responsiveness

## Git Practices

- Commit messages should be descriptive of scientific content changes
- Recent commit history shows pattern: "Add [Paper Name] Paper", "Update [page] with [feature]"
- This is a public-facing research site; commits should be clean

## Important Notes for AI Assistants

1. **No JavaScript** - This is intentionally a pure HTML/CSS site for maximum compatibility
2. **Scientific accuracy** - Verify any physics claims; defer to existing content when uncertain
3. **Maintain humility** - The framework explicitly acknowledges limitations and untested regimes
4. **Preserve structure** - Follow existing HTML patterns and CSS classes
5. **Cross-references** - Many pages link to each other; check for broken links after changes
6. **PDF files** - Large binary files; avoid unnecessary modifications
7. **Mobile responsive** - Site has responsive CSS; test changes on mobile viewport

## Contact

- Author: K. T. Niedzwiecki
- Email: niedzkatie@gmail.com
- Location: South Australia

---

*"Life crystallizes along the grain of the vacuum. So does knowledge."*
