# 🎙️ Live Transcription App

This is a real-time audio transcription web app using the **Deepgram Streaming API**. It captures audio from the user's microphone and streams it to Deepgram over a WebSocket connection. The final transcriptions are displayed live on the page.

# Demo

https://github.com/user-attachments/assets/382269d1-1d33-4234-8e6c-49132b9ba22c


## 🚀 Features
- Live microphone input using `getUserMedia`
- WebSocket connection to Deepgram API
- Real-time, streaming transcription display
- Clean and responsive UI with connection status

## 🛠️ Tech Stack
- **HTML5** & **CSS3** – for UI layout and styling  
- **JavaScript** – handles mic input and WebSocket communication  
- **Deepgram API** – for AI-powered live speech-to-text transcription

## 🧠 How It Works
1. User grants mic access.
2. Audio is recorded in chunks (`audio/webm` format).
3. Each chunk is streamed to Deepgram over WebSocket.
4. Final transcriptions are displayed in real-time.

## 🔧 Setup Instructions
1. Clone or download the repository.
2. Replace the WebSocket token with your own Deepgram API key:
   ```js
   const socket = new WebSocket('wss://api.deepgram.com/v1/listen', [
     'token',
     'YOUR_DEEPGRAM_API_KEY',
   ]);
   ```
3. Open `index.html` in a supported browser (Chrome preferred).
4. Start speaking—transcription appears instantly!

## ⚠️ Notes
- Requires a browser that supports `MediaRecorder` with `'audio/webm'`.
- Keep your API key secure—do not expose in public production apps.
- This is an MVP and can be expanded with pause/resume, download, or backend integration.

## 🧪 Demo
Demo link coming soon.

---

Built with 💡 and 🔊 using Deepgram.
