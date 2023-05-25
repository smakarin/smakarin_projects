
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

### Общий вывод

В результате проведенного анализа были сделаны следующие выводы:
1. Комментарии по исследованию:
Для анализа были взяты данные, начиная с 2012 года. Более старые данные не актуальны из-за смены поколений игровых платформ;
2. Выводы по исследованию платформ:
    * Потенциально наиболее прибыльными в 2017 году платформами являются PS4 и XOne. Также не стоит упускать из виду платформы 3DS и WiiU, которые, очень популярны в Японии и также находятся в лидерах по продажам.
    * Продажи для PC держатся на одном уровне и не зависят от смены платформ;
    * Наибольшие медианные продажи приходятся на платформы PS3, PS4, X360, Xone. Чуть ниже располагаются Wii и WiiU;
    * Средний пользовательский рейтинг платформ XOne и PC равен.
3. Выводы по исследованию игр
    * Оценки критиков влияют на продажи игр, а оценки пользователей нет. Исключение - игр для платформ от компании Nintendo - WiiU, Wii, DS и 3DS;
    * Самое большое количество игр выпускается в жанре Action. Самым прибыльным жанром является жанр Shooter;
    * Жанр Platform входит в тройку по прибыльности, но находится в конце списка по количеству выпускаемых игр;
    * Средний пользовательский рейтинг игр жанра Action выше, чем у жанра Sports.
4. Выводы по изучению портрета пользователей
    * Портреты пользователей в Северной Америке и Европе похожи, за исключением предпочтений в выборе игровой платформы - в Европе больше любят PS, в Америке Xbox.
    * Наиболее популярные жанры в Европе и Америке это Action, Shooter и Sports. Наиболее популярный рейтинг - M.
    * Портрет пользователя в Японии очень сильно отличается от Европы и Северной Америки:
    * В топ-5 самых популярных входят только местные платформы (PS и Nintendo), Xbox нет в топ-5 - самой популярной платформой является портативная 3DS.
    * Самым популярным жанром является Role-Playing, а на пятое место попали игры Fighting.
    * Много локальных игр, которые не вышли на международный рынок и их продажи занимают больше половины рынка.
    * Самыми популярными играми являются игры с рейтингом E и T. Рейтинг M только на 3 месте, не включая неопределенный.
5. Обобщенные портреты пользователей
    * Северная Америка - старше 17 лет, предпочитает американские товары, любит играть дома, любит активные игры (Action, Shooter) и увлечен спортом;
    * Европа - средний пользователь похож на американского за исключением того, что не привязан к стране производителю платформ;
    * Япония - средний пользователь - школьник, который любит играть вне дома по пути в школу или в школе, любит японские игры и платформы, создавать своих персонажей в играх и ассоциировать себя с ними. Также больше остальных он предпочитает Fighting.  
    
### Резюме  

Основными критериями, определяющими успешность игры во всем мире в 2017 году будут:
* Игра выпущена для платформ PS4 и XOne, при локализации в Японии стоит подумать о выпуске игры для портативных платформ;
* Игра должна быть жанра Shooter, Platform или Sports. Жанр Action популярен среди пользователей, но его медианные продажи ниже перечисленных ранее.
* Рейтинг игры для Северной Америки и Европы должен быть обозначен, как М. При выпуске игры в Японии стоит подумать о снижении рейтинга до E.
