# bayesian-media-mix-model
Bayesian Media Mix Model to analyze the impact of advertising campaigns on sales and ROI.

This project implements a **Bayesian Media Mix Model (BMMM)** to quantify the impact of marketing campaigns on product sales across multiple channels. Using historical advertising spend and sales data, the model estimates channel-level contribution, campaign effectiveness, and ROI while accounting for lagged effects and uncertainty in the estimates. 

The project is designed as a **hands-on guide for marketers and data scientists** to understand Bayesian approaches to media mix modeling, adstock effects, and data-driven campaign optimization.


---

## Environment Setup

This project uses a Conda environment for dependency management. Create the environment using the `environment.yml` file provided in the repository.

### **environment.yml**

```yaml
name: bayesian-mmm
channels:
  - conda-forge
  - defaults
dependencies:
  - python=3.11
  - numpy
  - pandas
  - scipy
  - scikit-learn
  - matplotlib
  - seaborn
  - plotly
  - jupyterlab
  - ipykernel
  - pymc=5      # Bayesian modeling
  - arviz        # posterior analysis & visualization
  - statsmodels  # optional regression diagnostics
  - tqdm         # optional progress bars
  - pip
  - pip:
      - opt_einsum  # sometimes required for PyMC
```

### Creating the Environment

```bash
conda env create -f environment.yml
conda activate bayesian-mmm
jupyter lab
```
