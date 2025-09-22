
# AI-Powered Resume Analyzer

An intelligent Resume Analyzer that extracts, parses, and analyzes resumes to provide structured insights.
Built with Streamlit frontend, Python backend, and powered by Google Generative AI (Gemini) for smart analysis.

🚀 Features

📂 Upload Resumes (PDF format)

🔍 Extract Text using pdfplumber

🖼️ OCR Fallback with pytesseract for scanned PDFs

🤖 AI Analysis with Google Generative AI (Gemini)

⚡ Streamlit UI for interactive and easy-to-use interface

🔐 Secure API Keys via .env (never hardcoded)

🛠️ Tech Stack
Component	Technology
Frontend	Streamlit
Backend	Python
AI Model	Google Generative AI (Gemini)
PDF Parsing	pdfplumber
OCR Fallback	pytesseract
Config & Secrets	.env file for API key management

⚙️ Installation

Clone the repository

git clone https://github.com/your-username/resume-analyzer.git
cd resume-analyzer


Create virtual environment & activate it

python -m venv env
.\env\Scripts\activate   # On Windows
source env/bin/activate  # On Mac/Linux


Install dependencies

pip install -r requirements.txt


Set up environment variables

Create a .env file in the project root.

Add your Google API key:

GOOGLE_API_KEY=your_api_key_here

▶️ Usage

Run the Streamlit app:

streamlit run app.py


Upload a PDF resume.

If text extraction via pdfplumber fails, the system falls back to pytesseract OCR.

The extracted text is sent to Google Generative AI (Gemini) for analysis.

Results are displayed in a clean, interactive UI.

🔐 Security

.env is ignored in Git (.gitignore) so your API keys remain private.

If deploying on Streamlit Cloud, use the Secrets Manager instead of .env.

📌 Example Output

Resume summary

Skills extraction

Experience breakdown

AI-generated suggestions for improvement

📄 Requirements

Python 3.8+

Poppler (for pdf2image)

Tesseract OCR (for pytesseract)

🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request.
