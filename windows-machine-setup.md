## Windows Machine Setup for Development

Following are some guidelines for setting up a Windows machine for development. You can learn more about individual software listed below by visiting their respective websites.

- Be familiar with using **Windows command prompt**. Most of these software adds their executable paths to the system PATH environment, so you can run them from the command prompt. A point to keep in mind that after installing a software, you will need to restart the running command prompts to make the software's executable available in the command prompt. For the command prompts within VS Code (see below), you will need to restart VS Code along with the command prompt from where you launched it.

- Install [**VS Code**](https://code.visualstudio.com/). You also need to install the extensions for the programming languages (for example, Python, Java) you are going to work with. By default, dark theme is enabled within VS Code. You can change it to light theme from VS Code settings.

  If you have a directory containing source code, it's recommended that you launch VS Code from inside the directory by running the following command in the Windows command prompt:
  ```shell
  cd path/to/source/code
  code .
  ```
  If you launch VS Code in the aforementioned manner, it will open the directory in the file explorer on the left side of the window. Also, you can start a command prompt within VS Code from the menu `Terminal -> New Terminal`. The command prompt will have the current directory set to the directory containing the source code. By default, the command prompt is set to Windows powershell, you should change it to Windows command prompt from VS Code settings.

  If you are starting a new project, the recommended way is to create a new directory for the project and then launch VS Code from inside that directory.
  ```shell
  cd path/to/projects
  mkdir new-project-name
  cd new-project-name
  code .
  ```
  VS Code will remember the recently opened directories, so you can quickly re-open the project directory from the File menu after launching VS Code from Start menu after opening the project directory for the first time.

- Install [**Git**](https://git-scm.com/). Install it with the default settings. The git commands will be available in the Windows command prompt. You should set up your name and email address in git by running the following commands:
  ```shell
  git config --global user.name "Your Name"
  git config --global user.email "Your Email"
  ```
  `gitk` is nice GUI tool for viewing the git history and file changes. You can run it from the command prompt.

  Later on, you should install a GUI tool like [KDiff3](https://kdiff3.sourceforge.net/) to fix merge conflicts in git. You'll need to configure git to use KDiff3 as the merge tool.

- Install [**7-Zip**](https://www.7-zip.org/). You'll need this to extract the compressed files downloaded from internet with various extensions like .zip, .tar.gz, .rar, etc.

- Install [**Everything**](https://www.voidtools.com/). This is a global file search tool that's much faster than the default Windows search.

- Install [**Cygwin**](https://cygwin.com/). With Cygwin, you'll be able to run Linux commands like `ls`, `grep`, `find`, etc. in the Windows command prompt. Note that, you need to manually add the Cygwin's bin directory (`C:\cygwin64\bin`) to the system PATH environment to make the Cygwin commands available in the Windows command prompt.

- Install the latest version of **Ubuntu** from Microsoft store. This is a Windows Subsystem for Linux (WSL) distribution. It's recommended to install it before installing Docker Desktop. You'll need to set up a username and password for the Ubuntu distribution after installing it.

- Install [**Docker Desktop**](https://www.docker.com/products/docker-desktop). Before installing, please read about how to set up [Docker Desktop with WSL 2 backend](https://docs.docker.com/desktop/features/wsl/).

- Install **Sysinternals Suite** from Microsoft Store. This is a collection of system utilities for Windows. You can use these utilities to monitor the system performance, manage processes, etc. Couple of useful utilities are Process Explorer (a replacement for the default Windows Task Manager) and Process Monitor (a tool for monitoring file system, registry, and process/thread activity for any process).

- Install programming languages like **Python**, **Java**, etc. You can install them from their respective websites.

- Be familiar with Windows package managers like [**winget**](https://learn.microsoft.com/en-us/windows/package-manager/winget/) or [**scoop**](https://scoop.sh/) and install them when required. Some Windows software doesn't come with an installer, and you have to manually download and extract them and set up the system PATH environment. If those software are available in the package manager, you can install them with a single command. For example, Maven for Java is available in scoop.

- Recommended approach for storing **notes**: You can create a "Notes" directory at a cloud backup path (like OneDrive, Google Drive etc.) and store your notes in markdown format. You can open the "Notes" directory in VS Code and edit the notes from there. As your notes are stored within a cloud backup path, they will be automatically backed up to cloud and you can access them from any device. Later, you can use [Obsidian](https://obsidian.md/) + [Syncthing](https://syncthing.net/), if you want to have a better viewing/editing experience from mobile devices. Obsidian stores notes in markdown format within a directory, so you'll just need to point Obsidian to the "Notes" directory.

- Be familiar with the **split-screen** feature in Windows. To use the split screen feature in Windows, you can press the `Windows` key and the `left arrow` or `right arrow` key to snap a window to one side of the screen. Then, select another window to fill the other half of the screen. This feature is useful when you are following a tutorial in a browser and writing code in VS Code. You can snap the browser window to one side of the screen and VS Code to the other side.

- Be familiar with some [**keyboard shortcuts**](https://support.microsoft.com/en-us/windows/keyboard-shortcuts-in-windows-dcc61a57-8ff0-cffe-9796-cb9706c75eec) in Windows.
