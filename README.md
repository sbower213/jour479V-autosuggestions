# jour479V-autosuggestions
Final Project for JOUR479V at the University of Maryland by Rachel Dooley and Steven Bower

## How to Use
This project analyzes autosuggestions provided by Bing and Google across various TLDs and languages.
To obtain these autosuggestions, run the get_suggestions function with parameters: (tld, lang, filename, subjects, predicates) where

tld: a string representing the domain you wish to query (e.g. "com", "co.uk")

lang: the code of the language you wish to query (e.g. "en", "ru", "es")

filename: the name of the file for the results to be saved in (typically ending in ".csv")

subjects: a string array containing the nouns you wish to query

predicates: a string array containing the terms that you want to follow each noun in the queries


Once you have obtained the dataframe with your results, use the normalize_dataframe function to tokenize the terms.
After that, you can use the get_sentiment function with your dataframe and csv file to determine the various sentiment levels in the autosuggestions.
All of these results can be printed using the print_results function, and the most common terms in these autosuggestion results can be found with the get_most_common function.
To display these results using matplotlib charts, use the visualize function included at the end of the notebook.
Examples of these functions in use can be found in the autosuggest_collect.py.ipynb file, intended for use with ipython notebook.