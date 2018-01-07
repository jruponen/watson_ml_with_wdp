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
3. Go to the project, "Assets" tab, and create a new Notebook (press 'New Notebook' in the Notebooks section)
4. Select "From URL", enter name (e.g House Price) and use this Notebook URL:
https://github.com/jruponen/watson_ml_with_wdp/blob/master/Predict%20House%20Price%20with%20Watson%20ML.ipynb
5. Follow the instructions on the Notebook, step-by-step

**Step 2 - Build a "Price Prediction" application to use your Watson ML model***  
1. In IBM Bluemix catalog (https://bluemix.net/catalog), deploy a "Node-RED starter" boilerplate, if not done already
2. When it is up & running, open your Node-RED application (go to your Node-RED app url, e.g https://jrnodered.mybluemix.net, or whatever URL you gave it)
3. Deploy Node-RED dashboard components by selecting "Menu" > "Manage Palette", go to "Install" tab and search for "node-red-dashboard"
4. Press "Install" next to node-red-dashboard component and wait for install to complete (your Node-RED will also restart)
5. Open the Node-RED flow template from the following URL and copy it's content on your clipboard:
https://raw.githubusercontent.com/jruponen/watson_ml_with_wdp/master/Node-RED_Predict-Price_app.txt
6. Switch back to Node-RED and import the flow by selecting Menu > Import > Clipboard
7. Paste clipboard content into the field and press the "Import" button
8. Double click on "Get params" node and paste your "ml_token" value here (you can find this in your Notebook)
9. Double click on "http request" node and paste your Watson ML REST API URL into the "URL" field
10. Finally, press "Deploy" on the Node-RED and go to your Node-RED app url with "/ui" extension, e.g:
https://jrnodered.mybluemix.net/ui (or whatever your Node-RED app URL is)

