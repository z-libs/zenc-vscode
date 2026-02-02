# Zen C VSCode Extension

## Running Locally

1.  **Prerequisites**: Ensure you have [Node.js](https://nodejs.org/) and `npm` installed.
2.  **Setup**:
    ```bash
    cd editors/vscode
    npm install
    ```
3.  **Run**:
    -   Open the `editors/vscode` folder in VSCode (`code .`).
    -   Press **F5** to start debugging.
    -   This will open a new "Extension Development Host" window with the extension active.

## Configuration

-   `zenc.serverPath`: Path to your `zc` compiler.
    -   By default, it assumes `zc` is in your `PATH`.
        - If you are running from the source build, set this to the absolute path of your `zc` binary (e.g., `/home/zuhaitz/Documents/Code/Zen-C/zc`).

## Publishing

To publish to the VS Code Marketplace:

1.  **Install vsce**: `npm install -g vsce`
2.  **Create Publisher**: Go to [marketplace.visualstudio.com](https://marketplace.visualstudio.com/) and create a publisher ID.
3.  **Login**: `vsce login <publisher id>`
4.  **Package**: `vsce package` (creates a `.vsix` file for manual install)
5.  **Publish**: `vsce publish`
