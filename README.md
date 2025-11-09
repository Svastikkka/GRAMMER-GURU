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
python -m spacy download en_core_web_sm
uvicorn app.main:app --reload

```