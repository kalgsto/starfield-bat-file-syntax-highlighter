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

By default, VS Code treats all `.txt` files as Plain Text. To prevent this extension from hijacking your normal text files, it is designed with a specific targeting rule:

**Automatic Activation:** The syntax highlighter will automatically activate for any `.txt` file located inside a folder named `Starfield` (e.g., `C:\Program Files (x86)\Steam\steamapps\common\Starfield\follower.txt`).

**Manual Activation:** If you are editing a batch file outside of your main Starfield folder, you can manually activate the syntax highlighting:
1. Open your `.txt` file in VS Code.
2. Click on **Plain Text** in the bottom right corner of the window (or press `Ctrl + K`, then `M`).
3. Select **Starfield Batch** from the dropdown menu.

## Installation (NOTE: not published yet! Will update when I publish it)

You can install this extension directly from within Visual Studio Code:
1. Open the Extensions view (`Ctrl + Shift + X`).
2. Search for **Starfield Batch Script**.
3. Click Install.

*(Alternatively, you can download it directly from the [Visual Studio Marketplace](LINK_TO_YOUR_MARKETPLACE_PAGE_HERE).)*

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
