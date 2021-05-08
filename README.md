# Code Sandbox Shell Script

Create a local JavaScript code sandbox. No folder structure, no packages, no fluff, intended for times when you just want to try something out quick-and-dirty. This script will repeatedly save you approximately 48 seconds of your life that you would otherwise never get back.

## Features

- Create _index.html_, _style.css_, and _index.js_ files
- Add a few very basic CSS reset rules
- Automatically open the sandbox as a workspace in VS Code

## Installation

Download the [latest release](https://github.com/kgrhartlage/code-sandbox-script/releases/download/v0.0.1/sandbox) and move the script file to a directory included in your `PATH` environment variable. Conventional paths for user scripts are `/usr/local/bin` or `/opt/bin`. Then make the script executable:

```bash
 $ chmod +x sandbox
```

## Usage

Execute the script using the `sandbox` command. The sandbox will always be created at `$HOME/Desktop`, regardless of your current working directory.

### Options

If no additional argument is provided to the `sandbox` command, the current date will be attached to the folder name:

```bash
$ sandbox
# => sandbox-YYYY-MM-DD
```

The date can be replaced by providing an argument to the `sandbox` command:

```bash
$ sandbox custom-name
# => sandbox-custom-name
```

## License

Released under the terms of the [MIT License](https://opensource.org/licenses/MIT).
