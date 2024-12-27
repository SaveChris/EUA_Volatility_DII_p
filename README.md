# Supplementary material for the paper "Non-parametric Causal Discovery of EUA Market Returns through the Information Imbalance" by C. Salvagnin, V. Del Tatto, M.E. De Giuli, A. Mira, and  A. Glielmo.
This repository contains the supplementary material for the paper *"Non-parametric Causal Discovery of EUA Market Returns through the Information Imbalance"* by C. Salvagnin,V. Del Tatto, M.E. De Giuli, A. Mira, and A. Glielmo.

---

## Overview
This study examines the financial returns of the European Union Emissions Trading System (EU ETS) using data from January 2013 to 2024. We propose to use a recently introduced non-parametric tool from the physics literature named **Differentiable Information Imbalance (DII)** to identify variables that are causally related to EU ETS returns. The DII approach is compared with well-known linear approaches based on **VAR models** and **Granger causality**.

We find significant overlap among the causal variables identified by both linear and non-linear methods, such as **Coal Futures** and the **IBEX35 index**, but also observe important differences. These differences could stem from the limitations of the linear methodology but require further investigation to be fully understood. 

The study provides valuable insights for enhancing causal discovery in financial and energy markets, providing potential implications for asset pricing, risk management, and policy decision-making.

---

## Table of contents
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [SRC](#src)
  - [Data](#data)
- [Contributing](#contributing)
- [License](#license)

---

## Getting started

### Prerequisites
Before you begin, ensure you have met the following requirements:
Before you begin, ensure you have met the following requirements:
- [Python](https://www.python.org/) = 3.12.0  
- [pandas](https://pandas.pydata.org/) = 1.5.3  
- [numpy](https://numpy.org/) = 1.24.0  
- [matplotlib](https://matplotlib.org/) = 3.6.3  
- [seaborn](https://seaborn.pydata.org/) = 0.11.2  
- [scipy](https://www.scipy.org/) = 1.9.3  
- [statsmodels](https://www.statsmodels.org/stable/index.html) = 0.13.5  
- [pickle](https://docs.python.org/3/library/pickle.html) = 4.0
- [jinja2](https://jinja.palletsprojects.com/en/latest/) = 3.1.4  


### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/SaveChris/EUA_Volatility_DII_p.git
   cd EUA_Volatility_DII_p

2. **Navigate to the project directory:**

   ```bash
   cd EUA_Volatility_DII_p
   ```

3. **Create a virtual environment:**

   ```bash
   python3 -m venv venv
   ```
   **Activate the virtual environment:**
    - On Windows:
        ```bash
        venv\Scripts\activate
        ```
    - On Unix or MacOS:
        ```bash
        source venv/bin/activate
        ```

4. **Install the required packages:**

   ```bash
   pip install -r requirements.txt
   ```
This command installs all the necessary packages to run the code specified in **'requirements.txt'** file.

5. **Congratulations!**
Your project should now be up and running!

Adjust the steps and commands based on your project's specific requirements. If your project involves a different language or tool, you may need to tailor the installation instructions accordingly. Additionally, providing clear and concise instructions with helpful comments can significantly enhance the user experience. If you run into some problems or you have any questions contact me [(Cristiano Salvagnin)](mailto:cristiano.salvagnin@gmail.com), or [Aldo Glielmo](mailto:aldo.glielmo@gmail.com).

## Usage
This work is based on Jupiter notebooks, the user can find, for each section of the paper the corresponding notebook. The user can run the notebook to reproduce the results of the paper.

### SRC
The [SRC](https://github.com/SaveChris/EUA_Volatility_DII_p/tree/main/SRC) section is organized as follows:
- **'Sec1_Introduction.ipynb'** contains the code to reproduce the results obtained in *Section 1 - Introduction*;
- **'Sec2_Data.ipynb** contains the code to reproduce the results obtained in *Section 2 - Data*;
- **'Sec3_Methodology.ipynb'** contains the code to reproduce the results obtained in *Section 3 - Methodology*;
- **'Sec4_Empirical_Analysis.ipynb'** contains the code to reproduce the results in *Section 4 - Empirical Analysis*;
- **'A_appendix.ipynb'** contains the code to reproduce the results in *Appendix*.

### Data
The [Data](https://github.com/SaveChris/EUA_Volatility_DII_p/tree/main/Data) section is organized as follows:
- **'Dataset_EUA_24_Daily_Returns.xlsx'** contains raw financial returns dataset;
- **'EUA_All_Phases_Daily.xlsx'** contains dataset used for EUA price dynamics (Fig:1);
- **'IG_DII_E1_returns.p'** contains pickle results of the estimated IG through DII;
- **'IGs_toymodel.p'** contains pickle results of the estimated IG through DII for the toy model;
- **'quadratic_and_linear_XY_to_Z.p'** contains raw dataset for toy model;
- **'weights_DII_E1_returns.p'** contains estimated causal coefficients through DII;
- **'weights_toymodel.p'** contains the estimated causal coefficients through DII for the toy model.

## Contributing
We welcome contributions to improve **EUA_Volatility_DII**!
If you encounter any issues or have suggestions for improvements, please check the existing issues to see if the topic has already been discussed. If not, feel free to contact me [(Cristiano Salvagnin)](mailto:c.salvagnin@unibs.it) or [Aldo Glielmo](mailto:aldo.glielmo@gmail.com).
You should provide the following information when opening an issue:

- A descriptive title
- Steps to reproduce the issue (if applicable)
- Expected behavior
- Actual behavior
- Environment details (e.g., operating system, Python version)
- Screenshots, if applicable

Thank you for your contributions!

## License
This project is licensed under the Apache License 2.0 - see the [License](LICENSE.txt) file for details.