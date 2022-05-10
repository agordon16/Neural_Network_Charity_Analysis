# Neural_Network_Charity_Analysis
## Overview
The purpose of this exercise is to build a classification model to assist in determining whether or not a charitable venture will be successful if funded by Alphabet Soup.

# Results
## Data Preprocessing

* The target variable for our analysis is the success rate. Based on historical data on whether or not previous ventures invested in were successful or not can help determine the likelihood of success for similar ventures submitted for.

![target](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/98a48b2b011a7f0e53928e42810087703bcd6226/Images/TargetArray.jpg)

* Our feature variables consist of our categorical list after binning has been completed and several nonessential columns have been removed.

![features](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/98a48b2b011a7f0e53928e42810087703bcd6226/Images/Features_InputVariables.jpg)

* The variables EIN and NAME were removed from the dataset as they are individual identifiers only and hold no bearing on the data.

![initial_drop](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/98a48b2b011a7f0e53928e42810087703bcd6226/Images/InitialDrop.jpg)


## Compiling, Training, and Evaluating the Model

* For the initial model I selected two hidden layers with 8 & 5 neurons each respectively, using relu activation mode for the input layers and sigmoid for the output layer. Since this was an initial run of the model I elected to go with a fairly simple setup to start with and determine if further complexity was needed. 

![initial_model](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/98a48b2b011a7f0e53928e42810087703bcd6226/Images/InitialModel.jpg)

* Using the initial model I was unable to achieve the target model performance value of .75 or higher. This suggests that further optimization may be needed to achieve the target performance rate.

![initial)results](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/8d9a6a56016c1d55fb351731322cbe7e3ff8dde5/Images/InitialResults.jpg)

* To try and increase model performance I made various changes to the model such as varying the neuron values, adding more hidden layers, utilizing different activation modes, and dropping a few more columns that I did not feel were relevant to the model. 

![model1](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/8d9a6a56016c1d55fb351731322cbe7e3ff8dde5/Images/Optimize1.jpg)

![model2](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/8d9a6a56016c1d55fb351731322cbe7e3ff8dde5/Images/Optimize2.jpg)

![model3](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/8d9a6a56016c1d55fb351731322cbe7e3ff8dde5/Images/Optimize3.jpg)


# SUMMARY
Based on the initial model and subsequent optimizations, this dataset would require more scrutinization and alternative optimization iterations to achieve the required performance metrics. The initial run came in at right around 70.3% accuracy which falls below the optimal 75% threshold. Optimization models did not improve this score with the exception of the random forest classifier which improved only slightly at 72.5%.

![rf](https://github.com/agordon16/Neural_Network_Charity_Analysis/blob/0b405a62caafe90aa2c4b1cfa49ef4791afb32ce/Images/RandomForest.jpg)