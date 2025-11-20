# Linux Buddy - Interactive Linux Command Tutorial with Hands-On Labs

![demo](https://github.com/user-attachments/assets/de714149-4e8d-4011-b94f-a2b20042b63e)

Master Linux commands through interactive terminal lessons with auto-generated practice labs. Featuring 100+ commands with ethical hacking context, instant terminal spawning, zero dependencies, and beginner-friendly explanations.

[![Python](https://img.shields.io/badge/python-3.13+-yellow.svg)](https://www.python.org/downloads/)
[![License: GPL-3.0](https://img.shields.io/badge/License-GPL%203.0-red.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
[![PyPI](https://img.shields.io/badge/pip-install%20linux--buddy-brightgreen)](https://pypi.org/project/linux-buddy/)
[![GitHub](https://img.shields.io/github/stars/jo4dan/linux-buddy?style=social)](https://github.com/jo4dan/linux-buddy)

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Architecture](#project-architecture)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Features

- ✨ **100+ Command Lessons** - Covers file operations, networking, text processing, system admin, and security tools
- 🎯 **Auto-Generated Labs** - Creates practice environments with dummy files for safe experimentation
- ⚡ **New Terminal Tabs** - Launches lessons in separate gnome-terminal tabs with formatted content
- 📚 **Ethical Hacking Context** - Every command includes cybersecurity significance and real-world use cases
- 🔒 **Zero Dependencies** - Uses only Python standard library (os, sys, shutil, subprocess, textwrap, math)
- 🎨 **4-Column Menu** - Clean paginated interface displaying 100 commands per page
- 🏗️ **Modular Architecture** - Professional SOLID-principle codebase with src/data, src/core, src/ui structure
- 🔧 **Beginner-Friendly** - Clear explanations, usage examples, and step-by-step practice instructions

## Installation

### Quick Install (Recommended)

Install directly from PyPI using pip:

```bash
pip install linux-buddy
linux-buddy
```

### Install


```bash
git clone https://github.com/jo4dan/linux-buddy.git
cd linux-buddy
python main.py
```

### Prerequisites

- Python 3.6 or higher
- Linux/Unix system (tested on Ubuntu, Debian, Fedora, Arch)
- gnome-terminal (recommended; fallback to bash if unavailable)
- No external dependencies required

## Usage

### Run the Tool

```bash
python main.py
```


### Navigation

- **Enter number** - Launch lesson for that command
- **n** - Next page
- **p** - Previous page
- **q** - Quit
- **Ctrl+C** - Exit anytime

### Workflow

1. Browse 100+ commands in the paginated menu
2. Select a command by entering its number
3. New terminal tab opens with lesson content
4. Practice in auto-generated lab directory
5. Type `exit` to close tab and return to menu
6. Continue learning or quit with `q`


## Project Architecture

```bash
linux-buddy/
├── main.py # Entry point
├── README.md
├── LICENSE
├── requirements.txt # Empty (no dependencies)
├── src/
│ ├── data/
│ │ └── lessons.py # Command data & lessons
│ ├── core/
│ │ ├── lab_manager.py # Lab environment setup
│ │ └── terminal.py # Terminal spawning
│ ├── ui/
│ │ ├── menu.py # Menu display
│ │ └── formatting.py # Text formatting
│ └── utils/
│ └── helpers.py # Utility functions
├── tests/
│ ├── test_lessons.py
│ └── test_lab_manager.py
└── labs/ # Runtime directories
```


## Troubleshooting

**gnome-terminal not found**: Install via `sudo apt install gnome-terminal` or use fallback bash mode

**Permission denied**: Check /tmp permissions or modify lab_dir to ./labs/ in terminal.py

**Python version error**: Verify Python 3.6+ with `python --version`

**Menu display issues**: Increase terminal width (minimum 80 characters) or open the tool in full screen

**Lab files not created**: Check write permissions in lab directory

File issues at [GitHub Issues](https://github.com/jo4dan/linux-buddy/issues)

## Contributing

Fork, branch, and PR! Contributions welcome for:

- New command lessons
- Bug fixes
- Documentation improvements
- Terminal emulator support
- Unit tests

```bash
git checkout -b feature/NewCommand
git commit -m 'Add iptables lesson'
git push origin feature/NewCommand
```


## License

GPL-3.0 License - see [LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html)

---

**Built by [@jo4dan](https://github.com/jo4dan)** | Star ⭐ if useful! | Questions: [jordannissi7@gmail.com](mailto:jordannissi7@gmail.com)

**SEO Keywords**: Linux command tutorial, ethical hacking training, interactive terminal learning, command-line practice labs, cybersecurity Linux commands, DevOps training, penetration testing reference, beginner Linux tutorial



