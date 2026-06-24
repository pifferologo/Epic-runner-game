# Epic Runner

A fast-paced endless runner built with **Unity** and exported as a **WebGL** build. Play directly in your browser — no install required.

## Overview

Epic Runner is a browser-based arcade game where you dodge obstacles, keep moving, and chase your best score. This repository contains the published WebGL player and assets ready to host or run locally.

## Features

- Instant play in modern web browsers
- Responsive layout for desktop and mobile
- Fullscreen support
- Compressed WebGL build (Brotli) for faster loading

## Tech Stack

| Layer | Technology |
|-------|------------|
| Engine | Unity |
| Platform | WebGL |
| Frontend | HTML5, CSS, JavaScript |
| Compression | Brotli (`.br`) |

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, or Safari)
- A local HTTP server (required — opening `index.html` directly from disk may block WebGL asset loading)

### Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-org>/Epic-runner-game.git
   cd Epic-runner-game
   ```

2. Start a local server from the project root. Examples:

   **Python 3**

   ```bash
   python -m http.server 8080
   ```

   **Node.js (npx)**

   ```bash
   npx serve .
   ```

3. Open `http://localhost:8080` in your browser.

4. Wait for the loading bar to finish, then click the fullscreen button if you want an immersive view.

## Project Structure

```
Epic-runner-game/
├── Build/                 # WebGL build output (loader, wasm, data)
├── TemplateData/          # Unity player UI assets and styles
├── index.html             # Game entry point
└── README.md
```

## Deployment

Host the entire repository contents on any static file host (GitHub Pages, Netlify, Vercel, etc.). Ensure your server serves Brotli-compressed files (`.br`) with the correct `Content-Encoding: br` header when possible.

## Version

- **Product:** Epic_runner  
- **Version:** 1.0.0

## License

All rights reserved unless otherwise specified by the project owner.
