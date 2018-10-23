# Background

This machine learning challenge came to me from a friend. He and I were discussing some challenges he saw in the retail space and I wanted to see how I would create a machine learning model to help retailers with loss prevention (or theft of product).

# Data Analysis

A machine learning algorithm is only as good as the data you feed it. If you do not understand the data, misinterpret what the data is telling you or miss important correlations, the algorithm will probably be useless. This is the main reason my most machine learning experts spend 75% of their time on the data.

## How much loss occurs

In my discussions with several people who are executives in retail organizations, I was surprised to find out that they can only estimate stock loss which results from theft. This means we need to create a model that estimates how much loss occurs, considering the following data:

1. How much stock is written off by the organization
2. How much of the stock that is written off is spoilage (the stock existed when it was written off)

The difference between these two values would constitute what I would define as "Unknown Stock Loss" or USL for short. i.e. stock that was purchased but no longer exists in the business.

We then need to break the USL into its component products to find out which products

We then create a model to compare "Unknown Origin Loss" between stores to get an idea of how each store compares.

We use the data for each store to compare against the following data:

1. Population numbers around the store.
2. Turnover of each store
3. The area the store services
4. The educational levels of the population
5. The income levels of the population

This analysis should give us a good idea if there are correlations between "Unknown Origin Loss" and the above metrics. If there isn't, it means that we need to investigate other metrics that might be correlated with a higher incidence of loss.

One of the main issues with stock loss is that the data is only entered sporadically. It might be easier to understand the implications, if we contrast this information with sales of product which is recorded at the checkout.

# Real time analysis

Video analysis will allow us to create a database of customers who may be shoplifting:

Customers who visit areas in the store that store products that are shoplifted more often than the baseline. For example, most people do not need to buy razors every week.

To work out if theft is occurring in real time we can use video to detect human beings who are putting product in their clothing.

While neither of these metrics tell us perfectly if theft is occurring, you can assume that people who shoplift, will shoplift again. This means that the system can create a database of "positive" occurrences and then look for those people again when they enter the store.

Customers the algorithm has not seen before may be more likely to be shoplifting.

