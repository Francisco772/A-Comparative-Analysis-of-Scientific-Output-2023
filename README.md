## 📌 Project Overview
This project challenges the traditional "volume-based" ranking of global research.While large economies like the **USA** and **China** dominate total publication counts due to their sheer economic scale, this "Giant bias" often overlooks smaller, highly efficient nations.We integrated socioeconomic indicators from **The World Bank** with real-time publication data from the **OpenAlex API** to identify "Specialist" nations—those that produce exceptional research output relative to their population and GDP.

---

## 🧪 Key Methodology
* **The Efficiency Metric:** A custom-weighted score designed to penalize pure scale and reward intensive productivity.Weights were derived from Pearson correlation coefficients to account for the "expected" output of a nation based on its wealth and size.

* **Missing Data Strategy (MICE):** Handled missing tertiary enrollment data using **Multivariate Imputation by Chained Equations** (10 iterations), ensuring data consistency across development profiles.

* **Advanced Dimensionality Reduction:**
    * **PCA:** Created a "Development Index" capturing **57.31% of data variance**.
    * **UMAP:** Identified non-linear "Geopolitical Neighborhoods," revealing that development is geographically clustered.


---

## 📊 Core Findings
* **The Specialist Rise:** When adjusted for scale, nations like **Lebanon, Cyprus, and Denmark** emerge as global leaders in research efficiency.
* **Field Nuance:** AI efficiency is heavily tied to digital infrastructure (**Internet Users**), whereas Medicine and Environmental research are often driven by regional necessity rather than just wealth.
* **The Scale Paradox:** We found a consistent **negative correlation** between population size and research efficiency ($-0.08$ to $-0.11$), suggesting that massive scale can lead to "efficiency friction".

---

## 🛠️ Tech Stack
* **Python:** `Pandas`, `NumPy`, `Scikit-learn` (MICE/IterativeImputer, PCA).
* **Visualization:** `Plotly`, `Seaborn` (Spearman & Pearson Heatmaps).
* **API:** `OpenAlex` (Programmatic retrieval of 2023 research counts).


# How to run

## How to setup
First, clone the repository:
```
git clone https://github.com/Francisco772/Data-in-the-wild.git
```
**Requirements**

Install the necessary Python libraries:
```
pip install pandas numpy seaborn matplotlib plotly umap-learn scikit-learn statsmodels pycountry
```
Then, run the main notebook on VSCode.

Note: We use Git LFS (Large File Storage) because our datasets are large. Make sure you have Git LFS installed (git lfs install) before cloning, or download the full dataset manually via this zip link: [World Bank Data (WDI_CSV.zip)](https://databank.worldbank.org/data/download/WDI_CSV.zip) .

## Team

António Santos, Francisco Oliveira, Henrique Aleixo, Tibor Szolomaier, Vincenzo Sabino
(IT University of Copenhagen)
