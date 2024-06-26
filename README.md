## Mozilla Linux Installer
[![Mozilla Badge](https://img.shields.io/badge/Mozilla-black?logo=mozilla&labelColor=black)](https://mozilla.org/)
[![Firefox Badge](https://img.shields.io/badge/Firefox-FF7139?logo=firefoxbrowser&labelColor=white)](https://mozilla.org/firefox/)
[![Firefox Dev Badge](https://img.shields.io/badge/Firefox_Dev-008DEA?logo=firefoxbrowser&logoColor=008DEA&labelColor=white)](https://mozilla.org/firefox/developer/)
[![Thunderbird Badge](https://img.shields.io/badge/Thunderbird-0A84FF?logo=thunderbird&labelColor=white)](https://thunderbird.net/)

This script was created to more easily install the Firefox Developer Edition tarball from the Mozilla website, but was expanded to encompass any Firefox version, along with Thunderbird.

By default, the instructions below will cause the programs to be installed for your user (recommended), although the script also supports installation as root.

### Executable Binaries

There are a few reasons as to why install the executable binaries from the official websites, as opposed to installing from your distribution repository:
- There are more versions of Firefox in the official website;
- Each executable binary is self-updating, keeping up with security;
- Each executable binary can be run directly from your user directory;
- Each executable binary can utilize the full security sandboxing from the project, which is more restrictive than their flatpak counterparts.

### How to install:

1. Extract the Firefox and / or Thunderbird tarballs downloaded from the respective official websites;
2. If the Firefox version is an alternate one (Developer Edition / Nightly), rename the extracted folder from "firefox" to "firefox-dev",
or an appropriate unique name for the command to run it.
3. Put each program folder in the same folder as the installer script;
4. Right click the installer script, select "proprieties", "permissions", and allow it to be run as application / executed as a program;
5. Right click the script directory, select "Open in terminal" and run it using the command: `./install-mozilla [applications]`
    - If the folder is called firefox-dev, you should run `./install-mozilla firefox-dev`
    - If you want to install firefox and thunderbird, you should run `./install-mozilla firefox thunderbird`
