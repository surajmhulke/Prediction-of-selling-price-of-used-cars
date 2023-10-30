# Prediction-of-selling-price-of-used-cars

The Problem
The prices of new cars in the industry is fixed by the manufacturer with some additional costs incurred by the Government in the form of taxes. So, customers buying a new car can be assured of the money they invest to be worthy. But due to the increased price of new cars and the incapability of customers to buy new cars due to the lack of funds, used cars sales are on a global increase (Pal, Arora and Palakurthy, 2018). There is a need for a used car price prediction system to effectively determine the worthiness of the car using a variety of features. Even though there are websites that offers this service, their prediction method may not be the best. Besides, different models and systems may contribute on predicting power for a used car’s actual market value. It is important to know their actual market value while both buying and selling.

The Client
To be able to predict used cars market value can help both buyers and sellers.

Used car sellers (dealers): They are one of the biggest target group that can be interested in results of this study. If used car sellers better understand what makes a car desirable, what the important features are for a used car, then they may consider this knowledge and offer a better service.

Online pricing services: There are websites that offers an estimate value of a…

Now-a-days, with the technological advancement, Techniques like Machine Learning, etc are being used on a large scale in many organisations. These models usually work with a set of predefined data-points available in the form of datasets. These datasets contain the past/previous information on a specific domain. Organising these datapoints before it is fed to the model is very important. This is where we use Data Analysis. If the data fed to the machine learning model is not well organised, it gives out false or undesired output. This can cause major losses to the organisation. Hence making use of proper data analysis is very important.

About Dataset:

The data that we are going to use in this example is about cars. Specifically containing various information datapoints about the used cars, like their price, color, etc. Here we need to understand that simply collecting data isn’t enough. Raw data isn’t useful. Here data analysis plays a vital role in unlocking the information that we require and to gain new insights into this raw data.

Consider this scenario, our friend, Otis, wants to sell his car. But he doesn’t know how much should he sell his car for! He wants to maximize the profit but he also wants it to be sold for a reasonable price for someone who would want to own it. So here, us, being a data scientist, we can help our friend Otis.
Let’s think like data scientists and clearly define some of his problems: For example, is there data on the prices of other cars and their characteristics? What features of cars affect their prices? Colour? Brand? Does horsepower also affect the selling price, or perhaps, something else?

As a data analyst or data scientist, these are some of the questions we can start thinking about. To answer these questions, we’re going to need some data. But this data is in raw form. Hence we need to analyze it first. The data is available in the form of .csv/.data format with us


Process to convert .data file to .csv:

open MS Excel
Go to DATA
Select From text
Check box tick on comas(only)
Save as .csv to your desired location on your pc!
Modules needed:

pandas: Pandas is an opensource library that allows you to perform data manipulation in Python. Pandas provide an easy way to create, manipulate and wrangle the data.
numpy: Numpy is the fundamental package for scientific computing with Python. numpy can be used as an efficient multi-dimensional container of generic data.
matplotlib: Matplotlib is a Python 2D plotting library which produces publication quality figures in a variety of formats.
seaborn: Seaborn is a Python data-visualization library that is based on matplotlib. Seaborn provides a high-level interface for drawing attractive and informative statistical graphics.
scipy: Scipy is a Python-based ecosystem of open-source software for mathematics, science, and engineering.



In the return output we see question marks and its data type is "object" , so this ? qustion mark indicate it is NaN Value.
It is necessary to convert this ? question marks to NaN standard format.
Because it is generate some confusion because its data type is "object" and at isna().sum() function there is also shows
there is not available of NaN values.
So we replace ? Question mark into NaN Value.

We check both Mean and Median for "normalized-losses" column but Mean value is slighter greater than Median.
This is because of availablity of some Outliers.
So we use Median to fill the NaN Values.
df["normalized-losses"] = df["normalized-losses"].fillna(df["normalized-losses"].median()).astype(int)
# we fill the NaN Values by Median of "normalized-losses" column and converted into "int" data type


# 9. Training Data Evalution

MSE is: 4974235.837890235
RMSE: 2230.299495110519
MAE is: 1585.3408437358958
r2 score is : 0.9223636932435281

we can say we are having 92 percent accuracy for this model...
