# GRAMMER-GURU
# PIPELINE
```
🎤 Voice Sample (.wav)
     ↓
🧠 Deepgram STT → transcript
     ↓
🔍 spaCy preprocessing + rule-based grammar analysis
     ↓
🤖  LLM → grammar score + natural feedback
     ↓
📦 JSON Response (score, feedback, transcript)
```


## How To Run
```bash
conda create  -n grammer-guru --file requirements.txt
conda activate grammer-guru
python -m spacy download en_core_web_sm
uvicorn app.main:app --reload
streamlit run frontend/main.py
docker compose up -d # Don't run in your local as you don't have docker installed
```