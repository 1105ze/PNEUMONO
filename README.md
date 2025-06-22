# PNEUMONO

**📰 Truthify — Fake News Detection Platform (Malaysia Hackathon)**

This project is developed as part of a hackathon challenge to tackle misinformation and disinformation in Malaysia’s online spaces.It combines machine learning, web scraping, and natural language processing (NLP) to verify online news content and assess its authenticity.

🚀 **Features**

👉 Submit URL to check news articles👉 Fake news detection using a fine-tuned BERT model👉 Extract article metadata (title, author, date, content)👉 Show Real or Fake result with article preview👉 Auto log all scanned articles into database👉 Search previously scanned articles👉 Display latest verified news on homepage👉 Related content preview (coming soon)

**🛠 Tech Stack**

FrontendHTML + CSS (via Jinja2 templates in Flask)

BackendPython 3.11 + Flask

Machine LearningBERT model fine-tuned for binary classification (Fake vs Real)

Librariestransformers, datasets, newspaper3k, beautifulsoup4, readability-lxmlsqlite3, pandas, requests, torch (PyTorch)

**📂 Folder Structure**

Hackathon/
├── app.py               # Flask web app
├── my_fake_news_bert/   # Fine-tuned BERT model (you need to provide)
├── static/              # Static files (CSS, images)
├── templates/           # HTML templates
├── news_scraped_output.csv # (optional) Scraped news content
├── thestar_news.csv     # (optional) Input URLs to scrape
├── README.md            # You are here!
└── requirements.txt     # Python dependencies

⚙ Installation & Run

⿡ Clone the project

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

⿢ Create and activate virtual environment

python3 -m venv venv
source venv/bin/activate

⿣ Install dependencies

pip install -r requirements.txt

⿤ Run the app

python app.py

Then open in browser:

http://127.0.0.1:5000/

If you want to test on mobile phone (same Wi-Fi):

# in app.py
app.run(debug=True, host='0.0.0.0')

Then access from mobile:

http://YOUR_LOCAL_IP:5000/

📌 Notes

The BERT model folder should be placed in:

./my_fake_news_bert

The news.db database will auto-create after running the app and detecting news.

Current project tested with:macOS + Python 3.11 + Flask 3.x

Contributions and pull requests are welcome!If you like this project, please ⭐ the repo!
