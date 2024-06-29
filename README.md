## Professional Certification in AI/ML
### Practical Application Assignment 11.2
### [Jupyter Notebook Link](https://github.com/Raesu/pcmlai-mod11/blob/main/prompt_II.ipynb)

#### Introduction
Based on the data set you shared, I used linear regression to build and test many models to predict the price of a car. The objective was to allow you to input several pieces of information (year of the car, fuel type, odometer reading, manufacturer, etc) and the model would predict the price it would sell for. This is based on the data you shared so it will maintain any bias that was in that data set (pricing dynamics related to car information).

#### Results
I ended up with a model that was able to estimate the price of a car that was about $20 off the truth in the training set. This means that with new unseen data, we can expect that the price output will be close to the final price. However, there is a lot of variation in the estimates and there is a chance that the model can produce a number far above or far below the market price.

One characteristic of the model is that it overestimates cheap cars, and underestimates more expensive cars. So for cars at the higher and lower end of your price ranges, I'd suggest further validation for pricing.

The top drivers of price are the year, the odometer reading, and fuel types. Manufacturers are also important, especially (Kia, VW, Hyundai, and American-made cars).

#### Usage Guidance
To deploy this model, I would input the necessary information ('region','manufacturer','fuel','title_status','transmission','state', 'year', 'odometer') and the price output as a starting number for the listing. You should sanity check the price (compare against other similar cars), and adjust as you see fit. The market price is always moving and salesmanship also plays a big role, so use this price output as guidance.

#### Next Steps
I would want to walk through all the data cleaning steps I did and make sure I did not make any rash decisions. You know the business better than me and having intuitive sense of what is important will help me build a better model.