# Michaelis-Menten Kinetics and Inhibition

## Description

This Michaelis-Menten Kinetics and Inhibition notebook is a tool designed for the Biochemistry Lab to analyze enzyme kinetics data using the Michaelis-Menten model. It allows students to input their experimental data and generate kinetics curves with fitted parameters. The calculator is specifically designed to run in Google Colab.

## Features

- Support for three types of enzyme kinetics experiments
- User-friendly interface for data input via text area
- Automatic data processing and curve fitting
- Generation of publication-quality plots for each experiment type:
  - Michaelis-Menten curves for MM-Kinetics
  - Inhibition curves for MM-Inhibition
  - Multiple kinetics curves for different inhibitor concentrations in MM-Inhibition-Week2
- Calculation of key kinetic parameters:
  - Vmax and Km for MM-Kinetics
  - IC50 for MM-Inhibition
  - Comparative Vmax and Km values for different inhibitor concentrations in MM-Inhibition-Week2
- Support for multiple inhibitor concentration datasets in MM-Inhibition-Week2 (α1, α2, α3, α4)
- Clear visualization of data points and fitted curves
- Display of calculated parameters alongside the plots
- Designed for use in Google Colab, ensuring accessibility and ease of use

## Usage

1. Open the notebook in Google Colab
2. Run all cells to initialize the calculator
3. Select the experiment type from the dropdown menu. There are three options:
   - MM-Kinetics: Standard Michaelis-Menten kinetics experiment
   - MM-Inhibition: Enzyme inhibition kinetics experiment
   - MM-Inhibition-Week2: Extended enzyme inhibition kinetics experiment
4. Input your data in the provided text area
   - Ensure your data is in tab-separated format with headers
   - For all experiments: First column should be substrate concentration, second column should be reaction rate or velocity
5. Click the "Plot Data" button to generate the appropriate kinetics curve
6. Analyze the resulting graph and calculated parameters

### Experiment Descriptions

1. MM-Kinetics (Michaelis-Menten Kinetics):
   Determines the basic kinetic parameters of an enzyme-catalyzed reaction. It measures the initial reaction rate at various substrate concentrations to calculate Vmax and Km.

2. MM-Inhibition (Enzyme Inhibition Kinetics):
   Investigates the effect of inhibitors on enzyme activity. Measures percent inhibition at various inhibitor concentrations to determine IC50 and assess inhibitor potency.

3. MM-Inhibition-Week2 (Extended Enzyme Inhibition Kinetics):
   Comparison of enzyme kinetics under different inhibition conditions. It measures reaction rates at different substrate concentrations for multiple inhibitor concentrations (α1, α2, α3, α4).

## Requirements

- Google Colab environment
- Required Python libraries (automatically imported in Colab):
  - pandas
  - numpy
  - matplotlib
  - scipy
  - ipywidgets

## Contributing

This project is primarily for educational use in the Biochemistry Lab. However, if you have suggestions for improvements or bug fixes, please open an issue or submit a pull request.

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for the full license text.

## Citation and Attribution

While the Apache License 2.0 does not mandate attribution, I kindly request that you cite this project if you use it in your research or applications. This acknowledgment helps others discover the tool and recognizes the effort invested in its development.

### How to Cite

If you use this Protein Refolding Kinetics Calculator in your work, please cite it as follows:

Nicholas A. Lang. (2024). Protein Refolding Kinetics Calculator. GitHub. https://github.com/nicolang1/Michaelis-Menten-Kinetics

Thank you for supporting open-source development by providing attribution!

## Disclaimer

This tool is provided as-is, without any warranties. Users should verify calculations independently for critical applications.

## Acknowledgments

This tool was created to assist students in the Biochemistry Lab course. Special thanks to the course instructors and students for their feedback and suggestions.
