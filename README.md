# Clickbait Detector & News Summarizer

CS4100 Artificial Intelligence final project. Two-part system that detects clickbait headlines and summarizes news articles.

## Components

### Clickbait Detection
Bidirectional LSTM with attention mechanism for sequence classification. The hierarchical structure processes word-level representations into sentence-level, then document-level for final classification.

### News Summarization
Transformer-based architecture for abstractive summarization. Generates concise summaries of news articles.

## Running

Install dependencies:
```bash
pip install -r requirements.txt
```

Run detection:
```bash
python clickbait_detector.py
```

Run summarization:
```bash
python summarizer.py
```

## Architecture Notes

The clickbait detector uses:
- Word embeddings -> BiLSTM encoder
- Attention over time steps for context
- Fully connected classification head

The summarizer follows standard transformer encoder-decoder pattern with attention.
