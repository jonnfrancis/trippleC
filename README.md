# Music Library Management System

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [Setup and Running the Application](#setup-and-running-the-application)
5. [How to Use the Program](#how-to-use-the-program)
6. [Classes Overview](#classes-overview)
7. [Future Enhancements](#future-enhancements)

## Introduction
The **Music Library Management System** is a command-line application written in Java. It allows users to manage a collection of artists, albums, and songs, as well as create and navigate playlists. This program provides basic library management features, including adding artists, albums, and songs, and allows playlist navigation with next, previous, and shuffle functionality.

## Features
- Add artists, albums, and songs to the music library.
- Display the entire library of artists, albums, and songs.
- Create playlists and add songs to them.
- Navigate through songs in the playlist with `next`, `previous`, and shuffle options.
- Search the library for specific artists, albums, or songs.

## Project Structure
```
MusicLibraryManagementSystem/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── musiclibrary/
│   │   │           ├── Main.java
│   │   │           ├── Artist.java
│   │   │           ├── Album.java
│   │   │           ├── Song.java
                    ├── PlaylistService.java
│   │   │           ├── Playlist.java
│   │   │           └── LibraryService.java
│   │   └── utils/ (Empty for now but optional for assets)
│   ├── test/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── musiclibrary/
│   │   │           ├── ArtistTest.java
│   │   │           ├── AlbumTest.java
│   │   │           ├── PlaylistTest.java
│   │   │           ├── PlaylistServiceTest.java
│   │   │           └── LibraryServiceTest.java
│
├── bin/ (compiled .class files)
├── README.md
├── lib/ (JUNIT jar files)
└── .vscode
```
## Setup and Running the Application

### Requirements
- **Java Development Kit (JDK) 17**
- **JUNIT** (for running tests)
- VS Code terminal or command line environment to run the program.

### Steps to Run the Application

1. **Open the project**:
   ```
   cd MusicLib
   ```

2. **Compile the Code**:
   ```
   javac -d bin src/main/java/com/musiclibrary/*.java
   ```

3. **Run the Program**:
   ```
   java -cp bin main.java.com.musiclibrary.Main
   ```

## How to Use the Program

After starting the program, you will be presented with a menu to interact with the Music Library system.

### Main Menu:
1. **Add Artist**: Enter the artist's name and specify if they are a band.
2. **Add Album**: Enter the album title, artist, and release year.
3. **Add Song**: Enter the song title, artist, and whether it belongs to an album or is a single.
4. **Display Library**: View all artists, albums, and songs in the library.
5. **Manage Playlists**: Create a playlist, add songs, shuffle, and navigate through songs.
6. **Search Library**: Search for specific artists, albums, or songs.
7. **Exit**: Exit the application.

### Playlist Navigation:
- You can navigate through playlists using options for `next song`, `previous song`, and shuffle the playlist.

## Classes Overview

### 1. **Artist.java**
   - Represents an artist or band.
   - Attributes: `name`, `isBand`, `albums`, `singles`.
   - Methods: `addAlbum()`, `addSingle()`, and getters.

### 2. **Album.java**
   - Represents an album that belongs to an artist.
   - Attributes: `title`, `artist`, `year`, `songs`.
   - Methods: `addSong()` and getters.

### 3. **Song.java**
   - Represents a song in the music library system.
   - Attributes: `title`, `artist`, `duration`, `album`.
   - Methods: Getters for song details.

### 4. **Playlist.java**
   - Represents a playlist containing multiple songs.
   - Attributes: `name`, `songs`, `currentIndex`.
   - Methods: `addSong()`, `getNextSong()`, `getPreviousSong()`, `shuffleSongs()`.

### 5. **LibraryService.java**
   - Manages the collection of artists, albums, and songs in the library.
   - Methods: `addArtist()`, `addAlbum()`, `addSong()`, `findArtistByName()`, `findAlbumByTitle()`, `findSongByTitle()`.

### 6. **PlaylistService.java**
   - Manages the playlist, allowing for creating, removing, and navigating through playlists.
   - Methods: `createPlaylist()`, `removePlaylist()`, `shufflePlaylist()`, `nextSong()`, `previousSong()`.

## Future Enhancements
- **File Persistence**: Add functionality to save and load the library and playlists from files.
- **Graphical User Interface (GUI)**: Build a JavaFX-based GUI to make the system more user-friendly.
