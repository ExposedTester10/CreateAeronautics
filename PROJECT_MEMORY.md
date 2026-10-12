# Project Memory: CreateAeronautics

## Goal
Create a survival-friendly Minecraft modpack centered around the **Create** mod and its addon **Create: Aeronautics**. The modpack emphasizes flight, machinery, and automation while maintaining balanced survival gameplay. It uses NeoForge as the base mod loader (version 21.1.259) targeting Minecraft 1.21.1.

## Important Context
- This GitHub repository resides in a parent folder on your personal computer that is attached to a **CurseForge client**.
- Running the modpack via CurseForge generates numerous log files for troubleshooting; these logs appear in various formats (JSON, config files, KubeJS scripts, etc.).
- The repository is intended to be synced with the CurseForge instance, allowing version-controlled updates to the modpack.

## My Role
I am here to:
- Help brainstorm and refine modpack ideas.
- Download and integrate mods (especially Create and its addons).
- Edit configuration files (JSON, TOML, YAML, properties, KubeJS).
- Assist with troubleshooting by analyzing logs and suggesting fixes.
- Provide guidance on mod compatibility, performance tuning, and gameplay balance.

## Current State
- Repository cloned from https://github.com/ExposedTester10/CreateAeronautics.git
- Contains a base `minecraftinstance.json` defining the mod loader and initial mod list.
- Includes `options.txt` for client settings.
- Licensed under MIT (see LICENSE).
- README placeholder.

## Next Steps
1. **Core Mods**: Ensure Create and Create: Aeronautics are present and up-to-date in `minecraftinstance.json`.
2. **Survival Foundations**: Add complementary mods for resources, exploration, and quality-of-life (e.g., Farmer's Delight, Lanterns, etc.) while preserving balance.
3. **Configuration**: 
   - Create a `config/` directory for mod-specific configs.
   - Tune Create mechanics (e.g., gear ratios, item processing) for survival.
   - Set up KubeJS scripts (`kubejs/` folder) for custom recipes, tweaks, and event handling.
4. **Testing**: 
   - Launch the pack via CurseForge to verify startup and log output.
   - Playtest survival progression and flight mechanics.
5. **Documentation**: 
   - Update README.md with installation, launch instructions, and modpack overview.
   - Maintain a changelog in the repository.
6. **Maintenance**: 
   - Regularly update mods and resolve conflicts.
   - Commit changes with descriptive messages.
   - Back up configs before major updates.

## Notes
- Review mod licenses before redistributing any packaged modpack.
- Keep logs organized; consider adding a log‑review script or guide for common issues.
- Use `.gitignore` to exclude large or transient files (e.g., `logs/`, `saves/`, `modrinth.index.json` if applicable) while preserving essential configs.