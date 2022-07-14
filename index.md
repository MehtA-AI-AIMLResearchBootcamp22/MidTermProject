# Midterm Project
By Ivy, Kam, William, Alex

## Features
Our features for this model were a bag of words for the pronouns, determiners, and punctuation marks, as well as the average number of words per sentence.

We first tried counting the number of pronouns, determiners, and punctuation marks, but found that the accuracy wasn't as good as it could be. When we included the specific pronouns, determiners, and punctuation that were used, the accuracy increased.

### Pronouns and Determiners
Researchers [have found](https://www.nature.com/articles/news030714-13) that women tend to use more pronouns in writing to talk about relationships. Women also use pronouns to establish a relationship with the reader. Men, on the other hand, write more about objects, leading to a higher use in determiners. The pronouns and determiners used in writing could thus distinguish between male and female authors.

### Punctuation Marks
[This analysis](https://www.textbroker.co.uk/the-gender-gap-do-men-and-women-write-differently) of men and women writers states that because men tend to write about objects and facts, they write more concise sentences. Similarly, since women tend to establish relationships with the readers, they tend to write longer sentences. This would lead to a different in their uses of punctuation marks.

### Words per Sentence
Since men tend to write more concisely than women, their sentences will be shorter and have fewer words. Therefore, the average number of words per sentence could distinguish between male and female writers.

## Preprocessing
For women's books, we filtered out the words "Finis" and "The end" at the end and the publishing date at the beginning because they don't add anything of value. For the men's books, we removed foot notes at the end and underscores in the middle of the texts. We then split each book into documents of ten sentences each. 

We found that making everything lowercase or lemmatizing the text didn't have any effect on the accuracy, which means that the location the words were used didn't have an impact.

We chose to not remove stopwords because many stopwords are pronouns or determiners, which are our features.
