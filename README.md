# Zellij Sessionizer

A script to easily manage your Zellij sessions.

## Requirements

Before you begin, ensure you have the following tools installed:

*   [Zellij](https://zellij.dev/): A terminal workspace and multiplexer.
*   [fzf](https://github.com/junegunn/fzf): A command-line fuzzy finder.
*   [fd](https://github.com/sharkdp/fd): A simple, fast and user-friendly alternative to `find`.

## Installation

### macOS

1.  **Install the required tools using Homebrew:**

    ```bash
    brew install zellij fzf fd
    ```

2.  **Create the installation directory:**

    ```bash
    mkdir -p ~/.local/bin
    ```

3.  **Install the script:**

    Copy the `zellij-sessionizer` script to the `~/.local/bin` directory.

    ```bash
    cp zellij-sessionizer ~/.local/bin/zellij-sessionizer
    ```

4.  **Make the script executable:**

    ```bash
    chmod +x ~/.local/bin/zellij-sessionizer
    ```

5.  **Ensure the script is in your PATH:**

    Add the following line to your shell's configuration file (e.g., `~/.zshrc`, `~/.bash_profile`):

    ```bash
    export PATH="$HOME/.local/bin:$PATH"
    ```

    Then, reload your shell's configuration:

    ```bash
    source ~/.zshrc # or source ~/.bash_profile
    ```

## Usage

To use the Zellij Sessionizer, run the following command in your terminal:

```bash
zellij-sessionizer
```

This will open a fuzzy finder interface (fzf) that allows you to select a session to attach to or create a new one.
