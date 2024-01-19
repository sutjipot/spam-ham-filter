# spam-ham-filter
A spam / ham email filter using naive Bayes filter.

## quick explanation
SpamHam Class: This class represents a Naive Bayes spam filter. It has the following attributes:

spam: A dictionary of occurrences for spam messages, where keys are words and values are counts.

ham: A dictionary of occurrences for ham (non-spam) messages, with a similar structure.

prior_spam and prior_ham: Prior probabilities for spam and ham messages, both initialized to 0.5.

The Naive Bayes probability calculations involve Laplace smoothing (adding 1 to both the numerator and denominator), and the logarithms of these probabilities are used to prevent underflow issues with very small probabilities.

The classification decision is made based on the value of logR: if it's greater than 0.5, the message is classified as spam; otherwise, it's classified as ham.
