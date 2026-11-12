---
title: Cheminformatics Virtual Laboratory
emoji: ⚗️
colorFrom: green
colorTo: blue
sdk: static
app_file: index.html
pinned: false
---

# Cheminformatics Virtual Laboratory

An interactive, browser-based learning environment for exploring cheminformatics concepts, molecular structures, and molecular-property descriptors.

## Features

- Seven workspaces: Overview & Hub, Theory & Concepts, 2D/3D Molecular Studio, Descriptor & Property Lab, Multi-Molecule Comparison, Knowledge Assessment, and Final Dossier Generator.
- Built-in reference molecules with bundled structural and property data.
- Lightweight SMILES input handling and schematic 2D structure rendering.
- Interactive molecular visualization with 3Dmol.js.
- Descriptor comparison charts with Chart.js.
- CSV exports and downloadable PDF summaries using jsPDF and jsPDF-AutoTable.
- Responsive interface styled with Tailwind CSS.

## Important scientific scope and limitations

This Space serves a standalone HTML/JavaScript application. It does **not** run Python or RDKit, and it does not perform full cheminformatics parsing or force-field calculations.

For built-in reference molecules, the app displays molecular data and 3D coordinates bundled in the page. For custom SMILES input, it applies lightweight syntax checks, simplified atom/bond handling, heuristic descriptor estimates, and schematic 2D/3D coordinate layouts. These custom-input outputs are exploratory demonstrations, not validated molecular calculations or physically optimized conformers. In particular, the app does not execute ETKDG or MMFF94.

Do not use the calculated or estimated outputs as experimental, clinical, regulatory, or publication-grade results. For robust calculations on arbitrary molecules, connect the interface to a cheminformatics backend such as RDKit.

## Browser dependencies

The page loads the following resources from public CDNs:

- Tailwind CSS
- Google Fonts (Inter and JetBrains Mono)
- 3Dmol.js
- Chart.js
- jsPDF
- jsPDF-AutoTable

A working internet connection is required for these CDN-hosted libraries and fonts. No Python packages or `requirements.txt` are needed for this Static Space.

## Run locally

Open `index.html` in a modern browser, or start a local static server from this directory:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy to Hugging Face Spaces

1. Create a new Space at <https://huggingface.co/new-space>.
2. Select **Static** as the Space SDK.
3. Upload `index.html` and this `README.md` to the repository root. Keep any existing `.gitignore` and `.gitattributes` files.
4. Commit the changes and wait for the Space to update.

## Repository files

```text
.
├── index.html
├── README.md
├── .gitignore
└── .gitattributes
```

## Authors

**KOLAN MAASIRI REDDY** and **SEEMA E**  
SRM Institute of Science and Technology, Tiruchirappalli  
School of Sciences, Division of Chemistry

## License

No license was specified in the supplied source. Add a `LICENSE` file before granting public reuse rights.
