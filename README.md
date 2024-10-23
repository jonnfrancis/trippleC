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
Now playing: Song: Shape of You, Artist: Ed Sheeran, Duration: 240 seconds
```
```
Enter command: manage songs
Song Management Commands: add, remove, back
```









   
