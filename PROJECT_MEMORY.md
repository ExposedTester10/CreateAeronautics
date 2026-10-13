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

## Prepared Mods Folder
A `mods/` directory has been created at:
`/opt/data/home/Documents/Obsidian Vault/Gavin/projects/CreateAeronautics/mods`
Due to anti-bot protections on CurseForge/Modrinth, automated download of mod JARs is not reliably possible. Please use the CurseForge client (or website) to search for and install the following mods into this instance.

## Recommended Mods to Install
### Core
- **Create** (core mod)
- **Create: Aeronautics** (flight addon)

### Performance & Optimizations (NeoForge 1.21.1)
- **FerriteCore** – memory usage optimizations
- **EntityCulling** – client-side entity culling for FPS
- **ModernFix** – combined fixes for performance and stability
- **LazyDFU** – client-side lazy data fixer upper
- **Clump** – improves entity ticking performance
- **AI Improvements** – optimizes AI tick loops
- **Sodium** (if using Fabric; for NeoForge consider **Phosphor** alternative) – note: Sodium is Fabric-only; for NeoForge, look for **Lithium** (Forge) or **EntityCulling** + **ModernFix** combo.
- **Lithium** (Forge) – server/client performance improvements
- **BetterFPS – Fork** (optional, if compatible)
- **Toast Control** – suppress unnecessary toasts
- **FancyBlockParticles** – reduce particle load
- **Mod Menu** – easy in‑game mod configuration
- **Just Enough Items (JEI)** – recipe viewing (essential for Create)
- **KubeJS** – for custom scripts, recipes, and tweaks (place scripts in `kubejs/`)

### Quality of Life & Survival Foundations (examples)
- **Farmer's Delight** – cooking and farming enhancements
- **Lanterns** – decorative lighting
- **Create: Deco** – decorative blocks for Create
- **Create: Stuff & Additions** – additional Create mechanisms
- **Charm** – pleasant UI enhancements
- **AppleSkin** – food/hunger info
- **JourneyMap** or **Xaero's Minimap** – mapping (optional)
- **Controlling** – manage keybind conflicts

### Configuration Tips
- After installing mods, launch the pack once via CurseForge to generate default config files.
- Edit configs under `config/` to tune Create mechanics (e.g., gear ratios, processing speeds) for survival balance.
- For KubeJS, place custom scripts in `kubejs/server_scripts/` and `kubejs/client_scripts/` as needed.
- Review mod compatibility; some performance mods may conflict (e.g., Sodium + Lithium not needed together).

## Next Steps
1. Use the CurseForge client to add the mods listed above to this instance.
2. Launch the pack to verify startup and check for errors.
3. Update `minecraftinstance.json` if needed (CurseForge client will manage this).
4. Create configuration folders and tweak settings.
5. Develop KubeJS scripts for custom Create recipes and automation.
6. Playtest survival progression and flight mechanics.
7. Document any custom changes in README.md and maintain a changelog.

## Notes
- Review mod licenses before redistributing any packaged modpack.
- Keep logs organized; consider adding a log‑review script or guide for common issues.
- Use `.gitignore` to exclude large or transient files (e.g., `logs/`, `saves/`, `modrinth.index.json` if applicable) while preserving essential configs.