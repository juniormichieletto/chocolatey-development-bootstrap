
# chocolatey-development-bootstrap

The common chocolatey packages that I usually need when I`m working in the Windows workspaces

Using Chocolatey package manager to install some apps

1. Install chocolatey package manager using powershell in administrative mode

```bash
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

2.Move chocolatey installation folder to you D:\<...your_tools_folder>

3.Change the chocolatey environment variable "ChocolateyInstall" pointing to new folder (the one that you moved in step 2)

4.Change the chocolatey "folder" in "path" environment variable, a sugestion is remove the old one and add a new value with %ChocolateyInstall%\bin

5.Reopen the powershell in administrative mode and Install apps that you want

```bash
    choco install git
    choco install openjdk11
    choco install openjdk8
    choco install maven
    choco install jetbrainstoolbox
    choco install ant
    choco install microsoft-windows-terminal

    choco install nodejs-lts
    choco install vscode
    choco install dbeaver

    choco install ditto
    choco install curl
    choco install notepadplusplus
    choco install sharex
    choco install googlechrome
    choco install firefox
    choco install 1clipboard
    choco install microsoft-teams
```
