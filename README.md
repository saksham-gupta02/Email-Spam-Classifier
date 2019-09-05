# Email-Spam-Classifier
This model will filter out the spam emails based on the words it is containing. A vocabulary is created with different 2500 words. And based upon this vocabulary and the probability of the words occurring in the mail. It will differentiate whether a mail is spam or Not. 

## Approach Used - Data Preprocessing
  First all the files has been read from the folder.
  from each mail only email body has been extracted.
  Remaining things like email header, sender information any html tag has been removed.
  Any missing body or irrelevant data is there has been removed.
  Words are stemmed using nltk stemmer.
  Punctuation from the mail was also removed.
  Than email body has been tokenized into words using nltk package.
  Vocabulary is created with top 2500 words which occurs the most.
  A Sparse matrix is generated and data was divided into train and test.
  and finally count the occurence of each word in one email for whole dataset.
  
## Making data Ready for Training
  A sparse matrix is created where each row contains the count of occurence of each word in email and vocabulary.
  Used Bayes Theorem.
  Then probability were calculated for SPAM emails, non spam emails.
  Probabilty of a word in spam email.
  Probability of a word in non spam email.
  Probability of a word being occur in the mail.
  
## Testing the model
  Model has been test on test data and performed very good with a f-1 score of 0.97
  
  
