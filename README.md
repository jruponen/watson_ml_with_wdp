# Predict house prices with Watson ML

**Original sources:**  
Part 1: https://medium.com/ibm-watson-data-lab/watson-machine-learning-for-developers-b98cefb3f890
Part 2: https://medium.com/ibm-watson-data-lab/building-your-first-machine-learning-system-b3d9401927b7

**Modified by:** Jukka Ruponen /IBM, 2018-01-07  

**Explanation:**  
This exercise will show you how to build a very simple linear regression model to predict a house price, based on the sample data set that you use for training the model (with just few rows of data). In no way is this ment to be an accurate model but instead show the principle how it is done. In the last part of the exercise you'll deploy your trained model to Watson Machine Learning service, in order to make it available for app developer.

**Step 1 - Create the model and deploy to Watson ML**
1. Sign in to WDP: https://dataplatform.ibm.com
2. Create a new project
3. Go to the project, "Assets" tab, and create a new Notebook from URL
4. Follow the instructions on the Notebook, step-by-step

**Step 2 - Build a "Price Prediction" application to use your model***
1. In bluemix catalog (https://bluemix.net/catalog), deploy a "Node-RED starter" boilerplate if not done already
2. When up & running, open your Node-RED application (go to the app url) and deploy the sample flow
