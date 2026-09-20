# Pras2005 - Personal Portfolio

A sleek, interactive personal portfolio website showcasing projects, skills, and experience through a unique Terminal User Interface (TUI) implemented entirely in frontend web technologies.

## Overview
This repository contains a single-page portfolio (`index.html`) for GitHub user `Pras2005`. It leverages vanilla HTML, CSS, and JavaScript to create a retro, keyboard-navigable terminal aesthetic over a modern web page. 

## Deep Dive Description
The core logic resides within the embedded `<script>` tag in `index.html`. 
- **Data Model**: Information about projects, experience, and skills is stored in a structured JavaScript dictionary named `TUI_DATA`. Keys correspond to data IDs (e.g., `speakql`, `lvm`, `krishi`) and contain `title`, `subtitle`, and `body` fields (rendered as HTML).
- **TUI State Management**: 
  - `tuiOpen`: Tracks if the overlay is active.
  - `activePaneIdx`: Tracks which of the 4 panes is currently focused.
- **Keyboard Navigation Engine**: Event listeners capture standard terminal/Vim keybindings (e.g., `j`/`ArrowDown`, `k`/`ArrowUp`, `q`, `Tab`, `1-4`) to traverse panes, select items, and dynamically render content into the `#tui-main-content` DOM element.

## Prerequisites
- Any modern web browser (Chrome, Firefox, Safari, Edge)

## Installation & Setup
No complex build steps or dependencies are required as this is a static vanilla web project.

1. **Clone the repository**:
   ```bash
   git clone git@github.com:Pras2005/Pras2005.git
   cd Pras2005
   ```

## Usage / Running Locally
Simply open the `index.html` file in your preferred web browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html
```
Once opened, click the "TUI" button or use the mapped keys to interact with the terminal overlay.

## Project Structure
```text
Pras2005
├── index.html        # The entire application (HTML layout, CSS styling, JS logic)
└── README.md         # Documentation
```
