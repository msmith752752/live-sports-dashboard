# Live Sports Dashboard

## Overview

Live Sports Dashboard is a real-time web-based dashboard that consumes live sports data and presents it in a clean, visual format with contextual insights.

The application is designed as a **second-screen experience** and can also be used as a **streaming overlay**, helping users quickly understand what is happening in a game without watching the full broadcast.

---

## Features

* **Real-time score updates**
  Automatically pulls live game data and refreshes every 15 seconds.

* **Game state awareness**
  Displays quarter, clock, and current game status.

* **Contextual insights engine**
  Interprets game conditions to surface insights such as:

  * Clutch situations
  * Tight games
  * Blowout scenarios
  * Lead changes

* **Dynamic UI styling**

  * Team-based color themes
  * Clean, centered layout optimized for readability
  * Designed for both standalone viewing and OBS overlays

* **Extensible architecture**

  * Placeholder support for betting metrics (spread, total, moneyline)
  * Easy integration with additional APIs

---

## Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Data Source:** Live sports API (ESPN public scoreboard endpoint)
* **Rendering:** Browser-based (compatible with OBS Browser Source)

---

## How It Works

1. The app polls a live sports API endpoint at regular intervals.
2. It identifies the target game based on team abbreviations.
3. Game data is parsed and rendered to the UI.
4. A lightweight “insight engine” analyzes score margin and game state to generate contextual messaging.

---

## Use Cases

* Second-screen companion for live sports viewing
* Streaming overlays (OBS Browser Source)
* Real-time data dashboard examples
* UI/UX experimentation for live data applications

---

## Setup

1. Clone the repository
2. Open the project folder
3. Launch the app:

Option A:

* Double-click `index.html`

Option B (recommended for live data):

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/index.html
```

---

## Configuration

Update the following variables in `index.html`:

```javascript
const TEAM_A = "DET";
const TEAM_B = "ORL";
const GAME_DATE = "YYYYMMDD";
```

---

## Roadmap

* Live betting odds integration (API-based)
* Momentum tracking (run detection)
* Multi-game dashboard view
* Animation and visual enhancements
* Mobile-responsive layout
* Backend service for persistent data processing

---

## Disclaimer

This project is for educational and informational purposes only.
No copyrighted video or audio content is used.
Any displayed odds or data should not be considered financial or betting advice.

---

## Author

Matthew Smith

---

## License

MIT License

