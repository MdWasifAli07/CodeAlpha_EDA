# Exploratory Data Analysis (EDA) — E-Commerce Catalog

## 📌 Repository: `CodeAlpha_EDA`
### 📑 Project: Task 2 — Exploratory Data Analysis

This project focuses on executing a structured, production-grade **Exploratory Data Analysis (EDA)** on the e-commerce product dataset extracted in Task 1. The analysis is built using an `.ipynb` notebook architecture optimized for **Google Colab**, leveraging statistical operations and visualization tools to transform raw, unformatted web data into clear, actionable business insights.

---

## 🎯 Core Project Objectives

The analysis follows a comprehensive business-driven data framework designed to answer the following operational queries:
1. **Data Integrity:** Inspecting structural shapes, identifying missing data fields, and diagnosing data type inconsistencies.
2. **Pricing Distribution:** Profiling pricing layers using continuous density plotting metrics to look for statistical anomalies.
3. **Rating Dispersions:** Tracking category volumes across ratings metrics to analyze platform feedback tendencies.
4. **Bivariate Correlations:** Testing the operational hypothesis: *Do higher-rated book categories explicitly command higher retail prices?*
5. **Inventory Performance:** Mapping exact active versus unavailable stock proportions across the catalog.

---

## 🛠️ Tech Stack & Libraries Utilized

The environment is built using Python 3 ecosystem standards for data science tasks:
* **Data Wrangling:** `Pandas` & `NumPy`
* **Data Visualizations:** `Matplotlib` (Object-oriented layout controllers) & `Seaborn` (Advanced statistical charts)
* **Feature Engineering & Formatting:** Python regular expressions (`re`) for parsing complex strings

---

## 📈 Analytical Workflow Steps

The notebook is divided into clear functional blocks for easy readability:

### 1. Environment & Data Ingestion
Sets up layout scales and global charting style templates. Features a Google Colab local file-stream upload block (`files.upload()`) to import datasets effortlessly on virtual runtimes.

### 2. Data Cleaning & Feature Engineering
* **Price Harmonization:** Strip monetary characters (`£`), clean empty strings, and map columns to high-precision numeric floats.
* **Ordinal Rating Categorization:** Transforms structural string elements (`"star-rating Three"`) into balanced, single-digit integers (`3`) for correlation assessments.
* **Categorical Standardization:** Groups inconsistent whitespace entries into strict data values (`In Stock`).

### 3. Univariate & Bivariate Explorations
* Dual Histogram-Boxplot combinations provide quick views of density distribution and clean outlier detection.
* Stratified categorical boxplots are implemented to evaluate price behaviors across star-rating boundaries.
* Split percentage pie charts provide a quick overview of product availability.

---

## 📊 Key Executive Findings

* **Data Health:** The scraped web layer extracted data perfectly; no critical variables or null fields were found in the dataset.
* **Pricing Models:** Retail prices display an even, roughly uniform distribution across the platform with no artificial or extreme outliers.
* **Feedback Balance:** Star ratings are uniformly split across 1 to 5 stars, showing a highly diverse selection of ratings.
* **Hypothesis Evaluation:** Bivariate visualizations reveal **zero statistical correlation** between rating tiers and price targets; highly rated products do *not* carry a premium price tag on this platform.

---

## 🚀 Usage Guide (Google Colab Deployment)

1. Open a new notebook template on [Google Colab](https://colab.research.google.com/).
2. Create Markdown cells for headings and paste the Python blocks into corresponding Code cells.
3. Run **Cell 2** and upload your generated `products.csv` file from Task 1.
4. Execute all runtime blocks sequentially to automatically generate visual figures, statistical summary logs, and your final executive summaries.
5. Export the finished file via `File -> Download -> Download .ipynb` and save it directly into your GitHub repository space.
