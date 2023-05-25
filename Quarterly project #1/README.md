
## Predicting Video Game Popularity

### Toolkit

Data Preprocessing: handling missing values, table grouping, duplicate handling, pandas;
Data Visualization: seaborn and plotly;
Hypothesis Testing: scipy library. 

### Input Data

In this project, historical data about game sales, user and expert ratings, genres, and platforms (e.g., Xbox or PlayStation) are available from open sources.
There is labeled data: information about games, platforms, ratings, the number of copies sold, broken down by regions and age groups.

### Objective

To identify patterns in the sales of different genres and platforms. To define successful genres. To test proposed hypotheses.

### Project Structure  
1. Studying the general information in the available file.
2. Preparing data for analysis.
3. Exploratory data analysis:
    * Study of the number of games released per year;
    * Analysis of game sales on different platforms over time;
    * Determining the period based on which we can forecast for the year 2017;
    * Analysis of platforms and choosing the most promising ones;
    * Is there a difference in the sales of each game on different platforms?
    * How do user and critic reviews affect sales?
    * Analysis of the profitability of different genres.
4. Creating a user profile for each region:  
    * Top 5 most popular platforms;
    * Top 5 most popular genres;
    * Does the ESRB rating affect sales in a particular region?
5. Hypothesis testing:
    * Average user ratings for the Xbox One and PC platforms are the same;
    * Average user ratings for the Action and Sports genres are different.
6. Overall conclusion 

### Overall Conclusion

As a result of the conducted analysis, the following conclusions were drawn:
1. Comments on the research:
The data used for analysis starts from 2012. Older data are not relevant due to the change in generations of gaming platforms;
2. Conclusions on platform research:
    * Potentially, the most profitable platforms in 2017 will be PS4 and XOne. Also, one should not overlook the 3DS and WiiU platforms, which are very popular in Japan and are also leaders in sales.
    * PC sales remain at the same level and are not affected by platform changes;
    * The largest median sales are for PS3, PS4, X360, XOne platforms. Slightly below are Wii and WiiU;
    * The average user rating of the XOne and PC platforms is equal.
3. Conclusions on game research:
    * Critics' ratings affect game sales, while user ratings do not. The exception is games for Nintendo platforms - WiiU, Wii, DS, and 3DS;
    * The largest number of games is released in the Action genre. The most profitable genre is Shooter;
    * The Platform genre is among the top three in terms of profitability, but it is at the end of the list in terms of the number of games released;
    * The average user rating of Action games is higher than that of Sports games.
4. Conclusions on user portrait research:
    * User portraits in North America and Europe are similar, with the exception of preferences in choosing a gaming platform - Europe prefers PS, America prefers Xbox.
    * The most popular genres in Europe and America are Action, Shooter, and Sports. The most popular rating is M.
    * The user portrait in Japan is very different from Europe and North America:
    * The top 5 most popular include only local platforms (PS and Nintendo), Xbox is not in the top 5 - the most popular platform is the portable 3DS.
    * The most popular genre is Role-Playing, and Fighting games made it to the fifth place.
    * There are many local games that have not hit the international market and their sales occupy more than half of the market.
    * The most popular games are games with E and T ratings. The M rating is only in 3rd place, not including the unspecified.
5. Generalized user portraits:
    * North America - over 17 years old, prefers American products, likes to play at home, enjoys active games (Action, Shooter) and is into sports;
   * Europe - the average user is similar to the American one, except that he is not tied to the country of the platform manufacturer;
   * Japan - the average user is a schoolboy who likes to play outside of home on the way to school or at school, loves Japanese games and platforms, likes to create his characters in games and associate himself with them. He also prefers Fighting more than others.
    
### Summary  

The main criteria that will determine the success of a game worldwide in 2017 will be:
   * The game is released for PS4 and XOne platforms, when localizing in Japan consider releasing the game for portable platforms;
   * The game should be of the Shooter, Platform, or Sports genre. The Action genre is popular among users, but its median sales are lower than those previously listed.
   * The game's rating for North America and Europe should be marked as M. When releasing a game in Japan, consider lowering the rating.
