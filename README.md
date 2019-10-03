# LSTM-TFIDF
## LSTM over time series text data. 

This contains a notebook and steps to explain how to implement a LSTM over a time series data of text notes.
The dataset has been modified from the original yelp-reviews dataset. Only 10,000 reviews have been considered for the sake of this notebook. [This](https://www.kaggle.com/yelp-dataset/yelp-dataset) is the link to the original dataset.
I have changed the dataset for this notebook. The changed dataset has also been uploaded in this repo.

### Description of the dataset
The dataset contains reviews of multiple hotels. I have added a unique hotel id for the reviews and modified the dates such that only one review is posted everyday. 

The original dataset also contained the column as "stars". I have added another column based on this, if the stars given to a hotel id are less than 2, then the hotel is shut down and if the stars are greater than 2 then it is still open.

Consider that you want to predict if a hotel will shut down or not based on the time series of reviews. Multiple reviews would then be associated with a single hotel id. The notebook essentially explains this whole thing. 

It shows how to use LSTM to the above, i.e predict something on a time series of text data. 
