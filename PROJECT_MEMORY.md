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
- **Vista Aeronautics Fix 1.0.1 beta** (required for Vista 5.5.7 to avoid "incompatible with Vista fix 1.0.1 or below" error)


## Troubleshooting

### Vista / Vista Aeronautics Fix incompatibility
If you see an error like:
```
Mod vista is incompatible with vistafix 1.0.1 or below
Currently, vistafix is 1.0.0
```
then the Vista Aeronautics Fix version is too old.  
- Ensure you have **Vista Aeronautics Fix 1.0.1 (beta)** or newer installed.  
- Remove any older `VistaAeronauticsFix-1.0.0.jar` from the `mods` folder.  
- Download the latest version from CurseForge (search for “Vista Aeronautics Fix”, choose the NeoForge 1.21.1 file).  
- Verify that both **Vista** (version 5.5.7 or newer) and **Moonlight Lib** are present, as the fix requires them.  
- After updating, launch the pack again.

### General crash debugging
1. Check the most recent crash report in `crash-reports/` (or `logs/latest.log` if available).  
2. Look for the line that says “Mod loading failures have occurred” and note the mod name and failure message.  
3. Common fixes:  
   - Update the offending mod to a compatible version.  
   - Remove conflicting mods (e.g., two versions of the same mod).  
   - Ensure all mods are for the correct loader (NeoForge) and Minecraft version (1.21.1).  
   - Delete the `config/` folder for the problematic mod to reset to default settings (backup first).  
4. If the crash persists after removing a suspect mod, repeat the process to isolate the culprit.


## Manual Fix for Vista Aeronautics Fix

The Vista Aeronautics Fix 1.0.1 jar must be downloaded manually from CurseForge due to anti‑bot protections.

1. Open your browser and go to: https://www.curseforge.com/minecraft/mc-mods/vista-aeronautics-fix/files
2. Locate the file **VistaAeronauticsFix-1.0.1** (marked as *Beta* or *Release*).
3. Click the **Download** button. Your browser will present a Cloudflare challenge; solve it (usually just wait a few seconds).
4. After the download completes, verify the file is a genuine JAR:
   - It should be about **5–6 KB** in size.
   - Opening it with a text editor should *not* show HTML like `<!DOCTYPE html>`.
5. Move the downloaded jar into the modpack’s `mods` folder:
   `C:\Users\this4\curseforge\minecraft\Instances\CreateAeronautics\mods\`
   (replace any existing `VistaAeronauticsFix-1.0.0.jar` or `VistaAeronauticsFix-1.0.1.jar`).
6. Launch the pack via the CurseForge client.

If you still see the "zip END header not found" error, repeat the download and ensure the file is not an HTML error page.

## Create Deep Seas Configuration

A template config file `create-deep-seas-common.toml` has been added to the `config/` folder. Adjust the values to tune hull strength, buoyancy, propulsion, and maintenance for a survival‑friendly experience.

**Suggested starting values (based on real‑life ship design):**
- Base hull strength: 1000 (adjust up/down for heavier/lighter vessels)
- Layer multiplier: 1.1 per additional hull plate
- Maximum layers: 3 before diminishing returns
- Base buoyancy: 8.0 per hull block
- Air chamber buoyancy: 3.0
- Propeller efficiency: 0.7, rudder effectiveness: 0.5
- Engine power scale: 0.9
- Collision damage factor: 0.25 (reduces accidental damage from minor bumps)
- Damage speed threshold: 0.25 blocks/tick
- Storm stability factor: 0.6 (reduces effective hull strength in storm)
- Lightning damage chance: 0.005
- Maintenance interval: 6000 ticks (~5 minutes) with a small iron cost.
- Maintenance cost: 2 iron ingots per check

Feel free to tweak these to match your desired level of realism and challenge.
