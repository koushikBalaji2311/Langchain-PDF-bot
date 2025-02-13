# Chat with Your PDFs using LangChain and Streamlit

This project allows you to chat with your PDF documents using LangChain, FAISS for vector storage, and a Hugging Face model for LLM-based responses. The application is built using Streamlit for a simple and interactive UI.

## Features
- Upload multiple PDF documents.
- Extract text from PDFs using PyPDF2.
- Chunk and process text using LangChain's CharacterTextSplitter.
- Generate vector embeddings using HuggingFaceInstructEmbeddings.
- Store and retrieve document chunks with FAISS.
- Use a conversational AI model (Mixtral-8x7B-Instruct) from Hugging Face.
- Maintain chat history using LangChain's ConversationBufferMemory.

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/koushikBalaji2311/langchain-pdf-chat.git
cd langchain-pdf-chat
```

### 2. Create a Virtual Environment and Install Dependencies
```bash
python -m venv venv
source venv/bin/activate   # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Set Up Environment Variables
Create a `.env` file in the project directory and add your Hugging Face API key:
```plaintext
HUGGINGFACEHUB_API_TOKEN=your_huggingface_api_key
```

### 4. Run the Application
```bash
streamlit run chatbotapp.py
```

## Usage
1. Upload one or more PDFs using the sidebar.
2. Click "Process" to extract text, generate embeddings, and create a conversational model.
3. Ask questions about the documents in the input field.
4. Get responses based on the document contents.

## Technologies Used
- **Python**: Programming language
- **Streamlit**: Web app framework
- **LangChain**: Conversational AI framework
- **FAISS**: Vector search engine
- **Hugging Face Models**: Mixtral-8x7B-Instruct
- **PyPDF2**: PDF text extraction

## File Structure
```
📂 langchain-pdf-chat
├── 📜 chatbotapp.py                 # Main Streamlit app
├── 📜 requirements.txt       # Dependencies
├── 📜 README.md              # Documentation
```

## License
This project is licensed under the MIT License.

## Contributing
Feel free to fork and improve this project. Pull requests are welcome!

## Author
[Koushik Balaji P]

