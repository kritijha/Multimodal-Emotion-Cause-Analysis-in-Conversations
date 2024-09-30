# Multimodal Emotion Cause Analysis in Conversations

This work is the final project for CSCI 535:  Multimodal Probabilistic Learning of Human Communication at the University of Southern California.


This repository contains the implementation of a computational framework for identifying and extracting emotion-cause pairs from conversations using multimodal data (text, audio, and video). The framework leverages various encoding techniques, fusion strategies, and deep learning-based classification models to analyze emotional expressions and their underlying causes in conversational settings. 

## Data Description
The framework utilizes the multimodal [Emotion-Cause-in-Friends (ECF) dataset](https://github.com/NUSTM/SemEval-2024_ECAC), derived from the popular television sitcom "Friends". This dataset is well-suited for the task of emotion recognition and emotion cause extraction in conversational videos due to its rich emotional content and diverse conversational scenarios.
![example](https://raw.githubusercontent.com/NUSTM/SemEval-2024_ECAC/main/example.png)

## Main Contributions

1. **Multimodal Emotion Detection**: The framework employs early and late fusion techniques to combine textual, acoustic, and visual cues for emotion detection. Early fusion involves concatenating encoded features from different modalities, while late fusion integrates the outputs of modality-specific classifiers.

2. **Emotion-Cause Pair Prediction**: The framework utilizes both Multilayer Perceptron (MLP) and Transformer-based models to predict emotion-cause pairs. These models incorporate multimodal embeddings and predicted emotion labels to determine valid emotion-cause relationships.

3. **Addressing Class Imbalance**: The framework employs weighted loss functions to mitigate the effects of class imbalance, ensuring robust performance across diverse emotional states.

4. **Combined Accuracy Metric**: A novel combined accuracy metric is introduced to evaluate the overall effectiveness of the emotion-cause pair prediction pipeline. This metric assesses whether the framework can accurately predict both the emotion and its corresponding cause.

## Key Results

The framework's performance was evaluated on the multimodal Emotion-Cause-in-Friends (ECF) dataset, derived from the television sitcom "Friends". The main results are summarized below:

1. **Emotion Detection**:
   - For text modality, the transformer model achieved the highest accuracy of 58.14% and an F1 score of 55.65%.
   - Early fusion with MLP performed best, with an accuracy of 54.52% and an F1 score of 53.83%.

2. **Cause Pair Prediction**:
   - MLP with late fusion performed best, with an accuracy of 88.23%.
   - Early fusion on the MLP classifier achieved the highest F1 score of 87.79%.

3. **Combined Accuracy**:
   - The text modality achieved the highest combined accuracy of 28.89%.

The results highlight the challenges and complexities inherent in multimodal emotion analysis, emphasizing the need for further exploration of model architectures and fusion techniques to improve accuracy and understanding in emotion and cause pair prediction tasks.

## Contributors
This project was created by the following people:

1. Anuranjan Pandey
2. Kriti Jha
3. Sweta Singh
