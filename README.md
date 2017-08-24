# Animation_rec

Animation recommendation system by using collaborative filtering & contents based filtering


0. Outline

 I tried to make animation recommendation system by using 'hybrid filtering' which is combined CF & CBF. 
 Data I Used for this project is 'Anime Recommendations Database' which you can find on kaggle(https://www.kaggle.com/CooperUnion/anime-recommendations-database)
 
 
1. Data preprocessing

 First of all, i have to make rating matrix of users per animation and genre matrix of movies. The '-1' means that user saw the animation, but didn't rated the animation. So, i replaced that value with 0. Also by transfering dense matrix to sparse matrix this process made lots of NaN values, and for similarity calculating use I have changed it to 0. Finally i combined two matrices by key, 'user'.
 
2. Modeling
 
 I used cosine simularity to get K nearest neighbors. Cosine distance has strength in not sensitive in count numbers.
