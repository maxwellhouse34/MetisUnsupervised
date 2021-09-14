## Toxic Comment MVP

### Task:
- Identify toxic comments among a 150,000 wikipedia comments
- Subgroup the comments into at least one category of toxicity

### EDA:
- 90% Safe (Non-Toxic) Comments
- Most comments under 250 words
- Unsafe comments appear to be typically shorter
- Comments are cut off at 5000 characters
- Identity_hate, severe_toxic and threat are very rare
- insults and obscenities are highly correlated

### Steps Completed:
- Preproccessing using nltk, regex and spacy
- Removing numbers (often ip addresses or dates)
- Removing punctuation
- Remove formatting errors (spacing, new line chars, etc.)
- Remove websites and large blocks of characters
- Apply CountVectorizor and TfidfVectorizor to identify document similarity
- Use Lemmatization and Stemming to better process large corpus
- Identify key terms using spacy
- Complete initial supervised learning estimates using Logistic Regression and Naive Bayes
- Complete initial decompostion using NMF

### Findings:
<img width="1108" alt="Screen Shot 2021-09-14 at 5 46 16 PM" src="https://user-images.githubusercontent.com/67508938/133338287-da1d107c-251f-462d-a06f-7b14f9d08f15.png">
As seen above, the most common terms for safe and toxic comments are clearly distinct.
This shows great promise in Logisitic Regression, which has 0.96 r^2.

### Next Steps:
- Apply NMF, SVD, PCA, and KMeans to more accuratly identify patterns and subgroupings
- Utilize spacy's full capabilities for deeper analysis



