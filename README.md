# AMLproject
# Project Structure:
The project consists of three parts:
1. classifier to tell real news from fake news
2. Generators, which take an input and generate a news article (two generators, trained on the fake & real news respectively)
3. Explanation & reasoning, what triggers the classifier 

# Roadmap:
- Initialize & clean data (14-15.5.2025)
      Remove date for all entries

  4 datasets in total to use:
      1. Real news dataset (split from original data)
      2. Fake news dataset (split from origninal data)
      3. Real model dataset (remove anything but title, category & text, maybe keep source)
      4. Fake model dataset (remove anything but title, category & text, maybe keep source)
    replace NaNs by unknown
    split data into fake & real news

- Create classifier & train it from IMDB example (14-15.5.2025)
    try to tune the example code to get a classifier with good accuracy

- Create generative models (21.5.2025)
    see how it was done before, take nanoGPT as reference


Model analysis: 
- 

- Work out how to reason about the values 

- 
- Presentation slides (TBD)

TODO:
- Alok
      - Dataset analysis
              Compare Vocabulary: Are the word distributions, frequencies, or jargon usage different?
            Style and Tone: Is one dataset more formal, narrative, concise, etc.
            Structure of Input/Output: Are sentence lengths, syntax complexity, or input formats different?
            Metadata: Are there hidden signals like timestamps, source authorship, or categories?
        - Slides start

- Chen
        Latent Space Visualization
        t-SNE, UMAP on internal embeddings
      Attention heatmaps if models are transformer-based
      Compare context windows or attention weights
  

- Tangzhi
- Model Architecture examination
  Actions:
      Check:
      Learning rates
      Loss functions
      Batch sizes
      Training epochs
      Tokenization method
      Make sure the same tokenizer was used unless intentionally different.


- Hadi
      Measure Bias or Drift
  Even subtle shifts in the training set can change model behavior drastically.
      Actions:
      Check for:
      Topic emphasis drift (e.g., one dataset discusses subtopic A more than B)
      Biases introduced by dataset-specific phrasing
      Repetition or memorization differences

- Carlos
      Hyperparameter optimization on classifier & analysis of it
