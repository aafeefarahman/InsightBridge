# InsightBridge
https://colab.research.google.com/drive/132SapaQ9Zjq3QIISdCibdkJ4QSglJOnU?usp=sharing
An AI-powered agent for inclusive communication – translates, classifies, and interprets real-time input to assist users with diverse accessibility needs. it is  lightweight, intelligent agent designed to enhance the clarity, structure, and purpose of any text-based content. It auto-detects the content type (e.g., Blog, Survey, News, About, etc.), then either "summarizes"" it or "checks for grammar and structure issues" — making communication more inclusive and accessible for all.

**Project Overview**
-InsightBridge is an AI-powered text interpretation tool designed to make written communication more accessible, inclusive, and actionable. 
-Built with simplicity and real-world use cases in mind, the app automatically identifies the type of content a user provides such as blogs, surveys, news articles, or descriptions—and applies intelligent processing based on its classification.
-Whether you're a content creator, researcher, startup founder, or community worker, InsightBridge helps you:
->Understand better by summarizing long or technical text,
->Communicate better by identifying and correcting grammar issues,
->Save time by automatically detecting content types and applying smart interpretation logic.
-Currently deployable via Google Colab or Streamlit, InsightBridge keeps everything lightweight, modular, and ready for rapid experimentation and feedback.

**How it Works:**
* The tool analyzes text, detects its type using rule-based logic, and applies either summarization (via Sumy) or grammar checking (via LanguageTool).
* **Use Cases:** Startups optimizing website content, journalists reviewing news summaries, educators interpreting student writing, and researchers digesting long surveys.
  
##  Technologies Used
- Python 
- Google Colab
- Streamlit
- OpenAI (for classification/response generation) 
- SpeechRecognition 
- LangDetect

---
##  Features
🔎 Content Type Detection
Automatically identifies the input content as a Blog, Survey, News, About, etc.
Uses rule-based keyword detection (can be enhanced with ML in future).
🧠 Intelligent Summarization
Summarizes long texts using the Sumy library.
Helps reduce reading time and extract key points from input data.
📝 Basic Grammar Error Detection (Environment Dependent)
Highlights grammatical issues using language-tool-python.
Works best in local environments with Java 17+.
📊 Minimal UI for Inputs
Simple input area for pasting text.
Streamlit or Google Colab interface for user interaction (flexible deployment).
📁 Lightweight & Flexible Deployment
No heavy GPU or server dependency – works in both Google Colab and VS Code.
Easy to clone, modify, and redeploy.

## Problem Statement
Many users, especially in multilingual communities, struggle to format, summarize, or grammatically refine their ideas. InsightBridge bridges this gap by using rule-based logic and AI tools for **content classification**, **summarization**, and **language correction**, helping users refine their communication with minimal effort.
 
---
## Installation
✅ Option 1: Google Colab (Recommended for fast access)
1. Open the [Colab Notebook](#)  
2. Run the following in the first cell:
python
!pip install nltk sumy
import nltk
nltk.download('punkt')
⚠️ Grammar checking requires Java 17+. Colab only supports Java 11.

✅ Option 2: Local Setup (VS Code + Streamlit)
Clone the repository:
git clone https://github.com/your-username/InsightBridge.git

**Install dependencies:**
pip install -r requirements.txt
Download NLTK tokenizer:
import nltk
nltk.download('punkt')
Run the app:
streamlit run app.py
🧩 Requirements
Python 3.10 or above
Java 17+ (only for grammar correction via language-tool-python)
Streamlit (for UI)
nltk
sumy
language-tool-python (optional)

**Use Cases**
Researchers:Summarize lengthy survey responses.
Journalists:Refine news content and check grammar.
Startups:Classify content and clean up About or Blog pages.
Educators: Quickly interpret students’ written material.

**Contributors**
Afeefa Rahman
Rimsha Nishath

**Notes**
We are constantly improving the logic behind content classification.
Translation and grammar checking modules are optional and may vary based on your environment.




