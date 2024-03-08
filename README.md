# Commonsense Knowledge in Dialogue Summarization

## Overview

This project investigates the integration of commonsense knowledge into the task of abstractive dialogue summarization. Leveraging the "Mind the gap!" framework, it delves into how commonsense, inferred through the COMET system, can significantly enhance the quality of summaries generated from dialogues. The study introduces and evaluates the SICK model and its advanced iteration, SICK++, designed to optimize the summarization process by effectively incorporating commonsense knowledge.

## Objective

The main goal is to ascertain the impact of adding commonsense knowledge to the dialogue summarization process. The research explores different models (e.g., T5-small, T5-base, BART-base, and PEGASUS-large) and datasets (DialogSum, SamSum, and TweetSumm), focusing on understanding how commonsense information can improve summary relevance and accuracy, especially in customer service contexts represented by Twitter conversations.

## Methodology

The study follows a two-fold experimental approach: 
1. Evaluating various models on DialogSum and SamSum datasets, with and without commonsense augmentation, to assess the effectiveness of commonsense knowledge in standard dialogue summarization tasks.
2. Extending the investigation to the TweetSumm dataset, which comprises Twitter customer service dialogues, employing the SICK and SICK++ models to evaluate commonsense's utility in real-world scenarios.

## Results

The results indicate that while commonsense knowledge integration does not uniformly enhance performance across all models, the SICK++ model exhibits significant improvements in summarization quality on the TweetSumm dataset. This underscores the potential benefits of structured commonsense integration, especially in specific contexts such as customer service dialogues on social media platforms.

## How to Run the Code

### Extension 1

To run the code, simply open the `Extension1_notebook.ipynb` file on Google Colab. Once opened, ensure that you select the GPU as your hardware accelerator. You can then execute all the cells in sequence.

The last cell contains scripts to train all the tested models. To choose a specific script to run, you can simply comment out the others and uncomment the one you're interested in using.

### Extension 2

For the second extension, there are two notebooks available:

1. **TweetSumm Dataset Creation**: `Tweetsumm_preprocessing.ipynb`
2. **Training with SICK**: `SICK_on_Tweetsumm.ipynb`

To use these notebooks, simply upload them to Google Colab, select the GPU as your hardware accelerator, and execute all the cells in each notebook.

The outcomes from the first notebook (`Tweetsumm_preprocessing.ipynb`) are already available in the Git repository, eliminating the need to recreate the dataset.

