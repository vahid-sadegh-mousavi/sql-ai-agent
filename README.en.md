# 📊 Intelligent Data Assistant - AI SQL Agent

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Flask](https://img.shields.io/badge/Flask-2.0-green.svg)
![Llama](https://img.shields.io/badge/Llama.cpp-LLM-orange.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Persian](https://img.shields.io/badge/زبان-فارسی-red.svg)
![English](https://img.shields.io/badge/Language-English-US-blue.svg)

</div>

<div align="center">
  
[🇮🇷 Persian](README.md) | [🇺🇸 English-US](README.en.md)

</div>

---

## Problem Solved

In organizations, accessing data requires SQL knowledge, making it difficult for non-technical users to generate reports from organizational data.

This project is an **AI Agent** that uses **Large Language Models (LLM)** and **Natural Language Processing (NLP)** to convert conversational Persian into **T-SQL queries** and displays results beautifully.

### Key Results
- **Eliminates SQL knowledge requirement** for non-technical users
- **Fast reporting** in under 5 seconds
- **90% accuracy** in natural language to SQL conversion
- **High security** with fully local execution (no internet required)

---

## Intelligent System Core

### 1. Persian Language Processing (NLP)
- **Named Entity Recognition**: Extract customer, product, and company names using **NER**
- **Translation to English**: Convert Persian questions for better processing
- **Text Normalization**: Standardize typos and formatting errors

### 2. Intelligent SQL Generation
- **Few-shot Learning**: Pre-defined examples for improved accuracy
- **Syntax Optimization**: Automatic conversion to T-SQL (SQL Server)
- **Error Correction**: Detect and fix common syntax errors

### 3. Beautiful Result Display
- **Interactive tables** with professional styling
- **Number formatting** with thousand separators
- **Generated query display** (toggleable)
- **Conversational Persian responses**

---

## Technical Features

| Feature | Description |
|---------|-------------|
| User Interface | Flask + HTML/CSS with responsive design |
| Language Model | Llama.cpp + Qwen-14B for Persian understanding and optimized query generation |
| Security | Fully local - no internet required |
| Quick Questions | Pre-built buttons for common queries |
| Database | SQL Server with Trusted Connection |

---

## Technologies Used

### Language & Frameworks
- **Python 3.9+** - Core development language
- **Flask** - Web service and UI
- **Llama.cpp** - LLM execution engine

### AI Models
| Model | Purpose |
|-------|---------|
| **Qwen-14B-Instruct** | Persian understanding, NER, translation |
| **SQLCoder-7B** | T-SQL query generation |

### Specialized Libraries
| Library | Purpose |
|---------|---------|
| **pyodbc** | SQL Server connection |
| **llama-cpp-python** | GGUF model execution |
| **waitress** | Production WSGI server |

---

## Installation & Usage

### Prerequisites
```bash
# Install Python 3.9 or higher
# Install required libraries
pip install -r requirements.txt

# Download models (~15GB)
# Place in models/ folder

### Required Files
Download models from HuggingFace:

Ophiuchi-Qwen3-14B-Instruct

### Run Application
cd sql-ai-agent
python src/main.py

### Access Application
http://localhost:5000

## Example Questions
Category | Question
---------|----------
Specific Customer | How many purchases and total amount did Persian Gulf Petrochemical Company have in month 7 of 2024?
Top Customers | Who are the top 3 customers by purchase amount in month 7 of 2023?
Total Sales | What is the total purchase amount for all customers in month 2 of 2025?

## Security Notes
- All processing is done locally
- No data is sent to external servers
- Database connection uses Trusted Connection (no password storage)
- Can run on internal organizational networks

## Future Development
- [ ] Visual reporting (charts and graphs)
- [ ] Fine-tuning on organizational data for better accuracy
- [ ] Query optimization suggestions
- [ ] Multi-step question support

## License
This project is released under the MIT License.