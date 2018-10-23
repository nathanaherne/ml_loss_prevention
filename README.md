# Background

This machine learning challenge came to me from a friend. He and I were discussing some challenges he saw in the retail space and I wanted to see how I would create a machine learning model to help retailers with loss prevention (or theft of product).

# Data Analysis

A machine learning algorithm is only as good as the data you feed it. If you do not understand the data, misinterpret what the data is telling you or miss important correlations, the algorithm will probably be useless. This is the main reason my most machine learning experts spend 75% of their time on the data.

## Data Correlations

To create a good machine learning model, we need to find quality correlations and quality is important. I am sure you have heard the saying "correlation doesn't equal causation", the saying exists because it is very important to understand why one event is related to another. A real world example is the stock price of [Berkshire Hathaway](berkshirehathaway.com) increases when a movie starring Anne Hathaway is released. If you wanted to use a machine learning algorithm to predict the stock price of Berkshire Hathaway, then it would be a good idea if the machine learning algorithm considered her upcoming movie releases. In saying this, there is no logical reasoning why movies starring a certain person should effect the stock price of a business. Alternatively, this correlation does show you the value of looking for all sorts of correlations in your available data, even completely random ones.

## How much loss occurs

In my discussions with several people who are executives in retail organizations, I was surprised to find out that they can only estimate stock loss which results from theft. This means we need to create a model that estimates how much loss occurs, considering the following data:

1. How much stock is written off by the organization
2. How much of the stock that is written off is spoilage (the stock existed when it was written off)

The difference between these two values would constitute what I would define as "Unknown Stock Loss" or USL for short. i.e. stock that was purchased but no longer exists in the business.

We then need to break the USL into its component products to find out which products are more likely to become USL.

We then create a model to compare USL between stores to get an idea of how each store compares with one another. There should be an even distribution (in percent) of USL products between stores. Deviations from a close to even distribution could point to some interesting correlations and could also help us to refine the dollar value of USL (products that are written off for other reasons)

We use the data for each store to compare against the following data:

1. Population numbers around the store.
2. Turnover of each store
3. The area the store services
4. The educational levels of the population
5. The income levels of the population
6. Weather

This analysis should give us a good idea if there are correlations between USL and the above metrics. We should find that there are some good correlations on which to build our model.

One of the main issues with stock loss is that the data is only recorded sporadically, when a stock take is done. This means we do not get up to the minute data like sales.

Once we have found correlations with our data, we should be able to create a model to predict USL.


# Real time loss prevention

Once we have good baseline information about stock loss in the organization, we can use this information to implement an algorithm to manage stock loss in real time.

## Video analysis

Video analysis will allow us to create a database of people (customers/staff etc) who may be stealing.

We create a baseline travel model that monitors the movement of customers and staff throughout the store. We use this information to help us track normal movement within the store (which can be useful for much more than just )

We use the system to flag customers who visit areas in the store that have products that are stolen more often than the baseline. For example, most people do not need to buy razors every week.

To calculate out if theft is occurring in real time we can use video to detect human beings who are putting product in their clothing.

While neither of these metrics tell us perfectly if theft is occurring, we can assume that people who steal, will most likely steal again. This means that the algorithm can create a database of "possible theft occurrences", look for those people again when they enter the store and monitor their movements.

Customers the algorithm has not seen before may be more likely to be shoplifting.

This system can be used to notify loss prevention officers of possible offenders.

