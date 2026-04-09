# notispf port for z/OS Open Tools

This repository contains the zopen port definition for [notispf](https://github.com/mrthock/notispf), a terminal text editor inspired by the ISPF editor from z/OS mainframes.

## About notispf

notispf brings the ISPF prefix command workflow to Unix System Services (USS) terminal sessions. If you know ISPF, you already know notispf — prefix commands like `D`, `DD`, `C`, `M`, `>>`, and the command line work the same way.

## Prerequisites

- z/OS Unix System Services
- zopen package manager
- Python 3.12 (`python_312` zopen package)

## Installation

```sh
zopen install notispf
```

## Usage

```sh
notispf myfile.txt
```

## Notes on EBCDIC

notispf edits files as-is in USS. For native z/OS datasets, use the DSFS feature to mount them into the USS filesystem before editing. This is the same behavior as other USS text editors (nano, vim, etc.).

## Links

- [notispf source](https://github.com/mrthock/notispf)
- [zopen community](https://github.com/zopencommunity)
