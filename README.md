# pretty.py

[![GitHub license](https://img.shields.io/github/license/YarikTH/pretty.py?color=blue)](https://raw.githubusercontent.com/YarikTH/pretty.py/master/LICENSE)
[![GitHub Releases](https://img.shields.io/github/release/YarikTH/pretty.py.svg)](https://github.com/YarikTH/pretty.py/releases)
[![download](https://img.shields.io/badge/download%20%20-link-blue.svg)](https://raw.githubusercontent.com/YarikTH/pretty.py/master/pretty.py)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](.)

Python script to enforce formatting rules of C++ and CMake.

Uses clang-format for C++ files and [Gersemi](https://github.com/blankspruce/gersemi) for CMake files.

Optionally allows to find project files that require prettifying using [GitPython](https://github.com/gitpython-developers/GitPython).

This script is mostly intended for personal usage for my projects. But feel free to use it too and give a feedback.

## Usage

Just download script using link above and use it. There are no plans to use proper python solutions like pip module etc.

```console
usage: pretty.py [-h] [-c] [--exclude [EXCLUDE [EXCLUDE ...]]]
                 [--clang-format CLANG_FORMAT] [--gersemi GERSEMI]
                 [src [src ...]]

A formatter to make your C++ and CMake code the real treasure.

positional arguments:
  src                   Files to format. Special value "-" to automatically
                        detect project files

optional arguments:
  -h, --help            show this help message and exit
  -c, --check           Check if files require reformatting. Return 0 when
                        there's nothing to reformat, return 1 when some files
                        would be reformatted
  --exclude [EXCLUDE [EXCLUDE ...]]
                        Files and directories to exclude from formatting
  --clang-format CLANG_FORMAT
                        Clang format to use for C++ files
  --gersemi GERSEMI     Gersemi to use for CMake files
```
