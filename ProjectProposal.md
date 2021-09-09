# Testing for Toxic Talk
## Description
For anyone operating in a forum or social media space in today’s world, it is impossible to ignore the rapidly changing landscape of conversation. From cyberbullying to hate speech to misinformation, the identification of toxic conversation is a valuable tool for any company or user conversing online. While the need for this classification is clear, the implementation and optimization are much more complicated. This project will look to accurately classify Wikipedia comments to identify toxicity.
## Question/need:
- What is the framing question of your analysis, or the purpose of the model/system you plan to build?
  - How can we best identify toxic comments? What aspects of vocabulary, word choice, and word order, or spelling best inform this filter?
- Who benefits from exploring this question or building this model/system?
  - Anyone operating in a digital, conversational space. Whether they are participating in a board game discussion forum, a Facebook comment section, or trying to find answers to a machine learning question.
## Data Description:
- What dataset(s) do you plan to use, and how will you obtain the data?
  - https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/
  - Jigsaw, subsidiary of Alphabet (Google)
  - Over 150,000 comments
  - Median of ~30 words per comment
  - 90% “non-toxic”
- What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?
  - The comments will be individual samples.
  - The features will be the texts of the comments
- If modeling, what will you predict as your target?
  - Whether or not a comment is toxic.
  - With time, I would like to focus on accurate prediction for the 6 categories provided by the competition.
## Tools:
- How do you intend to meet the tools requirement of the project?
  - Sklearn
  - Pandas
  - Numpy
  - Nltk
  - Gensim
  - Textblob
  - spaCy
  - Tableau
- Are you planning in advance to need or use additional tools beyond those required?
  - If I have time, I would love to apply some deep learning strategies to my project.
## MVP Goal:
- What would a minimum viable product (MVP) look like for this project?
  - Initial classification of toxic vs. non-toxic comments.





