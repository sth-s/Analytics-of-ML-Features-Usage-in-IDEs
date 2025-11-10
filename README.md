# Analytics of ML Features Usage in IDEs

This repository contains a comprehensive analysis of user activity data for Large Language Model (LLM) features within Integrated Development Environments (IDEs). The analysis covers a three-month period from March to May 2025, exploring user behavior patterns, product performance, and strategic business opportunities.

## Project Overview

The primary goal of this analysis is to move beyond surface-level metrics and uncover the underlying drivers of user engagement and spending. By examining interactions across different user licenses, LLM models, and features, this project identifies key user segments, their distinct behavioral strategies, and provides actionable recommendations to guide product and marketing decisions.

### Key Objectives

*   **Understand** user behavior patterns and engagement with different ML features.
*   **Analyze** the relationships between user licenses, models, and features.
*   **Identify** trends in usage and spending over time.
*   **Provide** data-driven, actionable business recommendations.

## Dataset

The dataset used for this analysis is `da_internship_task_dataset.csv`. It contains daily aggregated, anonymized user activity.

**Columns:**
*   `uuid`: Anonymized user ID.
*   `day_id`: Date of the user activity.
*   `license`: The user's license type (e.g., Basic, Premium, Enterprise).
*   `model`: The LLM model used (e.g., Model_A, Model_B).
*   `feature`: The IDE feature used (e.g., Feature_1, Feature_2).
*   `requests_cnt`: The number of requests made by the user on a given day.
*   `spent_amount`: The amount of credits spent by the user on a given day.

## Repository Structure


    .
    ├── analysis.ipynb # The Jupyter Notebook with all the code, analysis, and visualizations.
    ├── analysis.html # An HTML export of the notebook for easy viewing in a browser.
    ├── da_internship_task_dataset.csv # The raw dataset used for the analysis.
    ├── requirements.txt # A list of Python dependencies required to run the notebook.
    └── README.md # This file.


## How to Run

There are two ways to run this analysis: quickly in your browser using Google Colab, or by setting up a local environment for the full experience.

### 🚀 Quick Start with Google Colab (Recommended for Viewing)

This is the easiest way to get started without any local installation.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sth-s/Analytics-of-ML-Features-Usage-in-IDEs/blob/main/analysis.ipynb)

1.  Click the "Open in Colab" button above.
2.  The notebook will open in a new tab.
3.  You will need to upload the `da_internship_task_dataset.csv` file to your Colab session. You can do this by using the file browser on the left-hand side of the Colab interface.
4.  Run the cells in the notebook to execute the analysis.

**Important Note:** The interactive dashboards in Section 6 will **not** be displayed in Google Colab due to compatibility issues. For the full interactive experience, please run the notebook locally or view the pre-rendered `analysis.html` file in your browser.

### Local Environment Setup (for Full Interactivity)

To replicate the analysis on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/sth-s/Analytics-of-ML-Features-Usage-in-IDEs.git
    cd Analytics-of-ML-Features-Usage-in-IDEs
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Launch Jupyter Notebook and open `analysis.ipynb`:**
    ```bash
    jupyter notebook
    ```

## Executive Summary of Key Findings

The analysis revealed several critical, non-obvious insights into the business:

1.  **A Two-Tiered Product Economy:** The core of the product's value is defined by two distinct "engine" tiers—a low-cost **"Economy Tier"** and a high-cost **"Premium Tier"** based on the chosen model. This, not the specific feature, is the primary driver of user spending.

2.  **Two Distinct High-Value Segments:** The most valuable customers, **Enterprise** and **Premium** users, exhibit fundamentally different behaviors.
    *   **Enterprise users act as "Strategic Investors,"** willing to pay significantly more for premium models to solve critical tasks.
    *   **Premium users act as "Pragmatic Optimizers,"** focusing on maximizing volume and efficiency with economy models.

3.  **A Stable, Hybrid Revenue Model:** The business is not driven by a few "whales" (the 80/20 rule is rejected). Instead, it stands on two strong pillars: a "Concentrated Core" of high-value Enterprise/Premium users and a "High-Value Long Tail" of Basic/Standard users, proving the success of both Sales-Led and Product-Led strategies.

4.  **Separate B2B and Prosumer Markets:** Analysis of weekly activity patterns confirms that Enterprise/Premium users represent a B2B market with weekday-focused activity, while Basic/Standard users represent a "Prosumer" market with more flexible usage patterns. These are two separate audiences, not a single conversion funnel.

## Technologies Used

*   Python
*   Pandas
*   Matplotlib
*   Seaborn
*   Jupyter Notebook