# Michaelis-Menten Kinetics & Inhibition Analyzer

## Description

The Michaelis-Menten Kinetics & Inhibition Analyzer is a browser-based tool designed for the Biochemistry Lab to analyze enzyme kinetics data using the Michaelis-Menten model. The tool allows students to input their experimental data via direct copy-and-paste and automatically generates kinetics curves with fitted parameters. The analyzer is built as a standalone HTML file and can be run directly in any modern web browser - no installation or coding environment required.

This tool is hosted online for student access outside of the lab and is designed to work with data exported from **Thermo Fisher Vision Lite** spectrophotometer software.

---

## Features

- Fully browser-based - no installation required
- Direct copy-and-paste support from Vision Lite or Microsoft Excel
- Sample names used as concentrations are automatically parsed and ready to use
- Support for three types of enzyme kinetics experiments
- Automatic data processing and curve fitting
- Interactive, publication-quality plots powered by Plotly
- Customizable graph and axis settings for each experiment type
- Calculation of key kinetic parameters:
  - Vmax and Km for Michaelis-Menten Kinetics
  - IC50 for Michaelis-Menten Inhibition
  - Comparative Vmax and Km values across inhibitor concentrations for MM-Inhibition (α's)
- Support for replicate averaging
- Load example data for quick reference
- Can be run offline after the initial internet connection loads Plotly (see [Requirements](#requirements))

---

## Experiment Types

### 1. Michaelis-Menten Kinetics
Determines the basic kinetic parameters of an enzyme-catalyzed reaction. Accepts either:
- **Raw Kinetic Data (Absorbance vs. Time):** Paste directly from Vision Lite or Excel. Row 1 should contain substrate concentrations. The app calculates slopes (velocities) automatically.
- **Pre-calculated Velocities:** Two-column format — substrate concentration and reaction velocity.

Outputs Vmax and Km from a fitted Michaelis-Menten curve.

### 2. Michaelis-Menten Inhibition — % Inhibition & IC50
Investigates the effect of inhibitors on enzyme activity. Two sub-sections:
- **Raw Absorbance vs. Time:** Paste data with inhibitor names in Row 1. Generates a raw absorbance plot and a velocity table.
- **% Inhibition & IC50:** Row 1 contains inhibitor concentrations. The app calculates slopes, percent inhibition, and fits an IC50 curve.

### 3. Michaelis-Menten Inhibition — α's (Extended Inhibition Kinetics)
Compares enzyme kinetics under different inhibitor concentrations. Each α dataset (α1–α4) accepts raw absorbance values vs. Time data with substrate concentrations in Row 1. At minimum, α1 is required. Outputs overlaid Michaelis-Menten curves and a comparison of Vmax and Km across conditions.

---

## Data Input Format

Data can be copied and pasted directly from **Thermo Fisher Vision Lite** or **Microsoft Excel** (tab-separated format). Saving your data in Excel first is recommended for easier organization and reuse.

**General format for raw kinetic data:**
```
Row 1: [blank] | conc1 | conc2 | ...   ← substrate or inhibitor concentrations
Row 2: [blank] | label | ...           ← optional label row
Row 3: min     | A     | ...           ← column headers
Row 4+: time   | Absorbance values ...       ← raw absorbance data
```

> **Note:** If sample names in Vision Lite are set to the concentration values, they will be automatically recognized and used directly by the analyzer.

---

## Usage

1. **Open the HTML file** in a modern web browser (Google Chrome recommended).
2. **Select the experiment type** from the tab menu:
   - Kinetics
   - Inhibition – % inhibition and IC50
   - Inhibition – α's
3. **Paste your data** into the provided text area (from Vision Lite or Excel).
4. **Adjust graph settings** (optional) using the settings panel — customize plot titles, axis labels, velocity/concentration units, and time range.
5. **Click the appropriate action button** (e.g., "Plot & Fit," "Fit IC50," or "Compare Curves") to generate results.
6. **Review the output** — interactive plots and calculated parameters will appear below the input panel.

---

## Requirements

### Browser
- A modern web browser is required (Google Chrome is recommended).
- **Internet connection:** An internet connection is needed the **first time** you open the file so that the browser can load the [Plotly](https://plotly.com/javascript/) graphing library. After the initial load, the file may work offline depending on your browser's cache behavior. If Chrome's cache is cleared or the browser is restarted, an internet connection may be required again to reload Plotly.

### Hosting (Optional)
- The HTML file can be hosted on any standard static web hosting platform.
- This tool is currently hosted via **[Netlify](https://www.netlify.com/)** (free tier), which is more than sufficient for approximately 120 students. *(Not sponsored.)*
- Students can access the hosted version directly through their browser without downloading any files.

---

## Contributing

This project is primarily for educational use in the Biochemistry Lab. If you have suggestions for improvements or bug fixes, please open an issue or submit a pull request.

---

## License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for the full license text.

---

## Citation and Attribution

While the Apache License 2.0 does not mandate attribution, I kindly request that you cite this project if you use it in your research or teaching. This helps others discover the tool and recognizes the effort invested in its development.

### How to Cite

> Nicholas A. Lang. (2024). Michaelis-Menten Kinetics & Inhibition Analyzer. GitHub. https://github.com/nicolang1/Michaelis-Menten-Kinetics

---

## Disclaimer

This tool is provided as-is, without any warranties. Users should verify calculations independently for critical applications.

---

## Acknowledgments

This tool was created to assist students in the Biochemistry Lab course at the University of Utah, Department of Chemistry. Special thanks to the course instructors and students for their continued feedback and suggestions.
