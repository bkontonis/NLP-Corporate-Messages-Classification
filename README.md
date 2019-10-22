# Corporate Messaging Case Study

In this Notebook we will create a text message classification process. This corporate message data is from one of the free datasets provided on the [Figure Eight Platform](https://www.figure-eight.com/data-for-everyone/), licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

I use NLP to process text data and then apply a classifier that predicts under which of the three categories each message falls under.

For the NLP part I use a custom transformer, which is in the `custom_transformer.py` file that I import a few lines below.

The whole process is incorporated in a pipeline, which makes very clear the order in which each step is applied and also easier to optimize any step from the data processing to modeling.

For the above-mentioned optimization I use `GridSearchCV` and grid search some parameters in the data transformation steps as well as those for the classifier. After the grid search step we have the optimal parameters for all the steps applied in the pipeline.



## Dependencies
* Python 3.5+ (I used Python 3.7.4)
* Machine Learning Libraries: NumPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK, word_tokenize, WordNetLemmatizer



## Authors

Vasilis Kontonis
 - [LinkedIn](https://www.linkedin.com/in/vasilis-kontonis-baa281b4/)
 - [GitHub](https://github.com/bkontonis)


## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Acknowledgements
* This project is part of [Udacity Data Science Nanodegree Program](https://www.udacity.com/course/data-scientist-nanodegree--nd025).
* [Figure Eight](https://www.figure-eight.com/) for providing corporate messages dataset to train my model

