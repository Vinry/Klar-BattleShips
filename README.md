# Battleships (Sänka Skepp)

A Java console Battleships game from university coursework, created by **Martin and Paul**. The original Swedish interface and source code are preserved as a historical project.

The game includes human and computer players, manual or automatic ship placement, turn-based play, and a local high-score table.

## Build and play

A Java Development Kit (JDK) is required. Expected commands from the repository directory:

```sh
mkdir -p out
javac -encoding windows-1252 -d out *.java
java -cp out SankaSkepp.Main
```

The encoding option is needed for the original Swedish characters in the source files. The game reads and writes `highscore.txt` in the working directory; a missing file is reported when no scores have been saved yet.

The menu offers high scores, score reset, and a new game. At the player-count prompt, `0` selects computer-versus-computer play, `1` selects a human against the computer, and larger values select human players. Board coordinates use letters `A`–`J` and digits `0`–`9`, for example `A0`.

## Project status

This is coursework preserved for reference, not a polished game release. Input validation is limited: blank or incomplete coordinates can terminate a game. There is no automated test suite, and game rules and scoring still need systematic verification.

The implementation demonstrates object-oriented modeling, collections, console interaction, and file persistence. The in-game credit to Martin and Paul is retained; individual contributions are not documented in this repository.
