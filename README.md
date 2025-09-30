# Shrinkflation-Project
Data storytelling project on shrinkflation using BLS R-CPI-SC
# Shrinkflation, Measured: What Smaller Packages Actually Did to Prices

This project uses data from the U.S. Bureau of Labor Statistics (BLS) to explore **shrinkflation** — the practice of reducing product sizes while keeping prices the same.  

By combining two research datasets:  
- **R-CPI-SC Index** → shows what inflation would look like if package sizes never changed  
- **Frequency of Size Changes** → counts how often products in the CPI sample were downsized or upsized  

We can see both **how much prices changed** and **how often shrinkflation events occurred**.

---

## Key Findings
- **Shrinkflation is frequent:** Downsizing spiked in 2021–2022, peaking at ~74 events in a 12-month span, while upsizing stayed far lower.  
- **Groceries surged:** *Food at home* prices rose ~+28.7% above Dec 2019, even after adjusting for shrinkflation.  
- **Uneven impact:** Some categories (e.g., eggs, beef, juices) saw much larger cumulative increases than the overall basket.  
- **Double effect:** The hardest-hit categories are where both **prices rose fastest** and **downsizing was most common**, amplifying the consumer experience.  

---

## Repository Structure

data/raw/ # Original Excel files from BLS
data/processed/ # Cleaned CSVs created by the notebook
notebooks/ # Jupyter notebook(s) with analysis
outputs/figures/ # Exported charts for blog/presentation


---

## ⚙️ Reproducibility
To reproduce this project:

1. Clone the repo:
   ```bash
   git clone https://github.com/hadil-ghazal/Shrinkflation-Project.git
   cd Shrinkflation-Project

2. Create the conda environment:
conda env create -f environment.yml
conda activate shrinkflation

3.Run the notebook:
notebooks/01_shrinkflation_analysis.ipynb

4. The Cleaned data will be saved in data/processed/ and figures in outputs/figures/.


 ## Data Sources

R-CPI-SC Index: BLS Research CPI excluding size changes

Frequency of Size Changes: BLS downsizing/upsizing counts

## Limitations

These are research series, not official CPI production indexes.

Frequency counts reflect only the CPI sample, not the entire marketplace.

Imputation choices affect how size changes are removed from the index.

Takeaways should be framed as illustrative, not definitive.


##Conclusion:

Shrinkflation is real, but its overall inflation impact is modest.
The consumer frustration comes from the double effect:

Prices are higher, and

Packages are smaller more often.

Together, these trends explain why groceries feel more expensive than CPI alone suggests.
