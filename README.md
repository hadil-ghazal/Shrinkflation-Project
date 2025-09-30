# Shrinkflation-Project
Data storytelling project on shrinkflation using BLS R-CPI-SC
# Shrinkflation, Measured: What Smaller Packages Actually Did to Prices

This project uses data from the U.S. Bureau of Labor Statistics to explore **shrinkflation** which is the practice of reducing product sizes while keeping prices the same.

By combining two research datasets we can see both **how much prices changed and how often shrinkflation events occurred**. The datasets are :  
- **R-CPI-SC Index** - this shows what inflation would look like if package sizes never changed  
- **Frequency of Size Changes** - this counts how often products in the CPI sample were downsized(less product for the same price) or upsized(more product for the same price) 

---
## Important Deliverables:
- **Full analysis notebook**: https://github.com/hadil-ghazal/Shrinkflation-Project/blob/main/notebooks/01_shrinkflation_analysis.ipynb
- **Figures and visuals**: https://github.com/hadil-ghazal/Shrinkflation-Project/tree/main/outputs/figures
- **public facing presentation:** https://github.com/hadil-ghazal/Shrinkflation-Project/blob/main/outputs/public/01_shrinkflation_analysis.html
   - *Note: GitHub shows raw HTML code when previewing the public facing html. To view it as intended download that .html file and simply open it in your web browser to view

---

## Important Findings
- **Shrinkflation:** Downsizing spiked from 2021 to 2022 and peaked at about ~74 events in a 12 month span, while upsizing stayed far lower with minimal spiking events.  
- **Groceries surged:** Food at home (meaning groceries and ingredients) prices rose about ~+28.7% above December of 2019, independent of  shrinkflation.  
- **Uneven impact:** Some categories (like eggs, beef, and juice) had much larger increases than the overall population being analyzed.  
- **compounded pricing results:** The hardest hit categories are where both **prices increase most and fastest** and **downsizing was most common**, which compounded the impact to the consumers.  

---

## Repository Setup and Structure

data/raw/ # Original Excel files from BLS
data/processed/ # Cleaned CSVs created by the notebook
notebooks/ # Jupyter notebooks with the analysis
outputs/figures/ # Exported charts 


---

## Reproducibility
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

4. The Cleaned data will be saved in data/processed/ and figures in outputs/figures


 ## Data Sources

R-CPI-SC Index: BLS Research CPI excluding size changes

Frequency of Size Changes: BLS downsizing/upsizing counts

## Limitations and Data Background

A few things to keep in mind when interpreting this project:  

- These datasets were created by the **U.S. Bureau of Labor Statistics (BLS)** using the same underlying price data as the official CPI. The difference is in the methods which are listed in the numbering 1-3 below. Because they are **research tools**, not official indexes, they don’t give the full picture of the consumer experience. They are designed to answer the question of *how much of inflation comes from package size changes* . It is not meant to capture every detail of what customers experience. 
  1. The **official CPI** counts shrinkflation as a price increase.  
  2.The **R-CPI-SC (research CPI without size changes)** removes that effect, showing what inflation would look like if package sizes never changed.  
  3. The **frequency file** counts how often downsizing and upsizing events were observed in the CPI sample.  
- The **frequency counts** are only from the CPI sample, so they show patterns but not every product in every store.  
- The way BLS **adjusts for size changes** involves a level of assumptions, which means different choices could lead to slightly different numbers.  
- Bottom line: these charts are **illustrative, not definitive**. They show the shape of shrinkflation in the CPI sample, but not the whole marketplace or every customer’s experience.



## Conclusion:

Shrinkflation is real, but its overall inflation impact is modest.
The consumer frustration comes from the double/compounud effect which is when two things happen simultaneously: 1. Prices are higher **AND** 2. Products are smaller more often. It's fair to say if the price went up alone, or the products decreased in size alone - that the impact would be less burdensome. But given they are both happening simultaneously, the result feels more "expensive"

Combined, all these trends explain why groceries feel more expensive than CPI being assessed in isolation alone suggests.
