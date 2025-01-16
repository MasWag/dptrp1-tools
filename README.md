dptrp1-tools
============

[![ShellCheck](https://github.com/MasWag/dptrp1-tools/actions/workflows/shellcheck.yml/badge.svg)](https://github.com/MasWag/dptrp1-tools/actions/workflows/shellcheck.yml)

A collection of utility scripts for managing PDF files on Sony DPT-RP1 digital paper devices. Notice that the scripts are dedicated for my personal use.

Overview
--------

This repository contains scripts to help manage PDF files on Sony DPT-RP1 devices.

Requirements
------------
The scripts require the following tools to be installed:

- [bash](https://www.gnu.org/software/bash/) - The shell environment
- [dptrp1](https://github.com/janten/dpt-rp1-py) - Python utility for interacting with Sony DPT-RP1 devices
- [peco](https://github.com/peco/peco) - Interactive filtering tool

Scripts
-------

### download_thesis

Downloads thesis PDFs from the DPT-RP1 device.

**Usage:**
```bash
download_thesis [DIR]
```
- `DIR` (optional): Target directory for downloaded files. Defaults to `/tmp/`

The script will:
1. List all documents on the device
2. Filter for thesis documents from 2024 academic year
3. Show an interactive selection interface
4. Download the selected document to the specified directory

### mark_done_thesis

Marks selected thesis documents as completed by moving them to a "Done" folder.

**Usage:**
```bash
mark_done_thesis
```

The script will:
1. List all documents on the device
2. Filter for thesis documents from 2024 academic year
3. Show an interactive selection interface
4. Move selected documents to a "Done" subfolder

Author
------

Masaki Waga

License
-------

MIT License

