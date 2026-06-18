# Drop

Drop is a small [libGDX](https://libgdx.com/) desktop game. Move the bucket left and right to catch the falling droplets while the background music loops and the drop sound plays on each catch.

## Gameplay

- Catch falling droplets with the bucket.
- Use the left and right arrow keys to move.
- The game uses a fixed world size and a `FitViewport` so the play area stays consistent across window sizes.

## Requirements

- A Java Development Kit installed locally.
- Gradle Wrapper support through `gradlew` or `gradlew.bat`.
- A current JDK is recommended for development and packaging; the project targets Java 8 bytecode for the game modules.

## Run

Run the desktop version from the project root:

```bash
./gradlew lwjgl3:run
```

On Windows:

```bat
gradlew.bat lwjgl3:run
```

## Build

Common Gradle tasks:

- `./gradlew build` - compile and test all modules.
- `./gradlew clean` - remove build outputs.
- `./gradlew lwjgl3:jar` - create a runnable desktop JAR.
- `./gradlew lwjgl3:jarWin` - create a Windows-only JAR.
- `./gradlew lwjgl3:jarLinux` - create a Linux-only JAR.
- `./gradlew lwjgl3:jarMac` - create a macOS-only JAR.

## Controls

- `Left Arrow` - Move bucket left.
- `Right Arrow` - Move bucket right.

## Notes

- The desktop launcher lives in `lwjgl3/src/main/java/com/badlogic/drop/lwjgl3/Lwjgl3Launcher.java`.
- The main game logic lives in `core/src/main/java/com/badlogic/drop/Main.java`.
- Assets are loaded from the `assets` directory during desktop runs.
