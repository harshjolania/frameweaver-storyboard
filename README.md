# FrameWeaver: AI-Powered Storyboard Generator


## 📖 Overview
FrameWeaver is a Flask-based web application that transforms a text script into a visual storyboard. It leverages:
- **GPT-4o** for narrative enhancement and scene breakdowns  
- **image-gen-1** for comic-style scene illustrations  
- **TTS** (Text-to-Speech) for optional audio narration  

Users can log in, draft or upload an outline, and receive a sequenced collection of AI-generated panels with text, images, and audio.
- note the models can change in future for better and optimal performance 

---

## 🚀 Features
- **Scene decomposition:** Auto-splits a story into scenes with headings and dialogue.  
- **Consistent character visuals:** Uses shared reference images to maintain character appearance.  
- **Export options:** Download final storyboards as PDF or PowerPoint.  
- **User profiles & history:** Save and revisit past projects.  
- **Audio narration:** Play or download TTS for each scene.

---

## 🛠️ Tech Stack
- **Back-end:** Python, Flask, Gunicorn + WSGI  
- **Front-end:** Jinja2 templates, vanilla JS, CSS  
- **Storage:** MySQL (PythonAnywhere)  
- **AI APIs:** OpenAI GPT-4o, image-gen-1, TTS  
- **Hosting:** PythonAnywhere

---

## ⚙️ Prerequisites
1. Python 3.11+ installed locally  
2. A free PythonAnywhere account (with MySQL add-on)  
3. OpenAI API key with access to GPT-4o , image-gen modes  ,TTS
*note the Prerequisites can change in future for better and optimal performance

---

## 📝 Installation & Setup
```bash
# 1. Clone the repository
git clone https://github.com/FinalYear-Team14/frameweaver-storyboard.git
cd frameweaver-storyboard

# 2. Create & activate a virtual environment
python3 -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Configure environment variables
cp .env.example .env
# Edit .env to add:
#   OPENAI_API_KEY=<your_key>
#   FLASK_ENV=development
#   DATABASE_URL=mysql://<user>:<pass>@<host>/<db>

# 5. Initialize the database
flask db upgrade

# 6. Run the app locally
flask run
```
# Visit http://127.0.0.1:5000 in your browser (local host)

## 📂 Project Structure
```bash 
├── app.py                  # Flask entrypoint
├── storyboard_generator.py # Core logic & API integrations
├── templates/              # Jinja2 HTML templates
├── static/                 # CSS, JS, images
├── uploads/                # User upload directory
├── storyboard_assets/      # Generated assets storage
├── migrations/             # Flask-Migrate scripts
├── requirements.txt        # Python dependencies
└── report/                 # Final PDF & source files
```
---

## 📤 Usage
1. **Sign up** or **log in** with your email.  
2. **Create a new project**, enter or paste your story outline.  
3. **Generate storyboard** and preview the panels.  
4. **Download** as PDF/PPT or **play** the audio narration.

---

---

## 🤝 How to Contribute

We’d love your help improving FrameWeaver! Here’s the easiest way to get started:

1. **Open an issue** — let us know about bugs or feature ideas.  
2. **Fork & clone** the repo to your own account:  
   ```bash
   git clone https://github.com/FinalYear-Team14/frameweaver-storyboard.git

---

## 📄 License
This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

## 📬 Contact
Questions, feedback, or just want to say hi? Reach us at  :)        `harshkjolania@gmail.com`, `dishakn2003@gmail.com`,`diyasujilofficial@gmail.com `,`harishsasikumar363@gmail.com`.
