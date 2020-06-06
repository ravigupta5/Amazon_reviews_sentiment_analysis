# Amazon_reviews_sentiment_analysis
### NLP project using LSTM
The aim is to predict positive or negative sentiment of user towards the product on the basis of review (text) given

### Each Dataset contains the following columns : 
-  marketplace       - 2 letter country code of the marketplace where the review was written.
-  customer_id       - Random identifier that can be used to aggregate reviews written by a single author.
-  review_id         - The unique ID of the review.
-  product_id        - The unique Product ID the review pertains to. In the multilingual dataset the reviews
                      for the same product in different countries can be grouped by the same product_id.
-  product_parent    - Random identifier that can be used to aggregate reviews for the same product.
-  product_title     - Title of the product.
-  product_category  - Broad product category that can be used to group reviews 
                      (also used to group the dataset into coherent parts).
-  star_rating       - The 1-5 star rating of the review.
-  helpful_votes     - Number of helpful votes.
-  total_votes       - Number of total votes the review received.
-  vine              - Review was written as part of the Vine program.
-  verified_purchase - The review is on a verified purchase.
-  review_headline   - The title of the review.
-  review_body       - The review text.
-  review_date       - The date the review was written
  
#### For the project, 'review_body' is the independent feature and 'star_rating' (converted to sentiment) is the target feature  
#### Ratings 4 & 5 are considered as positive while the rest considered as negative
  
  
## Data preprocessing:
- Tokenization, 
- Encoding 
- Padding

### Sample processed data:
32969 = it <br>
54898 = works<br>
9790 = but<br>
32969 = it<br>
54740 = has<br>
49098 = really<br>
20677 = bad<br>
52932 = sound<br>
7026 = quality<br>
68729 = the<br>
50265 = bass<br>
55075 = doesn<br>
64489 = t<br>
60067 = work<br>
715 = almost<br>
23034 = at<br>
58471 = all<br>

## Training the model
![alt text](https://github.com/ravigupta5/Amazon_reviews_sentiment_analysis/blob/master/accuracy_curve.PNG?raw=true)

## Sample Prediction
Input: ('I got the phone last week, till now its working fine. The build quality is okay. Performance at par with best in the segment')
Ouput: [[4.9882536]]
