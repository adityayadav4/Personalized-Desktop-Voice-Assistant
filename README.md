# Personalized-Desktop-Voice-Assistant

🎙️ Personalized Desktop Voice Assistant
A smart AI-powered desktop voice assistant built with Python. This assistant listens to your voice commands and performs various tasks like opening apps, playing music, switching tabs, fetching responses from ChatGPT and Botpress, and even sending AI-generated emails.

🧠 Key Features

🗣️ Speech-to-text using Google's speech recognition

🧏 Text-to-speech via Microsoft Edge TTS (Swara neural voice)

🤖 Chat integration with:

    - Open-source Botpress bot

    - GPT-4 using unofficial g4f API

🎮 System automation using pyautogui

🎵 Play YouTube music with pywhatkit

📧 Compose and send AI-written emails via voice

💤 Sleep mode & Wake-up commands

📂 Project Structure
bash
Copy
Edit
.
├── main.py               # Main voice assistant logic
├── bot_scrapper.py       # Selenium-based Botpress chat interaction
├── gpt4.py               # GPT-4 integration (via g4f API)
├── functions/
│   └── emailsender.py    # Email sending logic
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
🔧 Installation
⚠️ Ensure ChromeDriver is installed and compatible with your Chrome version. Place chromedriver.exe in the project root.

1. Clone the repository

bash
Copy
Edit
git clone https://github.com/your-username/desktop-voice-assistant.git
cd desktop-voice-assistant

2. Create a virtual environment (recommended)

bash
Copy
Edit
python -m venv venv
venv\Scripts\activate  # On Windows

3. Install dependencies

bash
Copy
Edit
pip install -r requirements.txt

4. Run the assistant

bash
Copy
Edit
python main.py

🎙️ Voice Commands Examples

Voice Command	     Action

“Open Chrome”	     Opens Chrome via start menu

“Play Believer”	     Plays Believer on YouTube

“Switch tab”	     Moves to next browser tab

“What’s the time?”	 Speaks the current system time

“Write an email”	 Guides you to send an AI-generated email

“Sleep” / “Wake up”	  Sleep mode & reactivation

🤖 Bot Integration
-Botpress: A web automation interface using Selenium scrapes real-time replies from a hosted Botpress chatbot.

-GPT-4 (via g4f): AI generates email content and other natural language responses.

📬 Email Workflow
1. Say: "Write an email"

2. Provide recipient email

3. Speak subject line

4. Provide a prompt (e.g., invite for birthday)

5. GPT will generate email content

6. Email is sent using the predefined function

📌 Requirements
- Python 3.8+
- Google Chrome + ChromeDriver
- Internet connection (for GPT, Botpress, YouTube)
