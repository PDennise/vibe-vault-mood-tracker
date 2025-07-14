VibeVault -Mood Tracker-

## Project Overview
VibeVault is a terminal-based mood tracking application that allows users to log their daily emotions using free-text entries. The app performs sentiment analysis using NLP (TextBlob), stores mood data in a JSON file, and visualizes mood trends over time using matplotlib.

This tool aims to help users understand their emotional patterns and promote mindfulness through self-reflection.

---


## 🌟 Features

✅ Track daily mood with a text entry  
✅ Analyze sentiment (polarity & subjectivity) with TextBlob  
✅ Automatically timestamp each entry  
✅ Store all entries locally in a JSON file  
✅ Visualize mood trends over time with matplotlib  
✅ Export data to CSV  
✅ Graceful error handling for empty inputs or missing data  
✅ CLI-based interaction with a user-friendly menu  
✅ Future-ready: tags, emotion classification, time-of-day logging  

---

🚀 Installation
1. Clone the repository:
    git clone https://github.com/PDennise/vibe-vault-mood-tracker.git
    cd vibe-vault-mood-tracker
2. Create and Activate Virtual Environment
    For Mac/Linux:
        python3 -m venv venv
        source venv/bin/activate
    For Windows:
        python -m venv venv
        venv\Scripts\activate

3. Install the required libraries:
    pip install -r requirements.txt
    
4. Run the app:
    python3 main.py
