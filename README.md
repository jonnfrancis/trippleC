# Playlist Manager

## Project Overview

This Java-based **Playlist Manager** allows users to manage playlists, including creating, deleting, and switching between playlists, adding or removing songs, shuffling the playlist, and saving/loading playlists from a file.

Users can:
- Navigate through the playlist (play next/previous song).
- Shuffle the playlist.
- Add and remove songs dynamically.
- Create and switch between multiple playlists.
- Save the current playlist to a file and load playlists from a file.

## Features
- **Song Management**: Add or remove songs from the current playlist.
- **Playlist Management**: Create, delete, and switch between multiple playlists.
- **Playlist Navigation**: Play next, previous, or shuffle songs in the current playlist.
- **File I/O**: Save the current playlist to a file and load playlists from a file.

## Usage

### Running the Program
1. Navigate to the `src/` directory:
   ```
   cd src
   ```
2. Compile the Java files:
   ```
   javac Main.java models/*.java
   ```
3. Run the program:
   ```
   java Main
   ```

### Dependencies
***JUnit*** - For running tests.

## Commands
Once the program is running, the following commands are available:
- `next`: Play the next song.
- `previous`: Play the previous song.
- `shuffle`: Shuffle the current playlist.
- `display`: Display all songs in the current playlist.
- `manage playlists`: Access the playlist management menu (create, delete, display, switch).
- `manage songs`: Access the song management menu (add, remove).
- `save`: Save the current playlist to a file.
- `exit`: Exit the program.

## File IO
- **Saving Playlists**: Use the save command and specify a filename to save the current playlist.
- **Loading Playlists**: If a playlist file exists, the program automatically loads songs from the file during program startup.

### Example Commands:
```
Enter command: next
Now playing: Wunna,
 Artist: Gunna,
 Album: Ds4eva, (344 seconds)
```
```
Enter command: manage songs
Song Management Commands: add, remove, back
```

## File Structure
- `Main.java`: Handles user interactions and the main loop.
- `models/`:
  - `Song.java`: Represents a song, with attributes like title, duration, artist, and album.
  - `Artist.java`: Represents an artist or band.
  - `Album.java`: Represents an album containing multiple songs.
  - `Playlist.java`: Handles a collection of songs.
- `services/`:
  - `PlaylistManager.java`: Handles playlist-related operations (e.g., adding/removing songs, navigating the playlist, file I/O).
 
## Recursive Structure in Playlist Class
The `Playlist.java` class uses a recursive structure to manage multiple playlists. Specifically, not only does the playlist store songs, but it also employs recursion to store other playlists. 
 
## Future Enhancements
- Ability to edit song details after creation.
- Support for loading and saving playlists in JSON format.
- Stop using CLI and create a GUI











   
