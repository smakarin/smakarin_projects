
## Forecasting Video Game Popularity

### Toolset

Data preprocessing: handling missing values, table merging, duplicate handling, pandas;  
Data visualization: seaborn and plotly;  
Hypothesis testing: scipy library.  

### Introduction

In this project, historical data from open sources is available on video game sales, user and expert ratings, genres, and platforms (e.g., Xbox or PlayStation).
The provided dataset includes information about games, platforms, ratings, sales by region, and age groups.  

### Objective
The goal is to identify patterns in the sales of different genres and platforms, determine successful genres, and test proposed hypotheses.  
### Project Structure  
1. Exploring the general information in the provided dataset.
2. Data preparation for analysis.
3. Exploratory data analysis:
- Examining the number of games released per year.
- Analyzing game sales on different platforms over time.
- Identifying a time period for forecasting sales in 2017.
- Analyzing platforms and selecting the most promising ones.
- Investigating differences in sales for each game on different platforms.
- Exploring the impact of user and critic ratings on sales.
- Analyzing the profitability of different genres.
4. Creating a user profile for each region:
- Top 5 popular platforms.
- Top 5 popular genres.
- Examining the influence of ESRB rating on sales in each region.
5. Hypothesis testing:
- Comparing the average user ratings of Xbox One and PC platforms.
- Comparing the average user ratings of Action and Sports genres.
6. Overall conclusion. 

### Conclusion

Based on the analysis conducted, the following conclusions can be drawn:

1. General comments on the study: 
- The analysis used data starting from 2012, as older data is not relevant due to the shift in gaming platforms.
2. Conclusions on platform analysis:
- The potentially most profitable platforms in 2017 are PS4 and XOne. However, platforms like 3DS and WiiU should not be overlooked, as they are very popular in Japan and have significant sales.
- PC sales remain stable and unaffected by platform changes.
- The platforms with the highest median sales are PS3, PS4, X360, and Xone. Wii and WiiU are slightly below in terms of sales.
- The average user ratings for XOne and PC platforms are similar.
3. Conclusions on game analysis:
- Critic ratings have an impact on game sales, while user ratings do not. However, this trend is not applicable to games for Nintendo platforms (WiiU, Wii, DS, and 3DS).
- The most frequent genre is Action, while the most profitable genre is Shooter.
- The Platform genre ranks third in terms of profitability but has fewer game releases.
- The average user rating for Action games is higher than that for Sports games.
4. Conclusions on user profiles:
- User profiles in North America and Europe are similar, except for platform preferences. PS is more popular in Europe, while Xbox is more popular in America.
- The most popular genres in Europe and North America are Action, Shooter, and Sports. The most common rating is M.
- The user profile in Japan differs significantly from Europe and North America:
- Only local platforms (PS and Nintendo) are in the top 5, with Xbox not making the list. The most popular platform in Japan is the portable 3DS.
- The most popular genre is Role-Playing, and Fighting games made it to the fifth position.
- Many local games that have not been released internationally account for over half of the market.
- The most popular games have ratings of E and T. The M rating ranks third, excluding "Undefined."
5. Generalized user profiles:
- North America: Users are over 17 years old, prefer American products, enjoy playing at home, prefer active games (Action, Shooter), and have an interest in sports.
- Europe: The average user profile is similar to North America, with the exception that they are not tied to a specific country as the platform manufacturer.
- Japan: The average user is a school student who enjoys playing games on the way to school or at school, prefers Japanese games and platforms, enjoys creating their own characters in games and associating themselves with them. They also have a higher preference for Fighting games.  

Overall, this analysis provides valuable insights into the video game market, platform preferences, genre profitability, and user profiles in different regions. These findings can inform marketing and development strategies for video game companies.
    
### Summary  

The key criteria for a successful game worldwide in 2017 are as follows:

- The game should be released for platforms such as PS4 and XOne. For localization in Japan, considering releasing the game for portable platforms would be beneficial.
- The game should fall into the Shooter, Platform, or Sports genres. While the Action genre is popular among users, its median sales are lower compared to the previously mentioned genres.
- The game should have an M rating for North America and Europe. When releasing a game in Japan, consider lowering the rating to E.  

These findings can guide game developers and publishers in making strategic decisions regarding platform selection, genre focus, and rating considerations to maximize the success of their games in the global market.
