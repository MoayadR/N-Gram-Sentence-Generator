# N-Gram-Sentence-Generator
 This code is designed to generate sentences using n-gram models (bigrams or trigrams) from the Brown Corpus provided by the NLTK library.


# Importing Necessary Libraries: The code imports necessary libraries including NLTK, regex, and random.
## Downloading the Brown Corpus: It downloads the Brown Corpus from NLTK if not already available.

## Text Preprocessing Functions:
* remove_special_chars(): Removes special characters from a string.
* limit_spaces(): Reduces multiple spaces to a single space.
* preprocess(): Applies both cleaning functions to a string.

## Tokenization: The tokenize() function splits the corpus into a list of unique tokens.

## Probability Calculation: The max_probability() function compares probabilities to find the best next word for the sentence.

## N-gram Sentence Generation:
* n_gram_generator(): Generates sentences using n-gram models (bigrams or trigrams). It builds sentences by probabilistically selecting the next word based on the previous n-1 words.

## Main Function:
* Collects user inputs for the number of sentences, n-gram type (bigram or trigram), and maximum sentence length.
* Preprocesses the Brown Corpus to a single cleaned string.
* Generates and prints the specified number of sentences based on the n-gram model.

## How It Works:
* Input: The user specifies the number of sentences to generate, the type of n-gram model (bigram or trigram), and the maximum length of each sentence.
* Preprocessing: The Brown Corpus is cleaned and preprocessed to remove special characters and excess spaces.
* Sentence Generation: The code generates sentences by selecting words based on their probabilities in the context of the previous n-1 words.
* Output: Generated sentences are printed to the console.

This script can be used for natural language processing tasks such as text generation, modeling language patterns, and studying probabilistic language models.