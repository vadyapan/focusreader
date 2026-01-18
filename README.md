# FocusReader

**FocusReader** is a lightweight, distraction-free web application designed to help you read PDFs and track your reading time. It runs entirely in your browser with no backend required—your files and data stay private on your device.

## Features

- 📚 **Local Library Management**
  - Upload and store PDFs directly in the browser using **IndexedDB**.
  - Books are saved permanently (until cleared) without needing a server.
  - View cumulative reading time for every book in your library.

- ⏱️ **Focus Timer & Progress Tracking**
  - Set custom reading sessions (e.g., 20 minutes).
  - Visual circular timer countdown.
  - Automatic progress tracking: Time is saved to your book's history when you finish or save a session.

- 🎵 **Ambient Soundscapes**
  - Built-in ambient noise generator using the **Web Audio API**.
  - Select from Plane (low hum) or Train (rhythmic rumble) to mask distractions.
  - No external audio files needed—sounds are synthesized on the fly.

- 🎨 **Clean Interface**
  - Minimalist, focus-oriented layout.
  - Collapsible sidebar for maximum reading space.
  - Responsive design for desktop and mobile.

## Getting Started

Go to https://vadyapan.github.io/focusreader

## Usage Guide

1. **Upload:** Drag and drop a PDF file or click to browse. The book will appear in your library.
2. **Read:** Click "Read" on a book card.
3. **Timer:**
   - Enter session duration (e.g., 20 mins).
   - Click Start to begin the countdown.
   - Click Pause/Resume as needed.
   - Click Reset to commit your time to the book's total record.
4. **Ambient Sound:** Toggle "Plane" or "Train" at the bottom of the sidebar to play background noise.
5. **Collapse:** Click the arrow icon in the sidebar to minimize the controls and view the full PDF.

## Technical Details

- **Storage:** Uses **IndexedDB** for client-side storage. This allows large binary files (PDFs) to be saved efficiently without server uploads.
- **Audio:** Uses **Web Audio API** (Oscillators & Noise Buffers) to generate Brown Noise (rumble) and modulate it, simulating real environments without loading MP3s.
- **Architecture:** Single Page Application (SPA) built with Vanilla JavaScript, HTML5, and CSS3. No frameworks or build tools required.

## License

This project is open source and available for personal use.
