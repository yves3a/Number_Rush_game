Shaka Game
A modular, object-oriented multiplayer game focused on number-finding challenges.

Key Features
Supports two-player local gameplay

Online multiplayer for up to 10 participants

Multi-language interface

Customizable key bindings

Clean, modern architecture with reusable modules

Requirements
Bun or Node.js – Required to run the project and manage dependencies

A modern web browser

Getting Started
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/shaka-game.git
cd shaka-game
Install necessary packages:

bash
Copy
Edit
npm install
# OR
bun install
Running the Game Locally
To launch the development environment with live reloading:

bash
Copy
Edit
npm run dev
# OR
bun run dev
The game will be served via Vite at http://localhost:3000.

Multiplayer Server
To start the server for online play:

bash
Copy
Edit
npm run server
# OR
node server/index.js
This initializes the Socket.io server for real-time multiplayer gameplay.

Gameplay Instructions
Local Mode
Open the game in your browser

Enter names for both players

Adjust controls if needed

Press the confirmation keys to begin

Find and click numbers in order

Online Multiplayer Mode
Select "Play Multiplayer" from the main menu

Either create a new room or join one using a room code

Input your name and configure controls

Wait for others to join

Press "Ready" to start the game

Score by clicking numbers in the correct order

Production Build
To compile the game for deployment:

bash
Copy
Edit
npm run build
# OR
bun run build
The production-ready files will be placed in the dist directory.

Folder Overview
src/ – Main source code

main.js – Local game entry point

styles/ – Styling files

utils/ – Core game modules for local mode

game.js – Game logic controller

player.js – Handles player data and input

board.js – Grid and number layout

translator.js – Manages multilingual support

settings.js – Game settings manager

ui-manager.js – Controls user interface

multiplayer/ – Code for online multiplayer

main.js – Multiplayer entry file

game.js – Multiplayer game logic

player.js – Multiplayer player logic

board.js – Multiplayer game board logic

ui-manager.js – UI management for online mode

server/ – Multiplayer server-side logic

index.js – WebSocket server using Socket.io

License
Licensed under the MIT License.
