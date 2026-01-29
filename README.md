## 📌 Project Overview
[cite_start]This project challenges the traditional "volume-based" ranking of global research[cite: 22, 103]. [cite_start]While large economies like the **USA** and **China** dominate total publication counts due to their sheer economic scale, this "Giant bias" often overlooks smaller, highly efficient nations[cite: 22]. [cite_start]We integrated socioeconomic indicators from **The World Bank** with real-time publication data from the **OpenAlex API** to identify "Specialist" nations—those that produce exceptional research output relative to their population and GDP [cite: 23, 28-34].

---

## 🧪 Key Methodology
* [cite_start]**The Efficiency Metric:** A custom-weighted score designed to penalize pure scale and reward intensive productivity[cite: 104, 106]. [cite_start]Weights were derived from Pearson correlation coefficients to account for the "expected" output of a nation based on its wealth and size[cite: 108, 535].

* [cite_start]**Missing Data Strategy (MICE):** Handled missing tertiary enrollment data using **Multivariate Imputation by Chained Equations** (10 iterations), ensuring data consistency across development profiles[cite: 92, 98, 575].

* **Advanced Dimensionality Reduction:**
    * [cite_start]**PCA:** Created a "Development Index" capturing **57.31% of data variance**[cite: 483, 484].
    * [cite_start]**UMAP:** Identified non-linear "Geopolitical Neighborhoods," revealing that development is geographically clustered [cite: 471-475].


---

## 📊 Core Findings
* [cite_start]**The Specialist Rise:** When adjusted for scale, nations like **Lebanon, Cyprus, and Denmark** emerge as global leaders in research efficiency[cite: 219].
* [cite_start]**Field Nuance:** AI efficiency is heavily tied to digital infrastructure (**Internet Users**), whereas Medicine and Environmental research are often driven by regional necessity rather than just wealth[cite: 532, 533, 536].
* [cite_start]**The Scale Paradox:** We found a consistent **negative correlation** between population size and research efficiency ($-0.08$ to $-0.11$), suggesting that massive scale can lead to "efficiency friction"[cite: 537, 548, 569].

---

## 🛠️ Tech Stack
* **Python:** `Pandas`, `NumPy`, `Scikit-learn` (MICE/IterativeImputer, PCA).
* **Visualization:** `Plotly`, `Seaborn` (Spearman & Pearson Heatmaps).
* [cite_start]**API:** `OpenAlex` (Programmatic retrieval of 2023 research counts)[cite: 34].





















# Global Drivers of Research Efficiency (2023)

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
