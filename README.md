# Tic Tac Toe Classic (React)

A simple, modern Tic Tac Toe game where two players can play on the same device. The app provides a classic 3×3 grid, turn tracking, win/draw detection, a result banner, and an easy reset to start a new match.

> Container: `tic_tac_toe_frontend` (runs on port **3000**)

---

## Key Features

- 3×3 Tic Tac Toe grid
- Two-player gameplay on the same device (local play)
- Turn tracking (Player X / Player O)
- Win detection (3 in a row: horizontal, vertical, diagonal)
- Draw detection when the board fills with no winner
- Result display (winner or draw)
- Restart/reset to play again

---

## Tech Stack

- **React 18** (Create React App / `react-scripts`)
- **Node.js** (recommended: latest LTS)
- **npm** (or yarn)

---

## Getting Started

### Prerequisites
- Node.js (latest LTS recommended)
- npm (bundled with Node) or yarn

### Install
From the repository workspace root:

```bash
cd tic-tac-toe-classic-313900-313909/tic_tac_toe_frontend
npm install
```

### Run (Development)
```bash
npm start
```

Then open:
- http://localhost:3000

### Build (Production)
```bash
npm run build
```

This outputs a production build to `tic_tac_toe_frontend/build`.

### Preview Notes
Create React App does not include a built-in `preview` command like Vite. To preview the production build you can serve the `build/` directory using a static file server (how previews are started may vary depending on your system/environment and is typically handled externally).

---

## Available Scripts

In `tic_tac_toe_frontend/`, you can run:

- `npm start`  
  Runs the app in development mode.

- `npm test`  
  Runs tests in watch mode (if supported by your environment).

- `npm run build`  
  Builds the app for production to the `build` folder.

- `npm run eject`  
  Ejects CRA configuration (one-way operation).

If you prefer yarn, the equivalent commands are usually:
- `yarn start`, `yarn test`, `yarn build`, `yarn eject`

---

## Environment Variables

The frontend includes a `.env` file defining these variables:

- `REACT_APP_API_BASE`
- `REACT_APP_BACKEND_URL`
- `REACT_APP_FRONTEND_URL`
- `REACT_APP_WS_URL`
- `REACT_APP_NODE_ENV`
- `REACT_APP_NEXT_TELEMETRY_DISABLED`
- `REACT_APP_ENABLE_SOURCE_MAPS`
- `REACT_APP_PORT`
- `REACT_APP_TRUST_PROXY`
- `REACT_APP_LOG_LEVEL`
- `REACT_APP_HEALTHCHECK_PATH`
- `REACT_APP_FEATURE_FLAGS`
- `REACT_APP_EXPERIMENTS_ENABLED`

Most of these are template/general-purpose and **can remain unset** for this project, since Tic Tac Toe is a fully local frontend game (no backend required). If your deployment platform uses a different port or base URL, you may optionally set `REACT_APP_PORT` / `REACT_APP_FRONTEND_URL`.

> Note: Create React App only exposes env vars prefixed with `REACT_APP_` to the browser build.

---

## Project Structure (High Level)

```text
tic-tac-toe-classic-313900-313909/
  README.md                     # (this file)
  tic_tac_toe_frontend/
    package.json
    public/
      index.html
      manifest.json
      robots.txt
      favicon.ico
    src/
      App.js
      App.css
      index.js
      index.css
      App.test.js
      setupTests.js
```

---

## Style / Theme Notes

The intended style follows a **light theme** with modern UI accents:
- **Primary:** `#3b82f6`
- **Success/Accent:** `#06b6d4`

If you update UI components, try to keep consistent spacing, clear contrast, and a centered board layout (player info + result display near the board, with a restart button available after the game ends).

---

## How to Play (Gameplay Instructions)

1. Player **X** starts.
2. Click/tap an empty square to place your mark.
3. Players alternate turns (**X** then **O**).
4. The game ends when:
   - A player gets 3 in a row (win), or
   - All squares are filled (draw)
5. Use the **Restart/Reset** action to start a new match.

---

## Future Improvements

- Highlight the winning line (three winning squares)
- Add move history / “time travel” (undo/redo)
- Add scoreboard across rounds
- Add animations and subtle sound effects
- Add accessibility enhancements (keyboard navigation + ARIA for board cells)
- Add optional single-player mode (basic AI)

---

## License

TODO: Add license (e.g., MIT) and update this section accordingly.
