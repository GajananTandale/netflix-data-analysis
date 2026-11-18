# Netflix Data Analysis

Data analysis project done for the **Auspify Technologies** internship ("Data Analysis using Python"), using Python with pandas, matplotlib, seaborn and plotly.

**Made by:** Gajanan Tandale

## About the project
The dataset has about 8,790 Netflix titles (movies and TV shows). I cleaned the data and then analysed it to understand what kind of content Netflix has, where it comes from, when it was released, and who it is made for.

## Tasks completed
1. **Data cleaning:** checked missing values and "Not Given" entries, removed duplicate titles, fixed the date format, and saved a cleaned file (8,786 rows).
2. **Content type analysis:** Movies vs TV Shows, and how many titles were added each year.
3. **Country analysis:** top content-producing countries and the movie/TV split for each.
4. **Release-year trend:** how many titles were released each year and each decade.
5. **Rating and genre analysis:** rating distribution, top genres, a genre vs audience heatmap, and interactive Plotly charts.
6. **Business insights:** a one-page dashboard, runtime and season charts, and a short report with recommendations.

## Main findings
- About 70% of the titles are movies and 30% are TV shows.
- The United States has the most titles (3,240), followed by India (1,056) and the United Kingdom (638).
- Titles released in 2018 are the highest (1,144). Most titles were added to Netflix in 2019 (2,013).
- The 2010s make up about 67% of the catalogue.
- TV-MA (3,204) and TV-14 (2,155) are the most common ratings, so most content is for adults and teens.
- International Movies, Dramas and Comedies are the biggest genres.
- The median movie is 98 minutes long, and about 67% of the TV shows have only one season.

## Files in this repository
| File / folder | What it is |
|---|---|
| `netflix_analysis.ipynb` | Full code and results (Jupyter Notebook) |
| `netflix_analysis.html` | HTML copy of the notebook with outputs |
| `Dataset.csv` | Original dataset |
| `netflix_cleaned.csv` | Dataset after cleaning |
| `task6_dashboard.png` | Final business dashboard |
| `outputs/` | Interactive Plotly charts (download and open in a browser) |
| `screenshots/` | Screenshots of each task (task1 to task6) |

## Note about the audience column
The dataset only has ratings (like TV-MA or PG-13), so I made a new column called `audience` by grouping the ratings into five groups:
- **Kids:** TV-Y, TV-Y7, TV-Y7-FV, TV-G, G
- **Older Kids:** TV-PG, PG
- **Teens:** TV-14, PG-13
- **Adults:** TV-MA, R, NC-17
- **Not Rated:** NR, UR

This grouping is my own choice.

## Limitations
- The data ends in September 2021, so 2021 is not a full year.
- 287 titles have no country listed, so they are left out of the country results.
- The data shows what is on Netflix, not how much people watched it.

## How to run
1. Install the libraries: `pip install pandas matplotlib seaborn plotly jupyter`
2. Keep `netflix_cleaned.csv` in the same folder as the notebook.
3. Run `jupyter lab`, open `netflix_analysis.ipynb`, and choose **Kernel → Restart Kernel and Run All Cells**.
