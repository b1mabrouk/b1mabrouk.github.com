# Video Translation System

An advanced video translation system that converts Turkish speech to Arabic subtitles.

## Features

- Audio extraction from various video formats
- Turkish speech recognition using OpenAI Whisper
- Turkish to Arabic translation using state-of-the-art models
- Automatic subtitle generation and synchronization
- Real-time preview of translated subtitles
- Support for multiple video formats
- Download options for subtitled videos and SRT files

## Prerequisites

- Python 3.8+
- FFmpeg installed on your system
- CUDA-compatible GPU (recommended for faster processing)

## Installation

1. Clone the repository
2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file with your API keys:
```
OPENAI_API_KEY=your_key_here
```

## Usage

1. Start the server:
```bash
uvicorn main:app --reload
```

2. Access the web interface at `http://localhost:8000`

## Project Structure

```
video-translator/
├── backend/
│   ├── main.py              # FastAPI application
│   ├── services/
│   │   ├── audio.py         # Audio extraction
│   │   ├── transcription.py # Speech recognition
│   │   ├── translation.py   # Translation service
│   │   └── subtitles.py     # Subtitle generation
│   └── utils/
│       └── helpers.py       # Utility functions
├── frontend/
│   ├── index.html
│   ├── styles/
│   └── scripts/
└── requirements.txt
```
