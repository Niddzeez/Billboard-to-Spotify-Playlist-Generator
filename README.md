# Billboard to Spotify Playlist Generator 🎶

This Python project allows you to travel back in time musically! By scraping the Billboard Hot 100 chart for a given date, it creates a private Spotify playlist with the top 100 songs from that day.

## 📚 Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Configuration](#configuration)
- [Examples](#examples)
- [Troubleshooting](#troubleshooting)
- [Contributors](#contributors)
- [License](#license)

## 📌 Introduction

This tool scrapes the Billboard Hot 100 chart for a user-specified date and creates a private Spotify playlist containing those songs, using the Spotify Web API. It uses BeautifulSoup for scraping and Spotipy for Spotify integration.

## ✨ Features

- Scrapes Billboard Hot 100 chart from a specific date.
- Searches for each song on Spotify.
- Creates a private playlist in your Spotify account.
- Automatically adds all found songs to the playlist.
- Gracefully handles missing songs.

## 💾 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/billboard-spotify-playlist.git
   cd billboard-spotify-playlist
   ```
2. Create and activate a virtual environment (optional but recommended):
  ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows use `venv\Scripts\activate`
  ```
3. Install required dependencies:
  ```bash
  pip install -r requirements.txt
  ```

## ⚙️ Dependencies

- requests
- beautifulsoup4
- spotipy

To install manually
  ```bash
  pip install requests beautifulsoup4 spotipy
  ```

## 🛠 Configuration
To run this script, you need:

Spotify Developer Credentials:

-Go to the Spotify Developer Dashboard
-Create an app and get your Client ID and Client Secret
-Set the redirect URI to something like https://example.com/callback (must match your script)

Replace the placeholders in the script:
  ```bash
  client_id = "YOUR_CLIENT_ID"
  client_secret = "YOUR_CLIENT_SECRET"
  ```

## 🚀 Usage
Run the script: main.py
Then input a date in the format YYYY-MM-DD

It will:

-Scrape Billboard for top 100 songs on that date
-Authenticate with Spotify
-Create a private playlist
-Add available tracks

## 💡 Examples

```bash
> python main.py
Which year do you want to travel to? Type the date in this format YYYY-MM-DD: 1995-07-14
✔ Playlist '1995-07-14 Billboard 100' created!
✔ Added 87 out of 100 songs.
```

## 🐞 Troubleshooting

- Authentication failed: Make sure the client_id, client_secret, and redirect URI match your Spotify Developer Dashboard settings.
- Songs missing: Not all Billboard songs are available on Spotify. These are skipped with a message.
- Permission errors: Ensure your Spotify account allows playlist modifications

## 👥 Contributors

NIDHI LODHA — Author and Developer

## 📄 License

This project is licensed under the MIT License. 





 





