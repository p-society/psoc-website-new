---
title: "Getting Online"
date: 2022-03-27T17:41:25+05:30
draft: false
---

## Prerequisites

### A [Github account](https://github.com/signup)

### [Hugo](https://gohugo.io/getting-started/installing/)

> If you don't understand what's happening below, just skip over to "BUILDING FROM SOURCE". Or simply drop us a message on [discord](https://discord.gg/wtuq9bVA)

#### Windows

If you have [Chocolatey](https://chocolatey.org/) installed, run
`choco install hugo -confirm`

Or if you have [Scoop](https://scoop.sh/), run
`scoop install hugo`

#### Linux

If you have [HomeBrew](https://brew.sh/) installed, run
`brew install hugo`

(Or simply use your package manager)

#### MacOS

If you have [MacPorts](https://www.macports.org/), run
`port install hugo`

or If you have [HomeBrew](https://brew.sh/) installed, run
`brew install hugo`

#### Building from Source

- Download and install GoLang [(Windows)](https://go.dev/dl/go1.18.windows-amd64.msi)
- Download and install Git [(Windows)](https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe)
- Open a command prompt and run these commands:
  - `mkdir %USERPROFILE%/src`
  - `cd %USERPROFILE%/src`
  - `git clone https://github.com/gohugoio/hugo.git`
  - `cd hugo`
  - `go install`

### Any Code Editor (other than notepad :p)

Recommended ones are VS Code and Sublime Text.
