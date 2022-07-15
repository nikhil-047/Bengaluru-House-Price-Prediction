# Bengaluru-House-Price-Prediction

Built a model using sklearn and linear regression using the Bangalore home prices dataset from Kaggle. 
For creating the model I have used data science concepts such as loading and cleaning the data, outlier detection and removal, feature engineering, dimensionality reduction.For hyperparameter tunning ,I have used gridsearchcv, k fold cross validation.

Built a web app using HTML , CSS , JavaScript . which will allow a user to enter the home square ft area, bedrooms, bathroom and location it will call the python flask server to retrieve the predicted price.


Link For Dataset :- https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data

# How the web app works
1. After Training the model it is exported using pickle module and also the Location names will be exported as a json file
   Note :- The locations are exported because we need it for prediction as we need to have the columns in the same order that we had used to train.
2. Will create a file including functions to import the model and the location json file
3. Then from the UI we will get the user inputs 
4. Further we wil create a numpy array of zeros and replace the data in 0,1,2 index with the sqft area,bhk,bathroom .
   Based on the location selected by the user we will use the location json to get the index of it.And then in the numpy array we will replace the index of the location with "1" .Since we had used one hot encoding (for converting the Location names)
5. Get the predicted response and display to the user

# How to run the app
1. Download the folder
2. Navigate to server folder
3. Run the python file "server.py" in cmd (This will start the flask server)
4. Now run the HTML file "app.html"

# Dependencies
- Python
- Jupyter notebook
- Numpy and Pandas
- Matplotlib
- Sklearn
- Python flask for http server
- HTML/CSS/Javascript for UI

# What the app loks like

![house_price_prediction](https://user-images.githubusercontent.com/43903557/179243942-7b968f8c-9f83-4ce7-ba4f-c41e73e926fe.jpeg)

