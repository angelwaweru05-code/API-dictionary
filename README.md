## Project Overview
A simple dictionary web app that fetches word definitions, synonyms, and antonyms from the Free Dictionary API.

## File Structure
```
PROJECTS/
├── index.html      # Main HTML structure
├── index.js        # JavaScript logic (API fetch, DOM manipulation)
├── style.css       # Styling
└── README.md       # This file
```

## Features
- Search for any English word
- Display definitions with part of speech
- Show synonyms and antonyms
- Audio pronunciation
- Fallback data when API is unavailable

## API Used
- Primary: `https://api.dictionaryapi.dev/api/v2/entries/en/{word}`

## How to Run
1. Open `index.html` in a browser
2. Or use a live server:
   ```bash
   npx serve .
   
   ```

## Usage
1. Type a word in the search box
2. Click "Search" or press Enter
3. View definitions, synonyms, antonyms
4. Click "Play Pronunciation" to hear the word