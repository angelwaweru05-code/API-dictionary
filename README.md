## Project Overview
A simple dictionary web app that fetches word definitions, synonyms, and antonyms from the Free Dictionary API.

## File Structure
```
PROJECTS/
├── Dockerfile          # Nginx image for serving the app
├── docker-compose.yml  # Docker Compose service and port mapping
├── index.html          # Main HTML structure
├── index.js            # JavaScript logic (API fetch, DOM manipulation)
├── style.css           # Styling
└── README.md           # This file
```

## Features
- Search for any English word
- Display definitions with part of speech
- Show synonyms and antonyms
- Audio pronunciation
- Fallback data when API is unavailable

## API Used
- Primary: `https://api.dictionaryapi.dev/api/v2/entries/en/{word}`

## Run with Docker

Requirements: Docker Engine and the Docker Compose plugin.

Build and start the app from the project directory:

```bash
docker compose up --build
```

Open [http://localhost:8081](http://localhost:8081). Compose maps host port `8081` to Nginx port `80` in the container.

Stop the app with:

```bash
docker compose down
```

## Run without Docker

1. Open `index.html` directly in a browser, or start a local static server:
   ```bash
   npx serve .
   ```

## Usage
1. Type a word in the search box
2. Click "Search" or press Enter
3. View definitions, synonyms, antonyms
4. Click "Play Pronunciation" to hear the word