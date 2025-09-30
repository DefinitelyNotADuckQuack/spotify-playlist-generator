# Billboard 100 Playlist Generator 

This Python project scrapes the Billboard Hot 100 songs for a given date and automatically creates a private Spotify playlist with those songs.  

It combines **web scraping** (Billboard website) and the **Spotify Web API** via the `spotipy` library.  

---

## Features  
-  Scrapes Billboard Hot 100 songs for a given date (YYYY-MM-DD).  
-  Searches for each song on Spotify.  
-  Automatically creates a private playlist in your Spotify account.  
-  Adds all found songs to the new playlist.  

---

## Installation  

1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo requests beautifulsoup4 spotipy
   
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   
3. Or manually install them:

   ```bash
   requests
   beautifulsoup4
   spotipy

4. Set up your Spotify Developer credentials.

 # Spotify Developer Setup

- Go to the Spotify Developer Dashboard

- Create an app to obtain your client_id and client_secret.

- Add a Redirect URI (e.g., https://example.com/) in the app settings.

- Replace the placeholders in the code with your credentials:

   ```bash
  client_id="YOUR_CLIENT_ID",
   client_secret="YOUR_CLIENT_SECRET",
  
# Authentication (Token)

Before running the script, you must manually authenticate with Spotify and obtain an OAuth token:

- Use your app credentials (`client_id, client_secret, redirect_uri`) to request authorization from Spotify.
- You can do this with the Spotipy documentation
 or directly via the OAuth flow.

- After granting access, Spotify will return a token.

- Save this token in a file called `token.txt` in the project directory.

- The script will read this file to authenticate.

- If the token expires, you’ll need to refresh it or generate a new one.

---