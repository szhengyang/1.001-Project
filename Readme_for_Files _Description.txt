1. jan.csv, feb.csv,..., dec.csv
   
   Monthly raw data files after appending and joining operations (airline and weather data)
   using Tableau.

2. convertcsv.js

   Uses the npm package 'csvtojson' to convert csv files to json files. The output was
   monthly json files instead of a compiled one to avoid running into memory issues

3. jan.json, feb.json,..., dec.json

   Monthly raw data files after conversion from csv

4. googlechartvalues.js

   To derive key performance measures for use in google charts. Visualization is done 
   using both Google Charts and Tableau. Visualizations from both sources are incorporated
   using Google Charts API and Tableau Javascript API.

5. decisiontreeedited.js 
	
   Uses the npm package 'decision-tree'. The decision tree model will be running in the
   server, as specified by a separate file, testserver2.js.

6. regressiontrain.js

   Uses the NPM package 'ml-regression-multivariate-linear'. The coefficients of the 
   linear regression model is output into the coefficients.js file. 

7. coefficients.js

   Contains an array of coefficients for each of the variables and intercept. 

8. comparison.js

   To use regression model to generate predicted values using test sample. The predicted
   values will be subsequently compared with actual values using Tableau.  

9. app.js

   There are 2 main purposes of the app.js(server) file. The first is to allow the decision tree
   model to run in the background, so that the user interface is ready for user input at 
   any time. The second is to receive form data from the user interface. Form data and 
   prediction results are output to 2 files in the 'sourcehtml' folder, prediction.js and
   parameters.js.  

10.index.html (in 'sourcehtml' folder) 
 
   The home page of the website, which provides analysis on historical data and a form 
   for user input. 

11.prediction.html (in 'sourcehtml' folder) 

   Web page showing results of prediction according to user input, by requiring the 
   'prediction.js' and parameters.js' file. The regression calculations is also run within
   this page to find the length of delay if applicable. Also provides additional
   visual information for the user specific to input values. 