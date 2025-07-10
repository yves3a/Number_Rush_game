# Number Rush Game

An object-oriented, modular multiplayer game focused on finding numbers.

## Features

- Two-player local mode
- Online multiplayer with support for up to 10 players
- Multiple language options
- Custom key bindings
- Clean structure with reusable components

## Prerequisites

- [Bun](https://bun.sh) or [Node.js](https://nodejs.org/) – Required to run and manage JavaScript packages
- A modern browser

## Installation

1. Clone the project repository:
   ```bash
   git clone https://github.com/yourusername/number-rush-game.git
   cd number-rush-game
   ```

2. Install the dependencies:
   ```bash
   npm install
   # OR
   bun install
   ```

## Running the Game

### Development Mode (Local)

Start the development server with live reload:
```bash
npm run dev
# OR
bun run dev
```

Access the game at http://localhost:3000 via your browser.

### Multiplayer Server

Launch the server for online play:
```bash
npm run server
# OR
node server/index.js
```

This starts a Socket.io server to handle multiplayer connections.

## How to Play

### Local Mode
1. Launch the game in your browser
2. Input names for each player
3. Modify controls if preferred
4. Press your confirm keys to get ready
5. Locate and click numbers in order

### Online Multiplayer
1. Select "Play Multiplayer" from the main screen
2. Create a room or join one using a room code
3. Enter your name and set your controls
4. Wait for others to join
5. Click "Ready" when set
6. Compete to find numbers in sequence and score

## Building for Production

Generate a production-ready version of the game:
```bash
npm run build
# OR
bun run build
```

The final build will be saved in the `dist` directory.

## Project Structure

- `src/` – Game source code
  - `main.js` – Local mode entry file
  - `styles/` – CSS files
  - `utils/` – Core logic for local mode
    - `game.js` – Main game engine
    - `player.js` – Player behavior
    - `board.js` – Gameboard logic
    - `translator.js` – Manages language translations
    - `settings.js` – Handles game settings
    - `ui-manager.js` – Manages UI elements
  - `multiplayer/` – Multiplayer mode files
    - `main.js` – Multiplayer entry point
    - `game.js` – Multiplayer logic
    - `player.js` – Multiplayer player class
    - `board.js` – Multiplayer board functionality
    - `ui-manager.js` – Multiplayer UI control
- `server/` – Multiplayer backend
  - `index.js` – Socket.io server code

## License

MIT
