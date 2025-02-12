# Intro
Contains scripts and configs to setup my powershell environment including the custom prompt.

## Powershell
For much of this work you'll need powershell 7.2+ (Also known as Powershell Core).  Releases and instructions to install can be found here:  [Powershell Core](https://github.com/PowerShell/PowerShell)

## Windows Terminal
Windows terminal is my preferred terminal program and can host different types of CLI out of the box (Poweshell, CMD, and others) in a tabbed interface.

Installation instructions and details can be found here: [Windows Terminal](https://github.com/microsoft/terminal)


## Prompt
I use [oh-my-posh](https://ohmyposh.dev) for my custom prompt.  Check out this great repository for a ton of different configurations and features.  You can find my current config in [oh-my-config.json](prompt/oh-my-config.json).

To make it look properly, you will need to download and install a Nerd Font that contains the icons used in oh-my-posh.  Follow the instructions here:  [oh-my-posh Nerd Fonts](https://ohmyposh.dev/docs/config-fonts)

## Setup
Edit your profile script, which by using the following in your powershell terminal:

First you'll need to install a few powershell modules:

```console
install-module -Name PSReadLine 
install-module -Name oh-my-posh
install-module -Name terminal-icons
install-module -Name z
```
these 4 installs should give you everything needed

```console
$profile
```
This will provide the file/path to your profile.  

Add the following line in your startup profile (changing the appropriate paths of course)

```console
. C:\apps\powershell\ps-profile.ps1
```


