# data-mining-project
This is my Data mining course project and the things that I tried in it. As a part of our final project we were part of in-class Kaggle competition in which we had to predict airbnb lisiting booking rate (0=low, 1=high) from 66 other independent variables. We ended up winning the competition with AUC of 95.44. This repository has all the work I did or tried in the project.

airbnbFeatureEngineering1 : preprocessing of amenities and host since columns. Amenities column looked like this {TV,"Cable TV",Wifi,"Air conditioning",etc}. One new column was created for each of the amenities.

airbnbFeatureEngineering2 : preprocessing of all the other columns along with handling of missing values.

airbnbFeatureEngineering3 : topic modeling on description column using LDA.

airbnbModel : final xgboost model used along with hyperparameter tuning

point_of_interest: airbnb data had latitude and longitudes of each of the listings. This two features can be used to get the information about surrounding POI's.This is important beacause listings near tourist spots or cafes and restaurants has generally high booking rates. Thus count of these POI's can be obtained in given radius range arround the coordinates in order to determine the attractiveness of the location of the listing.  I have done it using overpass api and google api. Either can be used, overpass api is free but slow, google api can be expensive.( I did not use these features in the final model because of time constraints.)
