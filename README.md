# [atet](https://github.com/atet) / [**_godot_**](https://github.com/atet/godot/blob/main/README.md#atet--godot)

[![.img/logo_godot.png](.img/logo_godot.png)](#nolink)

# Introduction to Godot

These are instructions to quickly set up a new Godot developement environment for C#.

Excluding time to download and install dependencies, _**you will be able to complete this tutorial in ~10 minutes**_

--------------------------------------------------------------------------------------------------

## Table of Contents

### Introduction

* [0. Preface](#0-preface)
* [1. Requirements](#1-requirements)
* [2. Installation](#2-installation)
* [3. Godot](#3-godot)
* [4. VS Code](#4-vs-code)
* [5. Next Steps](#5-next-steps)

### Supplemental

* [Other Resources](#other-resources)
* [Troubleshooting](#troubleshooting)

--------------------------------------------------------------------------------------------------

## 0. Preface

[![.img/fig1_godot_3.5.jpg](.img/fig1_godot_3.5.jpg)](#nolink)

Godot has come a long way snce I first used it back in 2018. With the recent 2023 Unity fiasco, now's a better time than any to leverage this powerful, free, and open-source game development engine.

**Features** | **Options**
--- | ---
**Game Modes** | Single-player, Multi-player (local & networked)
**Formats** | 2D, 3D, extended reality (XR)
**Platforms** | Desktop, Mobile, Web-based

Although Godot traditionally uses its built-in interpreted language GDScript, we are going to use the more familiar (especially to Unity users) and compiled C# language.

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## 1. Requirements

### Hardware

Any computer made in the past decade will run Godot; we will use Windows 10 in this tutorial.

You don't need a powerful computer to develop on Godot nor do you need too much hard drive space as Godot's development environment weights in at under 150 MB while Unity can be multiple GBs. 

### Software

We will install two programs as you will **switch back and forth** between manual drag-and-drop actions in Godot and coding in Visual Studio Code (a.k.a. VS Code) during development; **this is standard practice with other game engines like Unity as well**.

[![.img/fig7_godot_vscode.jpg](.img/fig7_godot_vscode.jpg)](#nolink)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## 2. Installation

We will install the .NET framework (for C# development) and use portable versions of the Godot and VS Code development environments. Portable means you will not have to install the programs to Windows and can just use them once downloaded.

### .NET Framework

***TODO:*** *Previously installed .NET framework for C# development through a Unity installation, will confirm installation instructions from scratch.*

### Godot

Godot with C# support is available for Windows, MacOS, and Linux in a portable format.

For Windows, you can download a portable .NET version (for C# support) here: https://godotengine.org/download/windows/

[![.img/fig2_download_godot.jpg](.img/fig2_download_godot.jpg)](#nolink)

Once the `Godot_v4.1.2-stable_mono_win64.zip` (or higher version) file is downloaded, you can uncompress and use Godot right away after some additional setup for C# compatibility detailed below.

### Visual Studio Code

VS Code is available for Windows, MacOS, and Linux in a portable format.

For Windows, you can download a portable version here: https://code.visualstudio.com/download

[![.img/fig3_download_vscode.jpg](.img/fig3_download_vscode.jpg)](#nolink)

Once the `VSCode-win32-x64-1.83.1.zip` (or higher version) file is downloaded, you can uncompress and use VS Code right away after some additional setup for C# and Godot compatibility detailed below.

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## 3. Godot

There will be a couple configurations in Godot that only needs to be enabled once and a setting that must be done **for each new project** to ensure proper C# support.

### Do This Once

1. `Editor` → `Editor Settings` → `Text Editor` → `External` → Enable `Use External Editor` → Set `Exec Path` to Code.exe for VSCode
2. `Editor` → `Editor Settings` → `Text Editor` → `Behavior` → `Files` → Enable `Auto Reload Scripts on External Change`

### Do This Once per New Project

1. `Project` → `Tools` → `C#` → Select `Create C# solution`
2. In the bottom tabs: `MSBuild` → `Build` → `Build Project` (**do not initially open C# scripts from Godot, see below**)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## 4. VS Code

Though you can use the Script Editor from within Godot with C#, it will not support Intellisense like VS Code can; *believe me when I say you're going to want that*.

There will be a configurations in VS Code that only needs to be enabled once and a specific way to open your projects if you've closed them to ensure proper C# Intellisense support.

### Do This Once

1. Install the official Microsoft C# extension:

[![.img/fig4_vscode_extension.jpg](.img/fig4_vscode_extension.jpg)](#nolink)

2. `Files` → `Preferences` → `Settings` → `Extensions` → `C#` → `Omnisharp` → Enable `Dotnet > Server: Use Omnisharp`

### Do This per VS Code Restart

**You must always initially open your Godot C# files by opening the project folder from VS Code and not from a C# script within Godot for Intellisense to work properly**

1. `File` → `Open Folder...` → Navigate to top-level folder of Godot project
2. Now you can open C# scripts from either VSCode or within Godot

Intellisense should now be fully enabled in VS Code:

[![.img/fig5_vscode_intellisense.jpg](.img/fig5_vscode_intellisense.jpg)](#nolink)

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## 5. Next Steps

You are now ready to embark on your journey to become an applications developer! Whether your applications are productivity programs, teaching tools, or games for fun, you now have everything you need to get started.

[![.img/fig6_godot_applications.jpg](.img/fig6_godot_applications.jpg)](#nolink)
> Programs above from the [2022 Godot Showcase](https://godotengine.org/showcase/)

**TODO**: Add pitch and link to my next Godot tutorial

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## Other Resources

**Description** | **URL Link**
--- | ---
Intro to Intellisense | https://code.visualstudio.com/docs/editor/intellisense

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

## Troubleshooting

Issue | Solution
--- | ---
**"Intellisense is not working!"** | You must follow the configuration, setup, and instructions to open projects above for Intellisense to work in VS Code
**"It's not working!"** | This concise tutorial has distilled hours of sweat, tears, and troubleshooting; _it can't not work_

[Back to Top](#table-of-contents)

--------------------------------------------------------------------------------------------------

<p align="center">Copyright © 2023-∞ Athit Kao, <a href="http://www.athitkao.com/tos.html" target="_blank">Terms and Conditions</a></p>