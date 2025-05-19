# Mod Format
## Here be dragons! Anything here may be subject to change at any point.

## Mod Metadata (Required)
The mod metadata file is titled `mod.json`, and includes information such as the mods developer, title, description, version, and identifier, along with the destination games identifier and version.

```json
{
  "title": "Example Mod", // This is the title of your mod. (required)
  "description": "This is an example mod for the Godot Modloader!", // This is the description of your mod. Write a 1-2 sentence blurb here! (optional)
  "author": "Godot Modding", // That's you! (optional)
  "id": "org.godotmods.example_mod", // This is a unique identifier for your game. (required)
  "version": "1.0.0", // The version of your game. Ideally follows semver standard. (required)
  "destid": "org.godotmods.example_game", // The unique identifier for whatever game you are modding. Not including this means it's compatible with any game, likely because it's either a universal library or a directly Godot engine related tool. (optional)
  "destversions": "1.x" // If you include destid, this is the version of the game. If you do not, this is the version of Godot you are targetting. Non-matching versions will give a warning, not an error. (required)
}
```
