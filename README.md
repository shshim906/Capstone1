## Capstone1

STEAM store has over 77,000 applications(this includes games, expansion packs, and ost packs etc) and a game company can often have a hard time standing out in those cluster without spending a good amount of money in marketing. This may not always be so easy especially if the company is small or the game they have appeals to a smaller number of people.
Recommender system is a great way for a product to get a little more boost in this regard, as it tries to appeal to the very players that are likely to find the game interesting. By analyzing the customer and the game to suggest games that the customers are more likely to be attracted to, we can increase the sale of the product and save a little more money on marketing.

1. Data pull

Capstone 1 - Data Pull

Steam allows collection of review data using API.
The maximum number of reviews that they provide per a game is 100 according to what they mention on their website.
As there are a lot of games on the platform, this takes a very long time.
The data therefore should be saved as pickle in the working folder

2. Data Clean and EDA

Capstone 1 - Data Clean and EDA

Remove duplicates and reviews that are missing the review text data.
Sometimes the reviews may be marked as "English" but the text is in another language.
Therefore a language detection library was used to remove text that were not written in English.
The rating are not included in the raw data, therefore sentiment analysis was implemented to identify either the review is positive or negative.
Exploratory data analysis was performed to see whether longer reviews are more likely to be positive or negative.

3. Recommendation system

Capstone 1 - Content based game recommendation

Cosine similarity was calculated to find games that are similar to the games that a player already owns and played for more than 30 minutes.
TF-IDF score was used to find the significant words in each game review text.

Capstone 1 - SVDpp Collaborative game recommendation

SVD++ algorithm was used to provide recommendation to players who are new to the platform and does not have review data to find similar games from.
