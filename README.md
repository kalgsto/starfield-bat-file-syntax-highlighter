# Starfield Batch File Syntax Highlighter

A lightweight Visual Studio Code extension that provides dedicated syntax highlighting for Starfield console batch files. 

In Starfield, players and modders use standard `.txt` files to execute multiple console commands at once using the `bat filename` command. This extension transforms those plain text files into properly color-coded scripts, making it much easier to read, write, and debug your custom console batches.

## Features

This extension maps Starfield's engine syntax to standard VS Code TextMate scopes, meaning it will automatically adapt to whatever color theme you are currently using in VS Code.

*   **Commands & Functions:** Highlights base commands and target variables (e.g., `player.additem`, `cgf`, `forcerefintoalias`).
*   **Hex Reference IDs:** Distinctly colors 6 to 8-character alphanumeric Form IDs/Reference IDs (e.g., `001631C5`).
*   **INI Settings:** Recognizes and highlights Bethesda's specific INI parameter prefix system (`b`, `f`, `i`, `s`, `u` followed by a capital letter, like `bEnableMessageOfTheDay`).
*   **Strings & Arguments:** Formats quoted strings and inline arguments, specifically tailored for Papyrus global function calls.
*   **Comments:** Properly greys out lines starting with a semicolon (`;`).

## Usage & Activation

**Automatic Activation:** The syntax highlighter will automatically activate for any `.txt` file located inside a folder named `Starfield` (e.g., `C:\Program Files (x86)\Steam\steamapps\common\Starfield\follower.txt`).

**Manual Activation:** If you are editing a batch file outside of your main Starfield folder, you can manually activate the syntax highlighting:
1. Open your `.txt` file in VS Code.
2. Click on **Plain Text** in the bottom right corner of the window (or press `Ctrl + K`, then `M`).
3. Select **Starfield Batch** from the dropdown menu.

## Installation

This extension is not currently hosted on the VS Code Marketplace, but you can easily install it using the packaged `.vsix` file:

1. Download the `starfield-batch-1.0.0.vsix` file from this repository (click on the file in the list above, then click the **Download raw file** button on the right).
2. Open Visual Studio Code.
3. Open the Extensions view (`Ctrl + Shift + X`).
4. Click the **...** (Views and More Actions) menu at the top right of the Extensions panel.
5. Select **Install from VSIX...** from the dropdown menu.
6. Locate and select the `.vsix` file you just downloaded.

*(Alternatively, you can press `Ctrl + Shift + P` to open the Command Palette, type "Install from VSIX", and select the file.)*

The extension will install immediately and will automatically color-code `.txt` files located inside your Starfield directory.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
