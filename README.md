# Book-Recommendation-System
![image](https://www.bmscw.edu.in/images/library/lib_overview.jpg)
During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys. In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries). Recommender systems are really critical in some industries as they can generate a huge amount of income when they are efficient or also be a way to stand out significantly from competitors. The main objective is to create a book recommendation system for users.
## Content:

The Book-Crossing dataset comprises 3 files.


● Users
Contains the users. Note that user IDs (User-ID) have been anonymized and map to
integers. Demographic data is provided (Location, Age) if available. Otherwise, these
fields contain NULL values.


● Books
Books are identified by their respective ISBN. Invalid ISBNs have already been removed
from the dataset. Moreover, some content-based information is given (Book-Title,
Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web
Services. Note that in the case of several authors, only the first is provided. URLs linking
to cover images are also given, appearing in three different flavors (Image-URL-S,
Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the
Amazon website.


● Ratings
Contains the book rating information. Ratings (Book-Rating) are either explicit,
expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit,
expressed by 0.

## Data Pipeline:

Exploratory Data Analysis (EDA): In this part we have done some EDA on the features to see the trend.

Data Processing: In this part we went through each attributes and encoded the categorical features.

Model Creation: Finally in this part we created the various models. These various models are being analysed and we tried to study various models so as to get the best performing model for our project.

## Data Description

Users_dataset: Contains the users information 

User-ID (unique for each user) 

Location (contains city, state and country separated by commas) 

Age Shape of Dataset - (278858, 3)

## Books_dataset:

● ISBN (unique for each book) 			

● Book-Title 

● Book-Author 	

● Year-Of-Publication 

● Publisher 						

● Image-URL-M 						

● Image-URL-S 					

● Image-URL-L 						

● Shape of Dataset - (271360, 8) 

## Ratings_dataset:
Contains the book rating information. 

User-ID ISBN

Book-Rating 

Shape of Dataset - (1149780, 3) 


## Models Performed:

Popularity Based Recommendation

Model based collaborative filtering

Collaborative Filtering-(Item-Item based)

Collaborative Filtering-(User-Item based)


## Conclusion

In EDA, the Top-10 most rated books were essentially novels. Books like The Lovely Bone and The Secret Life of Bees were very well perceived.

Majority of the readers were of the age bracket 20-35 and most of them came from North American and European countries namely USA, Canada, UK, Germany and Spain.

If we look at the ratings distribution, most of the books have high ratings with maximum books being rated 8. Ratings below 5 are few in number.

Author with the most books was Agatha Christie, William Shakespeare and Stephen King.

We can conclude that item-item based collaborative filtering performed better than user-user based collaborative filtering because of lower computation among the memory based approach.

For modelling, it was observed that for model based collaborative filtering SVD technique worked way better than NMF with lower Mean Absolute Error (MAE)


## Future Scope

The future of recommender systems lie in integrating self actualization to do justice to serendipity while recommending which will also support rather than replace human decision-making by understanding preferences.

Recommender systems can be broadly divided into : Collaborative filtering, Content-based filtering, Hybrid recommender systems, Personality-based recommender systems. Each type of filtering algorithm is used according to the specific need of the application or the product. 

Here we are trying to achieve a recommendation which is not extremely personalised which may feel intrusive to the user and not very generic that it doesn’t really account the user’s distinct taste. Striking a balance between the two is what needs to be achieved. 

Furthermore there will be plenty of work needed to be done on the famous ‘cold start problem’ in order to somehow manage collecting just the right amount of implicit information and data to recommend users even if there is little or no direct information available on users.
