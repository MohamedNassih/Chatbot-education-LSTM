# Pedagogy Chatbot

## Overview

This project implements a Pedagogy Chatbot using a Long Short-Term Memory (LSTM) neural network. The chatbot is trained on a carefully curated dataset encompassing a wide array of intents and patterns pertinent to the field of pedagogy. Its purpose is to engage users in meaningful conversations by providing insightful responses to queries about diverse pedagogical theories, child development stages, effective teaching strategies, and much more.

## Project Structure

```
├── data
│   └── Intents.json          # The JSON file containing the training dataset
└── chatbot.py               # The main Python script for the chatbot
```
## Installation

1. Clone the repository:
```
git clone https://github.com/your-username/pedagogy-chatbot.git
```

2. Install the required libraries:
```
pip install -r requirements.txt
```

## Dataset

The heart of the chatbot's knowledge lies in the `Intents.json` file located within the `data` directory. This JSON file houses a structured dataset meticulously crafted to encapsulate a wide spectrum of pedagogical concepts. Each entry in the dataset comprises an "intent" representing a specific user query category, alongside corresponding "patterns" that exemplify diverse ways users might phrase their inquiries within that category. Moreover, each intent is associated with a set of "responses" from which the chatbot can intelligently select to provide relevant and informative answers.

## Model

An LSTM neural network forms the foundation of this chatbot. Renowned for their prowess in natural language processing, LSTMs excel at capturing long-term dependencies within text sequences, making them ideal for understanding the nuances of human conversation. This particular LSTM model is constructed and trained using the Keras library, a powerful and user-friendly deep learning framework.

## Training

To imbue the chatbot with pedagogical knowledge, the LSTM model undergoes rigorous training. The training process involves feeding the model with the intent and pattern data from the `Intents.json` dataset, enabling it to learn the intricate relationships between user queries and appropriate responses.  During training, the model's parameters are iteratively adjusted to minimize the discrepancy between its predicted outputs and the actual responses provided in the dataset. This process continues for a predefined number of epochs (iterations over the entire dataset) until the model achieves a satisfactory level of accuracy. The training parameters, such as the number of epochs and batch size, are carefully chosen to optimize the model's performance.

## Usage

1. **Installation:**
   ```bash
   git clone https://github.com/your-username/pedagogy-chatbot.git
   pip install -r requirements.txt
   ```

2. **Running the Chatbot:**
   ```bash
   python chatbot.py
   ```

3. **Interaction:**  Once the chatbot script is running, you will be greeted with a prompt to start a conversation. Simply type your question or statement, and the chatbot will process your input and generate a relevant response based on its training. To end the conversation, type "quit."
