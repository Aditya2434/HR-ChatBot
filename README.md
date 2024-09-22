HR Policy Chatbot
This project is an HR Policy Chatbot that allows users to query HR policies in a conversational format. It leverages Retrieval-Augmented Generation (RAG), LangChain, FAISS vector database, and the Google Gemini API to fetch and answer questions based on HR policy documents. The app is built using Streamlit for a smooth and interactive user interface.

Features
Document-Based QA: Upload PDF or DOC files containing HR policies. The chatbot will extract the information and store it in a vector database (FAISS) for efficient semantic search.
Semantic Search: Queries are answered based on similarity matching in the FAISS vector database, ensuring relevant results.
Google Gemini API: Powered by the Google Gemini model, the chatbot uses embeddings to understand and process HR-related queries.
Real-Time Interaction: Users can have real-time, memory-enabled conversations with the chatbot regarding various HR policies.
Streamlit UI: A user-friendly web interface that supports uploading files and querying policies effortlessly.
Tech Stack
Python: Backend and logic implementation.
Streamlit: Frontend UI for file uploads and interaction.
FAISS: Vector database for semantic search and document retrieval.
Google Gemini API: Used for generating embeddings and processing natural language queries.
LangChain: Orchestrates the RAG pipeline, handling query decomposition and response generation.
How It Works
HR Policies Download: HR policy documents are downloaded from a website and stored in the local storage.
Document Parsing: The documents (PDF/DOC) are processed to extract text and create embeddings using the Google Gemini API.
Vector Database (FAISS): The extracted embeddings are stored in a FAISS vector database for efficient similarity-based search.
User Queries: Users interact with the chatbot by asking questions related to HR policies. The chatbot performs a semantic search on the FAISS database and provides the most relevant policy information.
Conversational Memory: The chatbot retains memory of the ongoing conversation, allowing for a continuous and smooth user experience.
How to Run the Project
Prerequisites
Python 3.8+
Streamlit
FAISS
LangChain
Google Gemini API key
Required Python libraries (install via requirements.txt)
Steps to Run
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/hr-policy-chatbot.git
cd hr-policy-chatbot
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Set up your Google Gemini API Key:

bash
Copy code
export GOOGLE_API_KEY="your-google-api-key"
Run the Streamlit app:

bash
Copy code
streamlit run app.py
Open your browser and navigate to http://localhost:8501 to interact with the chatbot.

Future Enhancements
Adding support for more document formats (e.g., .txt, .xlsx).
Expanding the chatbot's capabilities to handle multiple topics beyond HR policies.
Integrating user authentication for secure policy access.
Contributing
Contributions are welcome! Please feel free to open issues, suggest new features, or submit pull requests.

License
This project is licensed under the MIT License.
