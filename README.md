# Tetris (Smiley Match Game)

A Java desktop puzzle game inspired by Tetris — match four or more identical smiley tiles in a row to clear them, built with Java Swing/AWT in NetBeans.

## How It Works

- Smiley tiles pile up in a grid; matching four or more in a row clears them, Tetris-style
- Clearing a match shifts the tiles above down to fill the gap
- 19 levels, each increasing the fall speed of incoming tiles for added difficulty

## Technical Highlights

- Custom linked list to track each tile's current vs. previous grid position for match comparison
- `javax.swing.Timer` + `ActionListener` driving the game loop and per-level speed increases
- Sound effects via `java.applet.AudioClip`, loaded from local file URLs
- `MalformedURLException` handling around sound-file loading

## Tech Stack

Java, Swing/AWT, NetBeans

## Running the Project

1. Open the project in NetBeans, or import the `.java` files under `src/` into your IDE of choice.
2. Keep the `IMAGES` and `sounds` folder and file names unchanged — they're referenced directly by filename in code. If you rename a file, update the matching reference in code.
3. Run the main class from NetBeans.

## Notes

Built as a two-person course project. The trickiest parts were getting the linked-list-based match detection right and keeping tile sizing consistent across the grid.
