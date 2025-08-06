# 🌍 Gemma 3n Multilingual Learning Assistant

An AI-powered learning assistant that helps you learn words from 16 Indian languages using Google's Gemma 3n model, translation services, and intelligent storage with FAISS vector search.

## 🚀 Features

### Core Capabilities
- **Multilingual Support**: Learn words from 16 Indian languages including Hindi, Tamil, Bengali, Kannada, Telugu, and more
- **AI-Powered Explanations**: Get comprehensive word explanations using Google's Gemma 3n model
- **Smart Translation**: Automatic translation from Indian languages to English using Hugging Face models
- **Intelligent Storage**: FAISS vector database for semantic search and word retrieval
- **Interactive Learning**: Jupyter notebook interface with widgets for easy interaction
- **Quiz Mode**: Test your knowledge with randomly generated quizzes
- **Search Functionality**: Find similar words using semantic search

### Supported Languages
- Hindi (Devanagari script)
- Tamil (Tamil script)
- Bengali (Bengali script)
- Kannada (Kannada script)
- Telugu (Telugu script)
- Gujarati (Gujarati script)
- Marathi (Devanagari script)
- Punjabi (Gurmukhi script)
- Urdu (Perso-Arabic script)
- Malayalam (Malayalam script)
- Odia (Odia script)
- Assamese (Bengali script)
- Manipuri (Bengali script)
- Kashmiri (Perso-Arabic script)
- Konkani (Devanagari script)
- Sanskrit (Devanagari script)

## 🛠️ Technology Stack

- **AI Models**: Google Gemma 3n (4B model), Hugging Face translation models
- **Vector Database**: FAISS for semantic search and storage
- **Embeddings**: Sentence Transformers (all-MiniLM-L6-v2)
- **Interface**: Jupyter Notebook with ipywidgets
- **Languages**: Python 3.8+
- **Key Libraries**: PyTorch, Transformers, Pandas, NumPy

## 📋 Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- API keys for:
  - Google AI (for Gemma 3n access)
  - Hugging Face (for translation models)

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd "Gemma 3n aug 2025"
   ```

2. **Install required packages**
   ```bash
   pip install torch transformers sentence-transformers faiss-cpu google-generativeai openai python-dotenv pandas numpy ipywidgets tqdm requests
   ```

3. **Set up environment variables**
   - Copy `config.env` and fill in your API keys:
   ```bash
   cp config.env .env
   ```
   - Edit `.env` with your actual API keys:
   ```
   HUGGINGFACE_API_TOKEN=your_actual_huggingface_token
   GOOGLE_AI_API_KEY=your_actual_google_ai_key
   ```

## 🚀 Usage

1. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Open the main notebook**
   - Open `Gemma3n_Multilingual_Learning_Assistant.ipynb`

3. **Run all cells**
   - Execute all cells in order to initialize the system

4. **Start Learning**
   - Select a language from the dropdown
   - Enter a word or phrase in the selected language
   - Click "Learn Word" to get AI-powered explanations
   - Use "Start Quiz" to test your knowledge
   - Use "Search Words" to find similar words

## 📁 Project Structure

```
Gemma 3n aug 2025/
├── Gemma3n_Multilingual_Learning_Assistant.ipynb  # Main application
├── config.env                                      # Configuration template
├── .gitignore                                      # Git ignore file
├── project.png                                     # Project screenshot
├── data/                                           # Data storage directory
│   ├── word_embeddings.faiss                      # FAISS vector index
│   └── learned_words.json                         # Word metadata
└── logs/                                           # Log files directory
```

## 🔍 How It Works

### 1. Translation Pipeline
- Input word in Indian language
- Translation to English using Hugging Face models
- Confidence scoring and error handling

### 2. AI Explanation Generation
- Google Gemma 3n generates comprehensive explanations
- Includes pronunciation, usage examples, cultural context
- Related words and synonyms

### 3. Intelligent Storage
- FAISS vector database for semantic search
- JSON metadata storage for word information
- Automatic indexing and retrieval

### 4. Learning Interface
- Interactive Jupyter widgets
- Real-time processing and feedback
- Quiz generation and search functionality

## 🎯 Key Features Explained

### Word Learning Process
1. **Input**: User enters a word in any supported Indian language
2. **Translation**: System translates to English using specialized models
3. **AI Explanation**: Gemma 3n provides comprehensive word analysis
4. **Storage**: Word is stored with embeddings for future retrieval
5. **Display**: Rich HTML output with all word information

### Quiz Mode
- Randomly selects words from your learned vocabulary
- Tests translation knowledge
- Provides immediate feedback with detailed explanations

### Search Functionality
- Semantic search using FAISS vector similarity
- Finds related words based on meaning
- Returns similarity scores and metadata

## 🔧 Configuration

The system uses a `config.env` file for configuration:

```env
# API Keys
HUGGINGFACE_API_TOKEN=your_token
GOOGLE_AI_API_KEY=your_key

# Storage Paths
FAISS_INDEX_PATH=./data/word_embeddings.faiss
METADATA_PATH=./data/learned_words.json

# Model Configuration
DEFAULT_TRANSLATION_MODEL=Helsinki-NLP/opus-mt-hi-en
```

## 📊 Utility Functions

The notebook includes several utility functions:

- `export_learned_words()`: Export all words to CSV
- `get_language_statistics()`: View learning progress by language
- `clear_all_data()`: Reset the learning database
- `test_all_features()`: Comprehensive system testing

## 🧪 Testing

Run the comprehensive test suite:
```python
test_results = test_all_features()
```

This tests:
- Translation service functionality
- Gemma explanation generation
- Storage and retrieval systems
- Search and quiz features
- Interface components
- Language support
- Configuration validation

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is open source. Please check the license file for details.

## 🙏 Acknowledgments

- Google for providing the Gemma 3n model
- Hugging Face for translation models
- The open-source community for the libraries used

## 📞 Support

For issues and questions:
1. Check the testing section in the notebook
2. Verify your API keys are correctly set
3. Ensure all dependencies are installed
4. Check the logs directory for error information

## 🔄 Updates

The system automatically:
- Saves learned words to persistent storage
- Maintains vector embeddings for semantic search
- Tracks learning progress and statistics
- Provides export functionality for data portability

---

**Happy Learning! 🌍📚** 