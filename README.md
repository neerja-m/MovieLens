
# Movie Lens 

## Business Context:

MovieLens is a company in the internet and entertainment domain providing an online database of information related to films, television series, and online streaming content including cast, production crew, trivia, ratings, fan, and critical reviews. Every year in collaboration with a guest curator, MovieLens publish their annual insights based on a theme providing a comprehensive view of a topic. The company is planning to bring out the "Movie Talkies: Classic" edition this year. The idea is to connect with viewers who have strong movie preferences as well as promote classic movies to attract newer customers and expand their viewer base.

## Problem Statement:

In order to create the "Movie Talkies: Classic" edition, the challenge lies in effectively analyzing and presenting a wealth of information about movies from a bygone era. The core issue is understanding the characteristics of these classic movies, user interests, and the relationship between user demographics and movie ratings. Without clear visuals, it's difficult to identify patterns, draw meaningful conclusions, and engage the audience on a deeper level. You have been hired as a Data Analyst by the company, to create a report that provides a detailed analysis of the classic movies that were released till 2000. The dashboard should provide insights on the following questions:

### Steps followed: 
The 3 CSV files comprising of the dataset were loaded into Power Query. The data was cleaned and transformed to remove redundant columns, and validated using the Power Query features. The data model was verified for integrity using the Column tools.
Genres were analyzed and a calculated column using DAX was created to group multiple pipe-delimited genres into a broader category for analysis purposes,  for example, the fields Action, Action|Adventure, Action|Thriller were grouped as “Action based”. A DAX function was also used to create a column that bucketed the release years of movies into decades to support meaningful analysis. Another column with DAX was created to classify users into 5 categories based on their ages. 

Card visuals were used to display the total number of movies released, number of users and the total genres. A donut chart to visualize the gender distribution, a gauge chart for the average rating, and a pie chart to highlight preference of movies, which could be filtered by gender using a drop-down slicer were other visuals used. Slicers were added to filter results by decade and gender, which were synced across other pages. Cross-filters were adjusted to keep results of card visuals constant. 

![Page1](https://github.com/user-attachments/assets/fb9aa534-0f82-46c3-ba40-6bd7ae35a353)

A clustered column chart was used to visualize the distribution of users across age groups based on their gender. For the location of these users, the map chart, along with bubbles to indicate the number of users in each location was used. A matrix visual is used that summarizes the average ratings across professions and age groups.

![Page2](https://github.com/user-attachments/assets/574bbc1e-fa19-4635-a691-c6bebfa801d6)

A treemap was used to display the Top N movies and genres with occupation and user age as additional slicers and the button feature to toggle between the two charts (genres and movies) was created with the help of bookmarks. A scatterplot between user age group and average rating, with number of users as the size of the bubble was used.

![Page3](https://github.com/user-attachments/assets/38e97294-534b-496b-923e-52be88cc025a)

Relevant slicers, filters, bookmarks, formatting, and page navigation features were used to enhance the report.
