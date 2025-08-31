🎙️ TTS & Voice Cloning (Notebook)

This project demonstrates Text-to-Speech (TTS) and Voice Cloning using Generative AI tools inside a Jupyter/Colab notebook.

It allows you to:
📝 Convert text into speech
🎤 Clone a reference voice and apply it to audio
⚡ Process long inputs with chunking

🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/emaanfatima28/TTS_-_VoiceCloning.git
cd TTS_-_VoiceCloning

2️⃣ Install Dependencies
If you’re running locally in Jupyter Notebook:
pip install -r requirements.txt


If you’re running in Google Colab, just add this at the top of your notebook:
!pip install -r requirements.txt

3️⃣ Get Your Deepgram API Key

Go to Deepgram Console
Create a free account
Go to API Keys → Create Key
Copy your key

4️⃣ Set API Key in Notebook
Instead of hardcoding, load it safely inside your notebook:

import os

# Option 1: Directly set in notebook (not recommended for sharing)
os.environ["DEEPGRAM_API_KEY"] = "your_api_key_here"

# Option 2: Use a .env file (recommended if running locally)
from dotenv import load_dotenv
load_dotenv()

.env file format (place in project root):
DEEPGRAM_API_KEY=your_api_key_here

5️⃣ Run the Notebook

Open the TTS_VoiceCloning.ipynb notebook in:
Google Colab (easiest, no setup needed)
Or Jupyter Notebook locally

🛠️ Tech Stack

Python (Torch, Torchaudio, Librosa, Whisper, etc.)
Deepgram API for TTS processing
OpenVoice for voice cloning