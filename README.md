# Contributing to StellarModManager

Thank you for your interest in contributing to the StellarModManager! If you wish to add your mod to the database follow the steps below.

## Adding a New Mod

To add your mod to the repository, please follow these steps:

1. **Fork this repository** to your own GitHub account.
2. **Add your mod entry** to the `mods.json` file.
3. **Ensure your mod zip follows the required structure** (see below).
4. **Open a Pull Request** against the main branch.

---

### 📦 Mod Package Requirements

For a mod to be compatible with StellarModManager, your `.zip` file **must** maintain the following structure at its root. 

If these requirements are not met, the Mod Manager will not be able to load your mod correctly.

#### Required Folder Structure

```text
YourMod.zip
├── <mod_id>.json  <-- Metadata file (MUST match the mod's ID exactly, e.g., jolly_decorations.json)
├── Mods/          <-- Folder containing the mod's .dll files
└── Plugins/       <-- Folder containing plugin files (if you need some)

```

The metadata file contains information about your mod that StellarModManager uses to identify, load, and display it.
 
#### Metadata Format

The file must contain valid JSON using the following structure:

```json
{
  "id": "jolly_decorations",
  "name": "Jolly's Decorations",
  "author": "Jollyname",
  "version": "1.0.0",
  "description": "Adds decorative parts to the game."
}
```
