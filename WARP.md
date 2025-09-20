# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Commands

### Building and Development

| Command | Description |
| :--- | :--- |
| `npm run build` | Compiles the TypeScript source code and makes the package ready for use. |
| `npm run watch` | Watches for changes in the TypeScript source and automatically recompiles. |

## Code Architecture

This project is a Model Context Protocol (MCP) server that provides browser automation capabilities using BrowserCat's cloud browser service.

### Key Components

*   **Tools**: The server exposes a set of tools that allow LLMs to interact with web pages. These tools include:
    *   `browsercat_navigate`: Navigates to a URL.
    *   `browsercat_screenshot`: Captures screenshots.
    *   `browsercat_click`: Clicks elements.
    *   `browsercat_hover`: Hovers over elements.
    *   `browsercat_fill`: Fills input fields.
    *   `browsercat_select`: Selects dropdown options.
    *   `browsercat_evaluate`: Executes JavaScript.
*   **Resources**: The server provides access to two resources:
    *   `console://logs`: Provides browser console output.
    *   `screenshot://<name>`: Provides access to captured screenshots.

### Dependencies

*   `@modelcontextprotocol/sdk`: The core dependency for implementing the MCP server.
*   `puppeteer`: Used for browser automation.

For more detailed information, please refer to the `README.md` file.
