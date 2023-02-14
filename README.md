This code is a modification of The Annotated Transformer http://nlp.seas.harvard.edu/annotated-transformer/

It is an exploration of transformer interpretability, and a tool to improve my understanding of the details of the transformer framework. It implements several methods for removing the effect of a specific word in an encoder-decoder transformer architecture. These methods are: 

1. Downweight all attention weights that involve the word
2. Delete the word
3. Replace the word with a blank token
4. Downweight the attention weights and replace the word with a blank token

It also implements a simple metric for measuring saliency of each word in the input relative to each word in the output. I am currently looking at the correlations between these methods, using the German to English translation tool from The Annotated Transformer as an example.
