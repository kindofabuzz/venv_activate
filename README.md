# venv_activate

A simple Bash script that automatically detects and activates Python virtual environments in your current working directory.

## Features

- 🔍 **Auto-detection**: Automatically finds `.venv` or `venv` directories
- 🎨 **Colored output**: Provides clear, colored terminal feedback
- 🚀 **New shell**: Launches a fresh Bash shell with the virtual environment activated
- ❌ **Error handling**: Graceful error messages for missing environments
- 👋 **User-friendly**: Personalized greeting messages

## Usage

Simply run the script in any directory containing a Python virtual environment:

```bash
./venv_activate
```

The script will:
1. Look for `.venv` or `venv` directories in the current location
2. Activate the found virtual environment
3. Launch a new Bash shell with the environment active
4. Display a friendly welcome message

## Supported Virtual Environment Structures

- `.venv/` (hidden directory, commonly used)
- `venv/` (visible directory, also common)

## Requirements

- Bash shell
- Python virtual environment with standard structure (`bin/activate` file)

## License

This project is released under the CC0 1.0 Universal license - see the [LICENSE](LICENSE) file for details. This means it's in the public domain and you can use it freely for any purpose.