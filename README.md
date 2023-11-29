# WA_ChessScala

## Overview

This Chess Game Project is a web-based application designed for playing chess in a real-time environment. It utilizes a modern tech stack comprising Vue.js for the frontend, Node.js for serving the frontend, and Scala (Play2) for the backend game logic.

## Architecture

The architecture of the Chess Game Project is divided into three main components:

1. **Node.js Server:**
    - Serves the Vue.js Single-Page Application (SPA) to the client.
    - Acts as the entry point for the frontend of the chess game.

2. **Vue.js SPA:**
    - A dynamic and interactive user interface for the chess game.
    - After loading, it establishes a direct WebSocket connection to the Scala (Play2) server for real-time gameplay.

3. **Scala (Play2) Server:**
    - Manages the core game logic, player moves, and maintains the state of the game.
    - Communicates directly with the SPA through WebSockets for a seamless gaming experience.

<br>

![WA_ChessScala_Use_Case.png](images%2FWA_ChessScala_Use_Case.png)

### Use-Case Diagram

The use-case diagram for the Chess Game Project illustrates the following scenarios:

- **Request Chess Game:** Players request the chess game SPA from the Node.js server.
- **Connect to Scala Server:** The SPA establishes a WebSocket connection with the Scala server.
- **Make a Move / Receive Opponent's Move:** Players make moves, and the Scala server updates the game state accordingly. Moves of the opponent are received in real-time.
- **Update Game Status:** The Scala server sends updates about the game status, like checkmate or draw, to the players.

## Project Structure

- `/frontend`: Contains the Vue.js SPA.
- `/backend`: Contains the Scala (Play2) server.
- Each directory has its own `README.md` with specific instructions on setup and running.

## Development and Deployment

Follow the individual `README.md` files in the `/frontend` and `/backend` directories for instructions on setting up and running the respective parts of the application.
