# LLM Explorer

LLM Explorer is a powerful tool that allows you to run and test Large Language Models (LLMs) with a chat interface for free on Google Colab. This project demonstrates the capabilities of modern AI technologies and provides an accessible platform for experimentation and learning.

## Features

- **Free GPU Access**: Utilizes Google Colab's T4 GPU resources for cost-effective LLM testing.
- **Interactive Chat Interface**: Streamlit-based UI for easy interaction with the LLM.
- **Document Processing**: Upload and analyze PDF documents to provide context for the LLM.
- **Multiple LLM Support**: Currently implements Llama 3.1, with potential for easy integration of other models.
- **Vector Store Integration**: Uses Chroma for efficient storage and retrieval of document embeddings.

## Getting Started

1. Open the `Chatbot.ipynb` notebook in Google Colab.
2. Ensure you're using a T4 GPU runtime.
3. Run the installation cells to set up the required dependencies.
4. Follow the instructions to install and run Ollama.
5. Upload a PDF document when prompted.
6. Interact with the chatbot through the Streamlit interface.

## Components

- `Chatbot.ipynb`: Main Jupyter notebook containing the setup and execution code.
- `app.py`: Streamlit application for the chat interface.
- Dependencies: langchain, llama-index, streamlit, ngrok, and others (see installation cells in the notebook).

## Usage

After setting up the environment and uploading a document:

1. The system will process the document and create a vector store.
2. A chat interface will be available through a public URL (provided by ngrok).
3. Ask questions related to the uploaded document, and the LLM will provide context-aware responses.

## Customization

- To use a different LLM, modify the `Ollama` initialization in the code.
- Adjust the embedding model by changing the `SentenceTransformerEmbeddings` parameters.
- Modify the `app.py` file to customize the Streamlit interface.

## Limitations

- Requires a Google account with access to Colab.
- Performance may vary based on Colab's available resources.
- The free ngrok plan has limitations on connection duration and bandwidth.

## Future Improvements

- Support for multiple document types (beyond PDF).
- Integration with more LLM models.
- Enhanced error handling and user feedback.
- Persistent storage options for chat history and document embeddings.

## Contributing

Contributions to LLM Explorer are welcome! Please feel free to submit pull requests, create issues, or suggest improvements.

## License

This project is open-source and available under the MIT License.

## Acknowledgments

- Thanks to the teams behind Langchain, Llama Index, and Streamlit for their excellent tools.
- Gratitude to Google Colab for providing free GPU resources for education and experimentation.
