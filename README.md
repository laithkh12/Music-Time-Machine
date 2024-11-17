# Billboard 100 to Spotify Playlist Creator

This Python script allows you to create a private Spotify playlist based on the Billboard Hot 100 chart for any given date.

## Description

The script performs the following tasks:
1. Scrapes the Billboard Hot 100 chart for a specific date.
2. Searches Spotify for songs based on the Billboard chart.
3. Creates a private Spotify playlist and adds the found songs to it.

## Requirements

Make sure you have the following Python packages installed:

- `beautifulsoup4` (for web scraping)
- `requests` (for making HTTP requests)
- `spotipy` (for interacting with the Spotify API)

You can install them using pip:

```bash
pip install beautifulsoup4 requests spotipy
```
---
## Getting Started
### 1.Scraping the Billboard 100
The script prompts the user to input a date in the format YYYY-MM-DD. It then scrapes the Billboard Hot 100 for that specific date.
### 2.Spotify Authentication
You will need to set up your Spotify Developer account to get your Client ID and Client Secret. Once obtained, replace the placeholders YOUR-CLIENT-ID and YOUR-CLIENT-SECRET in the script with your credentials.
To authenticate, the script uses the spotipy library with OAuth2.0.
### 3.Searching for Songs on Spotify
The script searches for each song title from the Billboard Hot 100 list on Spotify. If a song is found, its URI (unique Spotify identifier) is added to the list of songs for the playlist.
### 4.Creating a Playlist
The script creates a new private playlist in your Spotify account and adds the found songs.
---
## Usage
1. Clone the repository or copy the code to your local machine.
2. Run the script
3. Input a date when prompted (e.g., 1999-11-17).
4. The script will authenticate with Spotify, create the playlist, and add the songs.
---
## Troubleshooting
- Spotify Authentication Error:
  - Ensure your Spotify Developer credentials are correct, and check that the redirect URI matches the one in your Spotify Developer dashboard.
- Song Not Found:
  - If a song from the Billboard chart is not found on Spotify, it will be skipped with a message indicating the issue.
---
## Notes
- The playlist created will be private.
- Ensure that your Spotify account is linked and you have access to the necessary permissions to create playlists.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
