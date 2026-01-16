# GitHub Copilot Instructions

## Repository Overview

This repository contains `venv_activate`, a Bash shell script that automatically detects and activates Python virtual environments in the current working directory.

## Key Features

- Automatically detects `.venv` or `venv` directories
- Provides colored terminal output for better user experience  
- Launches a new Bash shell with the virtual environment activated
- Includes error handling for missing virtual environments
- User-friendly messages with project name and user greeting

## Code Style Guidelines

### Bash Scripting
- Use `#!/bin/bash` shebang
- Follow consistent indentation (4 spaces)
- Use descriptive function names
- Include proper error handling with meaningful error messages
- Use ANSI color codes for terminal output formatting
- Quote variables to prevent word splitting: `"$variable"`
- Use `return` with appropriate exit codes for functions

### Error Handling
- Write error messages to stderr using `>&2`
- Use appropriate return codes:
  - `0`: Success
  - `1`: General error (no venv found)
  - `2`: Specific error (activation file not found)

### Output Formatting
- Use color variables defined at the top of the script:
  - `Color_Off='\033[0m'` for resetting colors
  - `BGreen='\033[1;32m'` for success messages
  - `BRed='\033[1;31m'` for error messages
- Include informative messages about what the script is doing
- Use consistent messaging format

## File Structure

- `venv_activate`: Main executable Bash script
- `LICENSE`: CC0 1.0 Universal license (public domain)

## Testing Considerations

When suggesting improvements or modifications:
- Consider edge cases like missing directories or permissions issues
- Ensure cross-platform compatibility where possible
- Maintain backwards compatibility with existing functionality
- Test with both `.venv` and `venv` directory structures

## Development Guidelines

- Keep the script simple and focused on its core purpose
- Maintain readability and clear function separation
- Add comments only when the code logic is not self-explanatory
- Preserve the friendly, welcoming tone in user-facing messages