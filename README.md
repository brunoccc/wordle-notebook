# wordle-notebook
A Jupyter notebook about Wordle. 
This is mostly an excuse for learning about Jupyter notebooks, Python, Pandas and Numpy.

Note that the solver do not interact directly with the game, it's supposed to be used manually by the user who follows the instructions and return the results.  

At every attempt, the solver is removing from the list all the words that do not comply with the result and returns the most probable word to try next.
Probability of words is calculated once for all in the first part of the notebook using the letters distribution: a word containing very frequent letters is considered "more probable" than one containing only rare letters. For example, since in the words list the most frequent letters appear to be S, E, A, O, R, the most useful word for starting could be "AROSE". 
Of course this assumes that the hidden words of the game have been decided randomly and not with other criteria (e.g. less common words, or words not widely known etc).

Special thanks to https://gist.github.com/prichey/95db6bdef37482ba3f6eb7b4dec99101 for providing the file with all the words. 
