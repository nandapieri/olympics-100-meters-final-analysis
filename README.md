# Paris 2024 Men's 100m Final: YouTube Comment Analysis

An academic project for Module 6, **Telling the Game: NLP for Sports Intelligence**, of an MSc in AI Applied to Sports.

The project explores recurring expressions and sentiment in comments on one official Olympic Games YouTube video of the Paris 2024 men's 100m final. From 1,000 collected top-level comments, 618 English-language comments were selected for analysis.

Two NLP techniques are used:

- **N-gram Frequency Analysis:** bigram and trigram counts using CountVectorizer.
- **Sentiment Analysis:** NLTK VADER, compared descriptively with a Naive Bayes classifier trained on the human-labelled UCI Sentiment Labelled Sentences dataset.

The findings describe this selected sample and do not represent all viewers or public reactions.

## Project files

- `olympics_100m_nlp.ipynb`: methodology, code, results, discussion, and conclusions.
- `olympics_100m_nlp_executed.ipynb`: a copy with saved tables, charts, and examples for review without running the code.
- `comments.csv`: the frozen dataset of 1,000 collected comments.
- `.env.example`: a template for optional YouTube API configuration.

## Viewing and reproducing the analysis

Open the executed notebook to review the results. To reproduce the analysis in VS Code or Jupyter, keep `comments.csv` beside the notebook and run from **Dataset Quality Assessment** onward. The notebook's **Reproducibility and Environment** section lists dependencies and verified versions.

Internet access is needed for the UCI training dataset and, if missing, the NLTK VADER lexicon. YouTube API access is optional and disabled by default; reproducing the frozen analysis does not require an API key. Keep any local `.env` file private.
