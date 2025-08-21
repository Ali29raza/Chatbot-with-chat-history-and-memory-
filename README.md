# LangGraph Chatbot

An advanced chatbot application built using **LangGraph**, **Google
Gemini 2.0 Flash**, and **Streamlit**.\
The chatbot supports persistent conversation history using an SQLite
database, allowing users to manage multiple chat threads.

------------------------------------------------------------------------

## 🚀 Features

-   **Conversational UI**: Built with Streamlit's chat interface
    (`st.chat_message`, `st.chat_input`).
-   **Thread Management**: Create new chats, switch between
    conversations, and resume past discussions.
-   **Persistent Storage**: All conversation history is stored in an
    SQLite database (`chatbot.db`).
-   **LangGraph Integration**: Uses `StateGraph` for structured chatbot
    flows.
-   **Google Gemini 2.0 Flash LLM**: Provides fast and reliable
    responses.

------------------------------------------------------------------------

## 📂 Project Structure

    .
    ├── app.py                 # Streamlit frontend application
    ├── langgraph_backend.py   # Backend with LangGraph + Gemini integration
    ├── chatbot.db             # SQLite database for storing chat history (auto-created)
    └── README.md              # Project documentation

------------------------------------------------------------------------

## ⚙️ Installation

1.  Clone the repository:

    ``` bash
    git clone https://github.com/yourusername/langgraph-chatbot.git
    cd langgraph-chatbot
    ```

2.  Create and activate a virtual environment:

    ``` bash
    python -m venv venv
    source venv/bin/activate   # On Linux/Mac
    venv\Scripts\activate    # On Windows
    ```

3.  Install dependencies:

    ``` bash
    pip install -r requirements.txt
    ```

------------------------------------------------------------------------

## 🔑 Environment Variables

Create a `.env` file in the project root and add your Google API key:

    GOOGLE_API_KEY=your_api_key_here

------------------------------------------------------------------------

## ▶️ Running the App

Run the chatbot locally with Streamlit:

``` bash
streamlit run app.py
```

Then open <http://localhost:8501> in your browser.

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   **Python 3.10+**
-   **Streamlit**
-   **LangGraph**
-   **LangChain Core**
-   **Google Generative AI (Gemini 2.0 Flash)**
-   **SQLite (for checkpointing & thread storage)**

------------------------------------------------------------------------

## 📌 Future Enhancements

-   Add **user authentication** for personalized chats.
-   Support for **multimodal inputs** (text + image).
-   Enhanced UI/UX with themes and better sidebar organization.

------------------------------------------------------------------------

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first
to discuss what you'd like to change.

------------------------------------------------------------------------

## 📄 License

This project is licensed under the MIT License.
