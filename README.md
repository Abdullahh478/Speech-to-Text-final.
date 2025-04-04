# 🎤 Speech-to-Text & Sentiment Analysis Pipeline

A complete machine learning pipeline that demonstrates the real-world use of **speech recognition** and **natural language processing (NLP)**.

This project takes text data (YouTube comments), synthesizes it into audio, transcribes it back into text using OpenAI's Whisper model, and then performs **sentiment analysis** to determine whether the content is positive, negative, or neutral. It also measures how accurate the transcription was using **Word Error Rate (WER)**.

---

## 🔍 Project Overview

This system is divided into two core pipelines:

### 🗣️ 1. **Speech-to-Text (STT) Pipeline**
- Scrape text data (YouTube comments)
- Convert text to audio using `gTTS` (Google Text-to-Speech)
- Transcribe audio using OpenAI’s Whisper model
- Evaluate transcription accuracy using `jiwer.WER`

### 💬 2. **NLP Sentiment Analysis Pipeline**
- Tokenize transcribed text using `TextBlob`
- Classify sentiment polarity
- Label sentiment as Positive, Negative, or Neutral
- Combine results into a single, exportable dataset

---

## 🧠 Technologies & Libraries Used

| Tool / Library | Purpose |
|----------------|---------|
| `youtube-comment-downloader` | Scrape YouTube video comments |
| `gTTS` | Convert text into audio (speech) |
| `whisper` | Transcribe speech to text |
| `textblob` | NLP: tokenization and sentiment analysis |
| `jiwer` | Calculate Word Error Rate (accuracy) |
| `pandas` | DataFrame creation and Excel export |
| `tqdm` | Progress bars |
| `ffmpeg` | Required for audio handling |

---
