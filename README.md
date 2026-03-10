# Flash-Lite ⚡️

Flash-Lite is an AI-powered study tool that automatically generates flashcards from any text using local LLMs via Ollama. 

## 🚀 Features
- **Local AI:** Uses Llama 3 (via Ollama) to process your text privately on your machine.
- **Smart Generation:** Automatically creates 5 distinct question/answer pairs from any input.
- **Interactive UI:** Clean, modern interface with flip-card animations and study progress tracking.
- **No API Keys:** Runs entirely locally—no subscriptions or external API costs.

---

## 🛠 Setup & Installation

### 1. Install Ollama
Flash-Lite requires **Ollama** to run the AI model locally.
- **Download:** Visit [ollama.com](https://ollama.com/download) and download the version for your OS (macOS, Windows, or Linux).
- **Install:** Run the installer and ensure Ollama is running in your menu bar/system tray.

### 2. Pull the Model
Open your terminal and run the following command to download the Llama 3 model:
```bash
ollama pull llama3
```
*(You can also use `llama3:latest` as specified in the code)*

### 3. Clone and Setup the Program
To copy the entire codebase and get started:

```bash
# Clone the repository (or create the folder)
git clone https://github.com/NachikethReddyY/Flash-Lite.git
cd Flash-Lite

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# Install dependencies
pip install flask flask-sqlalchemy requests
```

---

## 📸 Screenshots & Usage

### Step 1: Input Text
Paste your study material into the main input field.
<img width="3404" height="1970" alt="image" src="https://github.com/user-attachments/assets/1f2e642c-7689-464b-968c-b20d007f6e4a" />


### Step 2: Generation
The AI will process the text and generate cards.
![Kapture 2026-03-10 at 17 43 52](https://github.com/user-attachments/assets/ede759d7-7ced-433e-b6e3-a7bcd6f08111)


### Step 3: Study
Flip the cards to test your knowledge!
![Kapture 2026-03-10 at 17 57 46](https://github.com/user-attachments/assets/fafeeeed-1d56-43c1-97ab-a7b0e9f10266)


---

## 💻 Technical Instructions (For Developers)

If you are setting up this repository for the first time:

```bash
echo "# Flash-Lite" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/NachikethReddyY/Flash-Lite.git
git push -u origin main
```

### Running the App
1. Ensure Ollama is running.
2. Run the Flask server:
   ```bash
   python main.py
   ```
3. Open your browser to `http://127.0.0.1:5001`
