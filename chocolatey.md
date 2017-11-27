# Chocolatey

## Installing

### Using Powershell

From : https://chocolatey.org/install

1. Run `Get-ExecutionPolicy`. If it Returns "Restricted", Then Run "Set-ExecutionPolicy Bypass -Scope Process."
2. Run `Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

## Installing packages

Install packages with `choco install <package-name>`

ex. `choco install git`

List of packages available at https://chocolatey.org/packages

    