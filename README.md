# kilocode-rules

This repository, `kilocode-rules`, holds rule files and system prompts for the Kilo Code VS Code extension. These files customize Kilo Code's AI behavior for your projects, improving its code generation, analysis, and debugging.

## What is Kilo Code?

Kilo Code is an open-source AI coding agent within VS Code, designed to automate and streamline various programming tasks. For more details, visit: [https://kilocode.ai/](https://kilocode.ai/).

---

## How to Use These Rules

To use these rules, rename the `kilocode-rules` directory to `.kilocode` and place it in your project's root. Kilo Code automatically detects files in a hidden `.kilocode` directory.

### Quick Setup (Terminal Only):

Follow these steps in your terminal:

1.  **Navigate into your project and clone the repo:**
    ```bash
    # Navigate to your project's main directory
    cd your-project-root

    # Clone the repo
    git clone https://github.com/shanefully-done/kilocode-rules.git
    ```

2.  **Rename the directory:**
    ```bash
    # Ensure you are executing this command from your main project directory (`your-project-root`).
    mv kilocode-rules .kilocode
    ```

Once `.kilocode` is in your project's root, Kilo Code will automatically start using these rules.
