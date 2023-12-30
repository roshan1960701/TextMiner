# Text Miner: WordCloud Generation and Analysis

![Wine Glass](https://github.com/roshan1960701/TextMiner/blob/main/Screenshot%202023-12-30%20at%2013.50.13.png)

![Word Cloud](https://github.com/roshan1960701/TextMiner/blob/main/Screenshot%202023-12-30%20at%2013.49.45.png)

## Introduction
The Text Miner is a Python-based application focused on creating WordClouds for various types of wines (41 in total) and for all records (3057) available. It includes a function that retrieves the top 5 most used words from each description and converts the list of words into a string for WordCloud generation. 

## Functionality
- **WordCloud Generation**: Produces WordClouds for individual wine types and all records.
- **Top 5 Words**: Extracts the most frequently used 5 words from each description.
- **String Conversion**: Converts the list of words into strings for visualization.
- **Custom WordClouds**: Implements masking to display words in specified shapes.

## Creating wordCloud for each type of wine (41 wines)
- The dataset contains 41 unique wine varieties. Utilizing the `unique()` function and `len()` function, we confirm this count.
- A function `generateWordCloud()` is created to produce word clouds for each wine type based on their descriptions. The function iterates through each type, converts descriptions to strings, and generates individual word clouds for each wine type.

## Creating wordCloud for all records (3057)
### Creating a function to get most 5 used Words from each description
- `wordGenerator()` function fetches the top 5 words from each description in the dataset, accumulating a total of 15,285 words.
- The list of words is converted into a string using a loop to concatenate each word into a single string.

### WordCloud for All records with most common used words from each description
- A WordCloud representing the combined most frequently used words from all descriptions is generated. Parameters such as width, height, background color, and max words are defined to visualize the word cloud.
- An attempt to mask the word cloud into a wine glass shape is made by utilizing an image as a mask for the WordCloud generation.



## References
- [Analytics Vidhya: Creating Customized Word Cloud in Python](https://www.analyticsvidhya.com/blog/2021/08/creating-customized-word-cloud-in-python/): Provides insights into creating personalized WordClouds in Python.
- [Stack Overflow: Increase Resolution with WordCloud and Remove Empty Border](https://stackoverflow.com/questions/28786534/increase-resolution-with-word-cloud-and-remove-empty-border): Offers solutions to improve WordCloud resolution.
- [Medium: WordClouds - Basics of NLP](https://medium.com/@harinisureshla/wordclouds-basics-of-nlp-5b60be226414): A basic guide to WordClouds and their relation to Natural Language Processing (NLP).
- [DataToFish: Substring Pandas DataFrame](https://datatofish.com/substring-pandas-dataframe/): Useful resource for substring operations in Pandas DataFrame, possibly relevant for data manipulation before generating WordClouds.
