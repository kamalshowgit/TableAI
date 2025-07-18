# TableAI: Secure Local Data Analyst

TableAI is a modern, production-ready Streamlit app that lets you analyze sensitive tabular data using a local AI-powered chatbot. All code and data stay on your machine—no cloud, no data leaks. Powered by Ollama (Mistral) and LlamaIndex, TableAI generates and runs Python (pandas) or SQL code to answer your questions, visualize data, and accelerate your analysis workflow.

---

## Features

- **Local-Only AI Chatbot:** No data leaves your machine. All code runs locally using Ollama (Mistral) and LlamaIndex.
- **Multi-Turn Chat:** Ask follow-up questions and refine code with context-aware AI.
- **Dynamic Output:** See highlighted values, tables, and graphs—automatically rendered.
- **Modern UI:** Clean two-column layout, dark theme, custom font, and smooth animations.
- **Robust Error Handling:** Friendly messages and guidance for all edge cases.
- **Code Editing & Running:** Review, edit, and re-run AI-generated code.
- **Supports Files & Databases:** Upload CSV, Excel, TSV, Parquet, JSON, or connect to SQL databases (SQLite, PostgreSQL, MySQL, MariaDB, SQL Server, Oracle, DuckDB).

---

## How It Works

1. **Landing Page:**
   - Upload a tabular file or connect to a database.
   - TableAI supports CSV, XLSX, XLS, TSV, Parquet, JSON, and major SQL databases.

2. **Preview Data:**
   - Instantly preview your data and its columns.
   - Click "Meet an analyst" to start chatting with the AI.

3. **Chatbot Analyst:**
   - Ask questions about your data in plain English.
   - The AI generates code, runs it, and shows the result (with code and output).
   - Edit and re-run code as needed.

---

## Screenshots

1. **Landing Page:**
   
   ![Landing Page](screenshots/Screenshot 2025-07-16 at 2.21.48 AM.png)

2. **Data Preview:**
   
   ![Data Preview](screenshots/Screenshot 2025-07-16 at 2.23.07 AM.png)

3. **Chatbot Analyst:**
   
   ![Chatbot View](screenshots/TableAI - Secure Data Analyst.png)

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/kamalshowgit/TableAI.git
cd TableAI
```

### 2. Create a Virtual Environment (Recommended)

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Requirements

```bash
pip install -r requirements.txt
```

### 4. Install Ollama & Mistral Model

- **Ollama:** [Install instructions](https://ollama.com/download)
- **Start Ollama:**
  ```bash
  ollama serve
  ```
- **Pull Mistral Model:**
  ```bash
  ollama pull mistral
  ```

### 5. Run the App

```bash
streamlit run app.py
```

The app will open in your browser at [http://localhost:8501](http://localhost:8501).

---

## Usage

- **Upload Data:** Use the landing page to upload a file or connect to a database.
- **Preview:** Review your data and columns.
- **Chat:** Click "Meet an analyst" and ask questions. The AI will generate code and show results.
- **Edit/Run Code:** Review, edit, and re-run code as needed.
- **Security:** All processing is local. No data or code is sent to the cloud.

---

## Troubleshooting

- **Ollama Not Running:** Make sure `ollama serve` is running in a terminal.
- **Model Not Found:** Run `ollama pull mistral` to download the model.
- **File Errors:** Ensure your file is a supported format and columns are clean.
- **Database Errors:** Double-check your connection string and table selection.
- **Other Issues:** See error messages in the app for guidance.

---

## Contributing

Pull requests and issues are welcome! Please open an issue for bugs or feature requests.

---

## License

MIT License. See [LICENSE](LICENSE) for details.

---

## Credits

- [Streamlit](https://streamlit.io/)
- [LlamaIndex](https://www.llamaindex.ai/)
- [Ollama](https://ollama.com/)
- [Mistral Model](https://ollama.com/library/mistral)

---

## Contact

For questions or support, open an issue or contact [Kamal Soni](https://github.com/kamalshowgit).
