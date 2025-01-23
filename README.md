# Predictify

## download trained model from here
https://drive.google.com/file/d/1IhwwK9wh0QgSCbAUhD7ChP0Lx3CDl0bq/view?usp=sharing


# Text Generation Model using LSTM

This repository contains a text generation model built with TensorFlow and Keras. The model is trained on the Kaggle Movie Subtitles dataset to predict the next word in a sequence, allowing it to generate coherent text. The architecture is based on a single LSTM layer combined with an embedding layer for efficient word representation and contextual understanding.

## Features

### LSTM-Based Model: Uses a single LSTM (Long Short-Term Memory) layer with 512 units, well-suited for sequence-based tasks like text generation.

### Embedding Layer: Learns dense vector representations of words (300-dimensional vectors) during training, capturing semantic relationships between words.

### Tokenization: Implements word-level tokenization for efficient processing of input text.

### Scalable Training: Designed to handle incremental training on large datasets while considering memory constraints (e.g., free Google Colab's 12GB memory limit).

## Dataset

### Source: Kaggle Movie Subtitles dataset

### Description: A large collection of movie subtitles providing diverse and context-rich text sequences.

### Preprocessing: The text data is tokenized, cleaned, and converted into sequences of input words and their corresponding target words.

## Model Architecture

### Embedding Layer: Converts input tokens into dense vectors of a fixed size (300 dimensions), which are learned during training.

### LSTM Layer: Processes sequences of embeddings, maintaining context across the input sequence with 512 units.

### Dense Layer: Converts the LSTM's output into a probability distribution over the vocabulary.

## Training Process

### Data Preparation:

The input text is tokenized into sequences.

Each sequence is padded to ensure uniform length.

The target word for each sequence is converted to one-hot encoding.

### Training:

The model is trained using categorical cross-entropy loss and the Adam optimizer.

Fine-tuning is supported, but care must be taken to avoid forgetting previously learned patterns.

### Evaluation:

The model’s accuracy is measured on the training data (achieving ~80% accuracy).

Generated text samples are used to qualitatively assess performance.

# Sample Outputs
_(input before hyphen - output afte hyphen)_


I am a - I am a humble man who is here to learn from my friends in the new world

you dont - you dont know what its like to carry a child and give birth

he - he made small talk

his - his body was discovered in an abandoned theater

her - her room was empty and the bed was still neatly made for her

I am sorry - I am sorry but we have to ask you to be out by the end of the week

I apologize - I apologize for interrupting like this

do - do you know what time it is

you know that - you know that its a bad thing for me

fine - fine ill do it my dear man

how to - how to find out this thing you dont know

## Future Improvements

### Data Augmentation: Incorporate diverse datasets to improve generalization.

### Stacked LSTMs: Experiment with deeper architectures to capture more complex patterns.

### Fine-Tuning Optimization: Improve techniques for incremental training without performance degradation.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

Kaggle for the Movie Subtitles dataset.

TensorFlow and Keras for their powerful deep learning frameworks.

The amazing online community for resources and support.
