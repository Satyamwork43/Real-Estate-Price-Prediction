
# HOUSING: PRICE PREDICTION
# Problem Statement:
Houses are one of the necessary need of each and every person around the globe and therefore housing and real estate market is one of the markets which is one of the major contributors in the world’s economy. It is a very large market and there are various companies working in the domain. Data science comes as a very important tool to solve problems in the domain to help the companies increase their overall revenue, profits, improving their marketing strategies and focusing on changing trends in house sales and purchases. Predictive modelling, Market mix modelling, recommendation systems are some of the machine learning techniques used for achieving the business goals for housing companies. Our problem is related to one such housing company. A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. The company is looking at prospective properties to buy houses to enter the market. You are required to build a model using Machine Learning in order to predict the actual value of the prospective properties and decide whether to invest in them or not. For this company wants to know: • Which variables are important to predict the price of variable? • How do these variables describe the price of the house?

# Business Goal:
You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for the management to understand the pricing dynamics of a new market.

# EDA
![image](https://user-images.githubusercontent.com/78307104/132952323-5ed08176-8aaa-4279-9cc5-28ae1f99c013.png)

# Obseravtion

1-From MSZoning i can say most of the people like house that have zone Residential Low Density, low density says people like to live in more space like villas

2-From Street i can say most of the people like to have home that are paved

3-From Type of alley access to property i can say mostly people like to have home at grvl

4-From lotshape i can say mostly people like reg and very less people who like to live in IR2,IR3

5-From LandContour: Flatness of the property i can say mostly people like to live in Near Flat/Level

6-From Lot configuration i can say mostly people like inside lot and some people like 20% of people like corner plot

7-From LandSlope: Slope of property i can say mostly 90% of people like Gentle slope

8-From Neighborhood: Physical locations within Ames city limitsi can say mostly people like to have have at North Ames after this people also like College Creek

9-From Condition1: Proximity to various conditions i can say mostly people like Normal and same with condition 2

10-From BldgType: Type of dwelling i can say mostly people like Single-family Detached


![image](https://user-images.githubusercontent.com/78307104/132952375-aab283ab-0a62-41c5-a227-6c81a62e122f.png)
![image](https://user-images.githubusercontent.com/78307104/132952418-d15e716e-cd7d-470d-af79-f1a86354f81f.png)
# Observation

1-Total Rooms Above Ground-As the room no. increasing the average price is also increasing till 11th room after that price start decreasing

2-Bedroom ABove Ground-For the 0,4,8 Bedroom price is high and price is very less for 6 and 2

3-Kitchen Above Ground-as the no of kitchen is increasing the price is reducing and mostly people take one kitchen only

4-In Basement full bathrrom and half bathrooms as the bathroom size increasing the price is also increasing

5-Fireplaces-As the fireplaces increasing the sale price is also increasing

6-PoolArea-as big the pool the more costly the house
![image](https://user-images.githubusercontent.com/78307104/132952450-38c37613-58a0-490e-86de-003154ed254f.png)
# Observation
3-Street-For flat stones or bricks access,Price is higher and majority of houses with gravel have price around 2 lakhs but as there is very less data for gravel street type this feature is not that important

4-LotShape-We can see that houses with regular Shapes have low price and as the irregularity increases, the average sale price of the house also increases

![image](https://user-images.githubusercontent.com/78307104/132952482-07f570e9-aae3-4441-ad83-0a92ffcc6942.png)
![image](https://user-images.githubusercontent.com/78307104/132952492-1f9337e2-d76f-4211-b0fd-d298ebb93d84.png)
# Obseravtion
WE can see that the houses and garage which were built during 0s have less sale price than the newer ones

with every year,house price increases

But if see,Year Sold feature the price fall down with each year which is strange.

Due to the strange behaviour in year sold,we subtract each feature with year sold

# Finally i trained many model but lightgbm was giving me good accuracy from all of them so here is the final learning curve and metrics

![image](https://user-images.githubusercontent.com/78307104/132952610-f082d1b2-d21b-484b-863c-aa8e5544bb9c.png)
