Movie Recommendation System

A personalized movie recommendation engine built using collaborative filtering techniques on the MovieLens dataset. This project was developed as part of a 1-day hands-on Data Science Masterclass by PW Skills, focusing on how platforms like YouTube and Netflix personalize user content using recommendation algorithms.

Objective :
To simulate a real-world movie recommendation engine that predicts user preferences based on historical interactions and provides relevant movie suggestions using both user-based and item-based collaborative filtering.

Key Concepts Explored :
1. User-Item Interaction Matrix – Building a sparse matrix to represent user ratings
2. Memory based Collaborative Filtering
3. Similarity Metrics
   - Pearson Correlation: Measures linear correlation between rating vectors
   - Cosine Similarity: Evaluates angle-based similarity between vectors
4. Dimensionality Reduction using SVD (Singular Value Decomposition)
   - Applied to reduce noise and improve latent feature extraction
5. Handling Data Sparsity – Filtering users/items with low activity to improve model performance
6. Cold Start Problem – Recognizing limitations when new users/items lack historical data
7. Real-time Recommendation Logic – Building Top-N recommendations dynamically based on input

Features Implemented :
1. Data preprocessing and merging movie metadata
2. Matrix construction: User-Movie interaction matrix
3. User-based collaborative filtering
4. Item-based collaborative filtering
5. Similarity calculation (Pearson & Cosine)
6. Top-N movie recommendations for selected users
7. Visual representation of user activity

Tech Stack :
This project was developed using Python 3 in a Jupyter Notebook environment. Core libraries include Pandas and NumPy for data manipulation, Scikit-learn for similarity computations and dimensionality reduction (using `cosine_similarity` and `TruncatedSVD`), and Matplotlib and Seaborn for data visualization. The recommendation system is based on memory based collaborative filtering

How it Works (Algorithm Flow) :

1. Load and preprocess the dataset
2. Construct a pivot table with users as rows and movies as columns
3. Compute similarity using Pearson or Cosine between users or items
4. Sort neighbors by similarity scores and filter highly correlated entries
5. Recommend Top-N movies not yet rated by the user
6. Optionally apply SVD to reduce dimensions and improve prediction accuracy
   
Dataset Overview :
The project uses the MovieLens 100K dataset from GroupLens Research, which contains 100,000 movie ratings from 943 users across 1,682 movies. Ratings range from 1 to 5. The data was loaded from two files: `u.data` (user ratings) and `Movie_Id_Titles.txt` (movie ID-to-title mapping). The dataset is ideal for building and testing recommendation systems.

Acknowledgements :
Thanks to PW Skills for the masterclass on “How YouTube Personalizes Content” and mentors and instructors who made the project possible

Connect : 
Feel free to connect or reach out for suggestions, contributions, or collaborations!

LinkedIn - https://www.linkedin.com/in/s-shubham-317359229
Email - sshubham22062003@gmail.com
