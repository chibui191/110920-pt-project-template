# Exploratory Analysis of Movies Released from 1915 to 2019

**Author**: Chi Bui

## Overview

The objective of this project is to use ***exploratory data analysis*** and ***visualization*** to identify current trends and key parameters of a successful movie. Applying these technique, this analysis seeks to identify customer preference and determine how to construct and optimize content for our product to reach its maximum potential.

## Business Problem

The filmmaking industry is currently dominated by 6 big players 'Warner Bros', 'Walt Disney', '20th Century Fox', 'Paramount', 'Sony', and 'Universal', which accounted for approximately 80% of the market share altogether. Planning for a debut into a highly competitive market for a new company would therefore require thorough analysis of the current landscape of the film industry.

The focus of this analysis is to investigate the relationships between certain attributes like **genres**, **directors**, **production company**, **month of release** on a movie’s commercial success, as well as the correlation between **ratings** and **box office gross**. My goal is to use data collected from two main sources [**Rotten Tomatoes**](https://www.rottentomatoes.com/) and [**the-numbers.com**](https://www.the-numbers.com/market/) to study market trends from 1915 to 2018 with a special focus on the 2000-2018 to derive insights on how to optimize a debut into the movie industry for a new company in 2021.

## Data

I was provided with 11 movie datasets from various sources:
- [Box Office Mojo](https://www.boxofficemojo.com/) (1)
- [IMDb](https://www.imdb.com/) (6)
- [Rotten Tomatoes](https://www.rottentomatoes.com/) (2)
- [The Movie Database](https://www.themoviedb.org/) (1)
- [The Numbers](https://www.the-numbers.com/market/) (1)

The final dataframe used for the majority of analyses this project (`tn_rotten_tomatoes`) is a merge between datasets from **the-numbers.com** and **Rotten Tomatoes**. This dataset contains 4,304 entries for movies released in the span of 104 years from 1915-02-08 to 2018-12-31.

The goal of this project is to weigh the impacts of attributes like **genres**, **directors**, **production company**, and **month of release** on the commercial success of movies as well as the correlation between ratings and box office gross. 

Commercial success of movies are evaluated on:
- <b>box office gross</b>
- <b>profit</b> = worldwide gross - production budget 
- <b>rate of return</b> = profit / production budget

## Methods

This project uses **descriptive analysis** including the analysis of trends and market distribution over time, which would provide a useful overview of the landscape of the filmmaking industry. 

Tools used primarily for this analysis:
- NumPy
- Pandas
- Matplotlib
- Seaborn


## Results

1. The number of movies released seems to have hit its peak in 2008, which coincides with Netflix's expansion to offering streaming services in 2007. In the span of 12 years, streaming media seem to have quickly taken over movie theaters.

![Plot-01](./images/plt-01.png)

2. Movies with high commercial success are rarely categorized solely as one single genre. Based on historical data, a combination of **Action & Adventure<** and **Science Fiction & Fantasy** with some **Comedy** and **Drama** elements tend to do relatively well. Although the number of movies released seems to have reduced since 2008, the percentage of movies tagged with **Action & Adventure** and **Science Fiction & Fantasy** are still on the rise, which indicates an upward trend for these.

![Plot-05](./images/plt-05.png)

![Plot-10](./images/plt-10.png)

3. In general, **May** and **June** are the best months to release a movie for potential profit. However, the best time to release a **Horror** and **Mystery & Suspense** movie would be **October**. Some of the movies with highest rates of return (profit/budget) in the last 20 years are categorized as **Horror** and **Mystery & Suspense**. 

![Plot-11](./images/plt-11.png)

4. Based on profit, top candidates to assume the role of Directors would be Anthony Russo, and James Cameron.

![Plot-14](./images/plt-14.png)

## Conclusions

Some recommendations for a new company to break into the movie production industry can be derived from this exploratory analysis as follows:
<br>
- Combining different genres generally boosts profit and return on investment as it helps attract more demographics. Some of the most profitable combinations include **Action & Adventure**, **Science Fiction & Fantasy** with some elements of **Drama**, **Comedy** and **Mystery & Suspense**. However, producing movies based too directly on past success could also lead to potentially over-saturating the market. Therefore, it is always important to incorporate elements of novelty into the movies and take into consideration how the audience might have evolved over time.  


- **May** and **June** are the best months to release a movie for potential profit. The best time to release a **Horror** and **Mystery & Suspense** movie would be **October**. Some of the movies with highest rate of return (profit/budget) in the last 20 years are categorized as **Horror** and **Mystery & Suspense**.  


- Top candidates to assume the role directors would be **Anthony Russo** and **James Cameron**. 

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-movie-exploratory-analysis.ipynb) or our [presentation](./Movie_Presentation.pdf).

For any additional questions, please contact **Chi Bui at [chibui191@gmail.com](mailto:chibui191@gmail.com)**

## Repository Structure

```
├── README.md                                             
├── dsc-phase1-project-movie-exploratory-analysis.ipynb   
├── DS_Project_Presentation.pdf                           
├── data                                                  
└── images                                                
```
