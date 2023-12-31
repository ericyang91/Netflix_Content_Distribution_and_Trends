# Netflix Content Distribution and Trends
![logo](https://i.pcmag.com/imagery/reviews/05cItXL96l4LE9n02WfDR0h-5.fit_scale.size_1028x578.v1582751026.png)

## Purpose:

The primary objective of this project is to conduct a comprehensive analysis of the distribution of movie genres on Netflix across different countries and to visualize the evolving trends over the years. Leveraging the power of Python for Exploratory Data Analysis (EDA) and Tableau for creating an interactive dashboard, the project aims to provide insights into the diverse preferences of audiences worldwide.

To achieve this, the project delves into the vast Netflix dataset, exploring the prevalence of genres in different regions and how these preferences have changed over time. By utilizing Python's data manipulation and visualization libraries, the analysis uncovers patterns, disparities, and emerging trends in movie genre consumption.

The Tableau dashboard created as part of this project serves as a visual representation of the findings, offering an intuitive and interactive platform for users to explore and understand the nuanced dynamics of movie genre distribution across countries. Through this visualization, users can gain valuable insights into the evolution of entertainment preferences on Netflix, identifying patterns that may be influenced by cultural factors, global events, or the platform's own content strategy.

In conclusion, this project not only contributes to a deeper understanding of global entertainment consumption but also showcases the powerful synergy between Python for data analysis and Tableau for visualization in uncovering intricate patterns within large and dynamic datasets. By shedding light on the evolving landscape of movie genres on Netflix, the analysis provides a valuable resource for content creators, analysts, and enthusiasts seeking to stay abreast of the ever-changing world of digital entertainment.

## DataFrame:

A quick snapshot of the raw DataFrame:
</br></br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/raw.png" alt="rawdata"/>
</p></br>

Below are the steps I took to clean the data:
- Filtered for movies only
- Dropped unnecessary columns and renamed the columns of interest
- Dropped null values
- Categorized minor genres under 'Other'
- Separated 'Date Added' column to 'Year Added' and 'Month Added'
- Dropped Year '2021' as we only had partial data


## Number of Contents for each Genre:
</br>
</br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/genre.png" alt="genre"/>
</p>
</br>

Between the years 2008 and 2020, the genre that witnessed the highest volume of movie releases was 'Dramas,' making it the most prolific category during this period. In contrast, the genre with the least number of movie releases was 'International Movies,' indicating a comparatively lower frequency of production and distribution within the specified timeframe. This observed trend underscores the significant prominence of dramas in the cinematic landscape, while also highlighting the relatively modest representation of international films during the analyzed period.

</br>
</br>

## Number of Contents Trend:
</br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/moviecount.png" alt="moviecount"/>
</p>
</br>

Commencing from the year 2016, there was a remarkable and exponential surge in the quantity of movies added to the platform. This upward trajectory reached its zenith in 2019, experiencing a peak in the influx of new content. However, the momentum exhibited a slight deceleration in 2020, with a discernible but marginal reduction in the number of movies added. This intriguing pattern suggests a dynamic evolution in the expansion of the platform's content library, characterized by a rapid ascent, a pinnacle in 2019, and a subsequent modest tapering off in the subsequent year.

</br>
</br>

## Average Number of Contents Released each Month:
</br></br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/monthlyaverage.png" alt="monthlyaverage"/>
</p></br>
When examining the average monthly patterns of movie additions, it becomes evident that both March and January stand out as the months with the highest influx of new content. These particular months consistently demonstrate a notable surge in the introduction of movies to the platform, suggesting a propensity for heightened activity in content acquisition during these periods. On the contrary, February emerges as the month with the least number of movie additions, showcasing a relative lull or subdued pace in the augmentation of the platform's cinematic repertoire. This observed variability across the months underscores the dynamic nature of content release strategies, with certain months exhibiting robust growth while others experience a more measured addition of movies to the streaming platform.
</br></br>

## Movie Distribution by Geography:
</br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/country.png" alt="country"/>
</p></br>

The preeminent contributor to the cinematic landscape during the specified timeframe was the United States, substantiating its position as the primary source of movie content. Following closely in the global cinematic tapestry were India, the United Kingdom, and Canada, each making substantial contributions to the diverse array of films available. This hierarchical distribution of movie contributions underscores the multinational nature of content availability on the platform, with the United States leading the way, followed by other significant film-producing nations such as India, the United Kingdom, and Canada. This collaborative amalgamation of cinematic offerings from these diverse regions contributes to the rich and multifaceted content tapestry that characterizes the streaming platform's global appeal.

</br>
</br>

## Top 6 Contributors:
</br></br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/topsix.png" alt="topsix"/>
</p></br>
</br>
</br>

## Chi-Squared Test of Independence:

The Chi squared test of independence is used to explore the relationship between two categorical variables - genre and geography.

Ho = There is no significant relationship between the genre of the Netflix contents and the countries that added them.

Ha = There is a significant relationship between the genre of the Netflix contents and the countries that added them.
</br></br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/chi2.png" alt="chi2"/>
</p></br>
</br>
</br>

## Dashboard:

A snippet of the [Tableau interactive Dashboard](https://public.tableau.com/app/profile/ji.yeol.yang/viz/NetflixGenreDashboard/Dashboard1):
</br></br>
<p align="center">
  <img src="https://github.com/ericyang91/Netflix_Content_Distribution_and_Trends/blob/main/images/dashboard.png" alt="dashboard"/>
</p></br>
</br>
</br>

## Summary:
</br>

This Netflix project analyzed the content available on the platform, focusing on various aspects such as genre distribution, temporal trends, regional contributions, and the relationship between geography and genre. Here are the key findings:

`Genre Distribution:`

The most prevalent genre on Netflix is "Drama," having the highest count among all genres.


`Temporal Trends:`

Netflix experienced the highest growth in content in 2019, indicating a consistent audience demand for contents.
The number of added contents peaked in 2019 and saw a slight decrease in 2020.

`Monthly Trends:`

On average, February is the month with the least number of content additions.
March stands out as the month with the highest average number of content additions, indicating a potential pattern in seasonal releases or strategic scheduling.

`Regional Contributions:`

The United States led in contributing the most number of contents to Netflix, showcasing a significant presence in the platform's content library.
In the USA, the genre "Documentary" had the highest count of additions, with "Drama" following closely.

`International Contributions:`

India emerged as a notable contributor to Netflix content, securing the runner-up position in terms of the number of contents added.
In India, "Drama" was the dominant genre with the highest count of additions.

`Chi-Squared Test of Independence:`

The chi-squared test of independence revealed a significant relationship between geography (country) and genre, suggesting that the distribution of genres varies significantly across different regions.

This comprehensive analysis provides insights into the dynamic landscape of Netflix content, highlighting the dominance of certain genres, temporal patterns, and the influence of geographical factors on content preferences.

</br>
</br>

## Languages and Libraries:
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/matplotlib-3776AB?style=flat&logo=matplotlib&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-3776AB?style=flat&logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/Visual_Studio_Code-007ACC?style=flat&logo=visual-studio-code&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)

