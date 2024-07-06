# Beer-Recommender-System
Building a Crowdsourced Recommender System
# Objective 
The objective of this project is to create the building blocks of a crowdsourced recommender system. It should accept user inputs in the form of desired attributes of a product and come up with 3 recommendations. 
Obtain reviews of craft beers from beeradvocate.com. 
https://www.beeradvocate.com/beer/top-rated/

Task A. Extract about 5-6k reviews. 

Task B. Assume that a customer, who will be using this recommender system, has specified 3 attributes in a product. E.g., one website describes multiple attributes of beer (but you should choose attributes from the actual data)
https://www.dummies.com/food-drink/drinks/beer/beer-for-dummies-cheat-sheet/
•	Aggressive (Boldly assertive aroma and/or taste) 
•	Balanced: Malt and hops in similar proportions; equal representation of malt sweetness and hop bitterness in the flavor — especially at the finish
•	Complex: Multidimensional; many flavors and sensations on the palate
•	Crisp: Highly carbonated; effervescent
•	Fruity: Flavors reminiscent of various fruits or Hoppy: Herbal, earthy, spicy, or citric aromas and flavors of hops or Malty: Grainy, caramel-like; can be sweet or dry
•	Robust: Rich and full-bodied

Task C. Perform a similarity analysis using cosine similarity (without word embeddings) with the 3 attributes specified by the customer and the reviews. 

Task D. For every review, perform a sentiment analysis (using VADER or any LLM). 

Task E. Create an evaluation score for each beer that uses both similarity and sentiment scores. 
Now recommend 3 products to the customer. 

Task F. How would your recommendation change if you use word vectors (e.g., the spaCy package with medium sized pretrained word vectors) instead of the plain vanilla bag-of-words cosine similarity? One way to analyze the difference would be to consider the % of reviews that mention a preferred attribute.

Task G. How would your recommendations differ if you ignored the similarity and feature sentiment scores and simply chose the 3 highest rated products from your entire dataset? Would these products meet the requirements of the user looking for recommendations? Why or why not? 

Task H. Using the top four attributes of beer (from word frequency analysis), calculate the lifts between these attributes and any 10 beers in your data. Choose one beer, and find the most similar beer (among the remaining 9) using the lift values.

