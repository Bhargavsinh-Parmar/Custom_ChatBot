# Custom_ChatBot

# Chatbot with TensorFlow and NLTK

This project is a simple chatbot implemented in Python using TensorFlow and Natural Language Toolkit (NLTK). It is designed to interact with users through predefined intents and patterns stored in a JSON file.

## Features

- **Natural Language Processing (NLP)**: The chatbot uses tokenization, lemmatization, and a bag-of-words approach for text preprocessing.
- **Pretrained Model**: TensorFlow is used to load a pre-trained model (`chatbot_model.h5`) to predict user intents.
- **Interactive Console Chatbot**: A terminal-based chatbot for environments without GUI support.
- **Customizable Intents**: Easily modify the `intents.json` file to extend the chatbot's functionality.

## Prerequisites

Ensure you have the following installed:

- Python 3.8 or higher
- TensorFlow
- NLTK

### Install Required Libraries

```bash
pip install tensorflow nltk
```

## File Structure

- `chatbot_model.h5`: Pretrained model for intent classification.
- `intents.json`: File defining the intents, patterns, and responses.
- `words.pkl` and `classes.pkl`: Pickle files for vocabulary and intent classes.
- `CHATBOT.ipynb`: Notebook containing the chatbot's logic and training steps.
- `README.md`: Documentation for the project.

## Getting Started

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/chatbot.git
   cd chatbot
   ```

2. **Prepare the Environment**:
   Make sure all the required Python libraries are installed.

3. **Run the Chatbot**:
   If you want to interact with the chatbot via the console, use the updated Python script.
   ```bash
   python chatbot_console.py
   ```

4. **Train the Model (Optional)**:
   If you've updated `intents.json`, you need to retrain the model using the training script.

## Customization

1. **Update Intents**:
   Modify the `intents.json` file to add new intents, patterns, or responses.

2. **Retrain the Model**:
   After updating the intents, run the training script (if applicable) to update the model.

3. **Console Chatbot**:
   The console chatbot provides a headless interface for environments without a GUI.

## Example Interaction

```text
You: Hi
Chatbot: Hello! How can I help you?

You: Thank you
Chatbot: You're welcome!

You: exit
Chatbot: Goodbye!
```

## Known Issues

- **TclError: No Display Name**: This issue arises when running a GUI-based application on a headless server. Use the console-based chatbot to avoid this.
- **Model Accuracy**: Ensure the model is retrained if new intents or patterns are added.

## Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

### Contact

For any issues or suggestions, feel free to open an issue on GitHub or contact the repository owner.
