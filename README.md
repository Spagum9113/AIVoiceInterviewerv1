# AI Voice Interviewer v1

A real-time, voice-based interview system powered by OpenAI's Realtime API. This project simulates an AI interviewer conducting an internship interview with a candidate (e.g., Ethan), asking questions about background, skills, experience, and motivation. It uses WebSockets for audio streaming, FastAPI for the server, and logs latency metrics for performance analysis.

## Features
- **Real-Time Audio Interaction**: Streams audio input/output via WebSockets using OpenAI's `gpt-4o-realtime-preview-2024-10-01` model.
- **Customizable Interview Flow**: Starts with a warm greeting, asks 5-7 tailored questions, and adapts follow-ups based on responses.
- **Latency Tracking**: Measures and logs the time from speech end to AI response for optimization.
- **Friendly & Professional Tone**: Designed to create a relaxed, supportive interview experience.
- **Audio Format**: Uses `g711_ulaw` for input and output audio compatibility with telephony systems (e.g., Twilio).

## Prerequisites
- Python 3.13.2 or higher
- An OpenAI API key with access to the Realtime API (set as an environment variable: `OPENAI_API_KEY`)
- A Twilio account (optional, for telephony integration) with credentials configured
- Dependencies listed in `requirements.txt`

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/ai-voice-interviewer-v1.git
   cd ai-voice-interviewer-v1
