# Analyzing Text Similarity and Distortion Using Edit Distance
## Description
This method can be used to estimate how similar or dissimilar two texts representing two dialects of language, definitions of similar concepts across different disciplines or same news from two media sources are. Additionally the method also helps to distor text (using insertion, deletion, substitution and transposition operations) with personal information.
The method offers 3 edit distance variants (__Simple edit distance__, __Levenshtein edit distance__ and __Damerau-levenshtein edit distance__) and has the following operations:

- simple edit distance between two texts (at word level)
- simple edit distance between two texts (at character level)
- levenshtein edit distance (with substitution cost 2) between two texts (at word level)
- levenshtein edit distance (with submistution cost 2) between two texts (at character level)
- damerau-levenshtein edit distance between two texts (at word level)
- demarau-levenshtein edit distance between two texts (at character level)
- distorting or randomizing text for given number of spins of randomly picked operations (insertion, deletion, substitution and transposition)


The methods are defined in `utils.py` and are called on sample tweets from the notebook `text_edit_distance.ipynb`

The method in plain python without any package installation and therefore, preserving the environment or the `requirements.txt` file is not required. Random seeds are defined to have predictable random numbers for reproducibility.

## Keywords
edit distance, randomizing text, levenshtein edit distance

## Use cases
- __Comparing Textual Similarity Across Different Domains:__ This method can be used to compare how similar or different definitions, phrases, or terminology are across different domains or contexts. For example, a social scientist could use the Simple Edit Distance or Levenshtein Edit Distance (at the word level) to compare the terminology used in different areas of research, such as "transparency" in public policy vs. "transparency" in computer science. This can help identify variations in the usage or meaning of terms across various fields.
- Analyzing Dialects or Variants of Language: You can apply these methods to compare texts in different dialects of the same language or different stylistic variations of writing. For instance, comparing tweets or social media posts from different geographic regions using Damerau-Levenshtein Edit Distance might help identify subtle differences that also consider character transpositions in informal writing.

- __Evaluating Media Reporting on the Same Topic:__ Use edit distance to compare how two media outlets report on the same news story. If you're working with two different versions of the same article or report, the Levenshtein Edit Distance (Word Level) could highlight the differences in word choice and structure.

- __Text Distortion for Privacy or Anonymization:__ You can use this method to distort sensitive text data (like tweets or user-generated content) by applying random operations. This can help anonymize or distort text while maintaining its structural integrity for analysis.

## How to use
- run jupyter using command `jupyter lab` or `jupyter notebook`
- execute the notebook cells to call all methods defined in `utils.py` on same texts

## Sample input (For example to tweets)

```
tweet1 = "Excited to share our latest research on AI and its impact on social sciences! Leveraging data for better insights"
tweet2 = "Thrilled about our new findings on how AI transforms social science research. Innovation meets impact!"
```

## Sample output

```
simple edit distance at character 71, at word 16
levenshtein edit distance at character 109, at word 26
...
```

### Contact Details
Taimoor Khan (taimoor.khan@gesis.org)
