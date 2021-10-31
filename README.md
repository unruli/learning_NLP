# learning_NLP
Data comes in many different forms: time stamps, sensor readings, images, categorical labels, and so much more. But text is still some of the most valuable data out there for those who know how to use it. Natural Language Processing (NLP), I will use the leading NLP library (spaCy) to take on some of the most important tasks in working with text.

spaCy is the leading library for NLP, and it has quickly become one of the most popular Python frameworks. Most people find it intuitive, and it has excellent documentation.

spaCy relies on models that are language-specific and come in different sizes. You can load a spaCy model with spacy.load.

A common task in NLP is text classification. This is "classification" in the conventional machine learning sense, and it is applied to text. Examples include spam detection, sentiment analysis, and tagging customer queries


                      Bag of Words
Machine learning models don't learn from raw text data. Instead, you need to convert the text to something numeric.

The simplest common representation is a variation of one-hot encoding. You represent each document as a vector of term frequencies for each term in the vocabulary. The vocabulary is built from all the tokens (terms) in the corpus (the collection of documents).

As an example, take the sentences "Tea is life. Tea is love." and "Tea is healthy, calming, and delicious." as our corpus. The vocabulary then is {"tea", "is", "life", "love", "healthy", "calming", "and", "delicious"} (ignoring punctuation).

For each document, count up how many times a term occurs, and place that count in the appropriate element of a vector. The first sentence has "tea" twice and that is the first position in our vocabulary, so we put the number 2 in the first element of the vector. Our sentences as vectors then look like

v1v2=[22110000]=[11001111]
 
This is called the bag of words representation.
