# Aurora Music Player - Repo Structure

This repo powers the Aurora Music Player app. Below is the folder structure:

```
Mp3Player/
├── Albums/
│   └── Albums/
│       └── Sample Album/           ← One folder per album
│           ├── album.json          ← Album metadata (name, artist, cover, etc.)
│           ├── songs.json          ← Metadata for all songs in the album
│           └── 01-sample-track.mp3 ← Actual MP3 files
│
├── Playlists/
│   └── My Playlist/                ← One folder per playlist
│       └── playlist.json           ← Playlist metadata + song refs
│
├── Songs/
│   └── Sample Track/               ← One folder per standalone single
│       ├── song.json               ← Song metadata + lyrics
│       └── sample-track.mp3        ← The MP3 file
│
└── Artists/
    └── artist.json                 ← Your artist profile
```

## How to add an album
1. Create a folder inside `Albums/Albums/Your Album Name/`
2. Add `album.json` (copy from `Sample Album` and edit)
3. Add `songs.json` (copy and edit, one entry per MP3)
4. Upload your `.mp3` files into the same folder

## How to add a standalone song
1. Create a folder inside `Songs/Your Song Name/`
2. Add `song.json` with metadata + lyrics
3. Upload the `.mp3` file

## How to add a playlist
1. Create a folder inside `Playlists/Your Playlist Name/`
2. Add `playlist.json` referencing songs by their album + filename

## Artist profile
Edit `Artists/artist.json` with your bio, photo URL, social links, etc.
