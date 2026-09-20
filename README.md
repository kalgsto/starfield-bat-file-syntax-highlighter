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

## Installation (Manual Install)

This extension is not hosted on the VS Code Marketplace, so you will need to install it manually:

1. At the top of this repository page, click the green **Code** button and select **Download ZIP**.
2. Extract the downloaded ZIP file.
3. **Important:** Rename the extracted folder to exactly FearTheReaper.starfield-batch-1.0.0
4. Move that renamed folder into your local VS Code extensions directory:
   * **Windows:** `%USERPROFILE%\.vscode\extensions` (e.g., `C:\Users\YourUsername\.vscode\extensions`)
   * **macOS/Linux:** `~/.vscode/extensions`
5. Completely close and restart Visual Studio Code. 

The extension will now be active and will automatically color-code `.txt` files located inside your Starfield directory.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
