# PD Checker — Permitted Development Decision Tool

An interactive, single-page tool for checking whether a proposed rear extension qualifies as permitted development (PD) under Class A of the GPDO 2015 (England).

Built for **Steve Hunt Partnership** as a lightweight, dependency-free static web tool.

---

## Project details

| | |
|---|---|
| **Local path** | `C:\Users\GaryHunt\Claude\Code Projects\SHP\pd-checker\` |
| **GitHub repo** | https://github.com/gazappdev/pdchecker |
| **GitHub Pages URL** | https://gazappdev.github.io/pdchecker |
| **Legislative reference** | GPDO 2015, Schedule 2, Part 1, Class A |

---

## What it does

Steps the user through the Class A decision tree for a rear single-storey (or two-storey) extension, asking one question at a time. At each step it shows:

- The relevant planning question
- The legislative reference (GPDO 2015 clause)
- A guidance note with practical context
- YES / NO buttons, and a BACK button from step 2 onwards
- A running answer trail showing all previous answers

Outcomes:

- **PASS** — Likely permitted development, with a checklist of recommended next steps (LDC advice)
- **WARN** — Prior Approval required via the Neighbour Consultation Scheme (larger home extension)
- **FAIL** — Not permitted development, with a specific reason and recommended next step (full planning application, LBC, etc.)

---

## Technical notes

- Single file: `index.html` — all HTML, CSS, and JavaScript inline
- No frameworks, no npm packages, no build step
- Google Fonts loaded via CDN (Outfit + DM Sans)
- Works offline except for font loading (system font fallback applies)
- Fully static — serves from any web server or GitHub Pages

---

## Enabling GitHub Pages

1. Go to the repo: https://github.com/gazappdev/pdchecker
2. **Settings → Pages**
3. Under *Source*, select: **Deploy from a branch**
4. Branch: `main` · Folder: `/ (root)`
5. Save — the site will be live at https://gazappdev.github.io/pdchecker within ~60 seconds

---

## Update workflow

```
# Edit index.html locally, then:
git add index.html
git commit -m "describe change"
git push
# Live at https://gazappdev.github.io/pdchecker within ~60 seconds
```

---

## Future tabs (planned)

| Tab | Class | Status |
|---|---|---|
| Rear extension | Class A | ✓ Live |
| Side extension | Class A (side wall rules) | Stub — coming soon |
| Loft conversion | Class B | Stub — coming soon |
| Outbuilding | Class E | Stub — coming soon |
| Front extension / porch | Class C / D | Stub — coming soon |

---

## Disclaimer

This tool is provided for guidance only and does not constitute planning advice. Always verify against current legislation, consult the relevant Local Planning Authority, and consider obtaining a Lawful Development Certificate (LDC) before commencing works.
