# Movie Rating Analysis

This project explores the IMDb Top 1000 dataset to uncover the factors behind cinematic success. It analyzes how creative elements (genres and directors), audience reception, and critical scores influence a film's financial performance.

### Tech Stack
* **Languages:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn

### Core Objectives
* **Data Wrangling:** Cleaned unstructured data, including converting 'Runtime' and 'Gross' columns into numeric formats for statistical analysis.
* **Creative & Trend Analysis:** Identified dominant genres and directors, and explored how film characteristics vary across different eras.
* **Statistical Analysis:** Used correlation heatmaps and regression modeling to evaluate the relationship between ratings, runtime, and financial success.

### Conclusion & Key Findings
After performing a comprehensive analysis, the following insights were uncovered:

* **Revenue Determinants vs. Runtime:** Contrary to the assumption that longer films generate more revenue, our regression analysis shows only a weak positive correlation ($r \approx 0.14$) between `Runtime` and `Gross` revenue. This confirms that film duration is not a significant predictor of a movie's financial performance.
* **Cinematic Success (Quality Metrics):** Our analysis shows that `IMDB_Rating` and `Meta_score` share a strong positive relationship. This proves that both professional critics and general audiences are consistent in their assessment of a film's "cinematic success," making these ratings reliable indicators of perceived quality.
* **Financial Success (Box Office Metrics):** While ratings are reliable indicators of cinematic quality, they are poor predictors of box office revenue. Financial success appears to be driven more by external factors—such as genre popularity, marketing, and distribution—than by the film's critical or audience rating.
* **Final Takeaway:** We must distinguish between **cinematic success** (how good a film is) and **financial success** (how much money it makes). A film can be a critical masterpiece and a financial underperformer, or vice versa, because box office revenue is determined by broader market dynamics rather than artistic merit alone.

### Project Structure
* `imdb_top_1000.csv` - The raw IMDb movie dataset.
* `analysis.ipynb` - Jupyter Notebook containing data cleaning, statistical analysis, and visualizations.
