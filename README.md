# My Data Science Project Template 📊

This repository serves as a foundation for developing data science projects. Every project I share will follow this structure. To consult the readme in Spanish, click here [README_ESP.md](https://github.com/sofiavalino/template-datascience-project/blob/main/README_ESP.md)

## Purpose 🎯

The goal of this repository is to establish a clear and organized structure for data science projects, making collaboration and development easier.

## Repository Structure 🗂

```plaintext
template-datascience-project/
├── data/                       # Data storage
│   ├── raw/                    # Raw data
│   ├── processed/              # Clean and processed data
├── notebooks/                  # Jupyter Notebooks
│   ├── exploration.ipynb       # Initial exploration and analysis
│   ├── model.ipynb             # Model creation and evaluation
├── src/                        # Source code
│   ├── preprocessing.py        # Data preprocessing
│   ├── models.py               # Model creation and evaluation
│   ├── utils.py                # Utility functions
├── outputs/                    # Generated outputs
│   ├── figures/                # Visualizations and plots
│   ├── predictions/            # Generated predictions
├── app/                        # Application and deployment scripts
│   ├── main.py                 # Application entry point
│   ├── api.py                  # API-related functions
│   ├── config.py               # Project-specific configurations
├── deployments/                # Deployment configurations
│   ├── kubernetes/             # Kubernetes manifests
│   ├── docker/                 # Docker configurations
│   ├── cloudbuild/             # Cloud Build configurations
├── docs/                       # Documentation and diagrams
│   ├── diagrams/               # Architecture and workflows
│   ├── reports/                # Analytical reports
├── requirements-project.txt    # Project dependencies
├── README.md                   # Project documentation
└── .gitignore                  # Git ignored files and folders
```

## Using `shared-resources` Repository 🔧

This project integrates with a shared repository [`shared-resources`](https://github.com/sofiavalino/shared-resources), containing reusable tools and configurations.

### Key Features of `shared-resources`

- **Centralized Logger**: Provides unified activity logging (`logger.py`).
- **Global Configurations**: Manages routes, API keys, and common parameters (`config/global_config.py`).
- **Shared Utilities**: Includes reusable tools like `timer.py` for execution tracking and `data_loader.py` for loading datasets.
- **Logging Templates**: Predefined logs for activities like preprocessing.

### Steps to Use `shared-resources`

1. Add the submodule to your repository:
   ```bash
   git submodule add https://github.com/sofiavalino/shared-resources shared/
   git submodule update --init --recursive
   ```

2. Import and use its tools in your project:
   ```python
   from shared.utils.data_loader import load_data
   df = load_data('data/raw/dataset.csv')
   ```

3. Update the submodule regularly:
   ```bash
   git submodule update --remote
   ```

## How to Run This Project 🖥️

1. Clone the repository with its submodules:
   ```bash
   git clone --recursive https://github.com/sofiavalino/template-datascience-project.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements-project.txt
   ```

3. Follow the instructions in the notebooks or scripts to execute the project.

## Contributions 🤝

Feel free to suggest improvements or report issues by opening an issue or submitting a pull request. Your feedback is highly appreciated.

## License 📜

This project is under the [MIT License](https://github.com/sofiavalino/template-datascience-project/blob/main/LICENSE). Review the license terms for usage and modification.

## Contact 📧

Explore the projects and reach out if you have questions or suggestions!

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white&style=flat-square)](https://www.linkedin.com/in/sofiavalino/)  
[![Gmail](https://img.shields.io/badge/-Gmail-D14836?logo=gmail&logoColor=white&style=flat-square)](mailto:valinosofia@gmail.com)

## My Blog 📚

Check out my blog for university notes and topics on Data Science and Computer Science. You'll find study materials, project details, and more!

[![Blog](https://affable-valinosofia.wordpress.com/wp-content/uploads/2024/07/site-logo.png?w=88&h=88)](https://affable-valinosofia.wordpress.com/)
