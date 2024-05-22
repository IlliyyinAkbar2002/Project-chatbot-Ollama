# Ollama Chatbot Application

This is a chatbot application built with Streamlit and Ollama. The application allows users to interact with a chatbot powered by different models provided by Ollama.

The main file in this project is:

- [app.py](app.py): This is the main application file. It uses Streamlit to create a web interface for the chatbot. Users can select a model from a dropdown, and then interact with the chatbot in a chat interface. The chat history is stored in the Streamlit session state.

## How it works

The `ollama_generator` function is a generator that yields responses from the Ollama chatbot. It takes a model name and a list of messages as input, and yields the chatbot's responses one by one.

The Streamlit interface consists of a title, a dropdown for selecting the model, and a chat interface. The chat interface displays the chat history and allows the user to input new messages. When a new message is input, it is added to the chat history and the chatbot's response is generated and displayed.

## Dependencies

This project requires the following Python libraries:

- Streamlit
- Ollama

You can install these with pip:

```bash
pip install streamlit ollama

```bash
streamlit run app.py