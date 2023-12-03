### Business Understanding

The business I will be looking at creating a linear regression model for is King Real Estate. They are looking at purchasing some properties in the King's county area and a re looking for some direction and predictions at what the house prices will be depedning on certain features.

## Data Understanding

The dataset I will be using is the Kings County House sales dataset. 

This includes the following information for over 2000 properties:
 - ID
 - price
 - bedrooms
 - bathrooms
 - sqft_living
 - sqft_lot
 - floors
 - waterfront
 - view
 - condition
 - grade
 - sqft_above
 - sqft_basement
 - yr_built
 - yr_renovated
 - zipcode
 - latitutde
 - longitude
 - sqft_living15
 - sqft_lot15

Using this data I will advise King Real estate as to what features will affect the price of a house.

## Data Preparation
In preparation for modeling I have decided to drop some of the data to limit the dataset to what information I will be using. transformed the data to the Dtype i would require for certain models.

## Modeling

To begin the process I created a heatmap to determine a starting point on observing what house characteristics had high correlation with price.

![download](https://github.com/nysmitch/dsc-phase-2-project/assets/147038854/fcd930a6-a5a2-4b83-9be0-d23c30079273)

This showed the highest correlation with price being sqft_living with a smaller correlation with bathrooms and bedrooms.
![download](https://github.com/nysmitch/dsc-phase-2-project/assets/147038854/c4f6069d-e19f-4454-82ea-2f1410ae1c53)

After creating a regression model for the mean square footage of a zipcode and the price the following statistices were produced:


<img width="638" alt="image" src="https://github.com/nysmitch/dsc-phase-2-project/assets/147038854/0f0d5aed-c45c-4f39-8d7e-2b2d4ea5a0d3">


From this we can see that average square footage explains 59% of the variance in sales. 
This creates the following model of the regression:

![download](https://github.com/nysmitch/dsc-phase-2-project/assets/147038854/e8f5a8e1-3ea4-4dff-8c63-0a1879b2387a)




Following this I attempted to creae an SKLEARN predictive model which became severly affected by outliers.
![download](https://github.com/nysmitch/dsc-phase-2-project/assets/147038854/b36ea655-480f-4e24-966d-4b5095f81759)




These were removed from the data and model retested. This improved the RMSE of the model overall but not enough. I then tried scaling the 



