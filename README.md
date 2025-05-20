# MXAG7 - AI-Powered Command Line Assistant

MXAG7 is an AI-powered command-line tool that helps Ubuntu system administrators execute commands with AI guidance and analysis. This version of MXAG7 uses **Ollama**, an open-source LLM, instead of the OpenAI API, allowing you to run the AI locally without requiring an API key.

## Features

- **AI-Powered Command Analysis**: Analyzes commands before execution to explain what they do.
- **Risk Assessment**: Highlights potential risks of commands before execution.
- **Dependency Detection**: Identifies required packages and dependencies.
- **Secure Execution**: Confirms with you before running potentially destructive commands.
- **Offline AI Integration**: Uses Ollama's local models, eliminating the need for an internet connection or external API keys.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/mxag7-ollama.git
   cd mxag7-ollama
   ```

2. **Install Ollama**:
   Follow the instructions to install Ollama on your system from the [Ollama Quickstart Guide](https://ollama.readthedocs.io/en/quickstart/).

   Example (for macOS):
   ```bash
   brew install ollama
   ```

3. **Run the Installation Script**:
   ```bash
   sudo bash install.sh
   ```

4. **Set Up the AI Agent**:
   Since Ollama does not require an API key, setup is simple:
   ```bash
   sudo mxag7 setup
   ```

## Usage

To use MXAG7, simply prefix your commands with `sudo mxag7`:

```bash
# Example: Install Postal mail server
sudo mxag7 install postal

# Example: Update system packages
sudo mxag7 apt update && apt upgrade -y
```

## Requirements

- **Operating System**: Ubuntu Linux (tested on Ubuntu 20.04+)
- **Python Version**: Python 3.8 or newer
- **AI Backend**: Ollama (installed locally)
- **Root Access**: Required for installation and execution.

## Uninstallation

To remove MXAG7 from your system, run the uninstallation script:
```bash
sudo bash uninstall.sh
```

## License

MIT License
