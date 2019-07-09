---
layout: post
title: Useful tools
categories: pc
description: Summary of useful software for programming and other stuff.
image: assets/images/radek-grzybowski.jpg
---

# Useful Tools

## Typora

Slim line markdown editor with live preview. Supports images, headers, lists, mathematics, code fences, tables, diagrams, inline styles, etc.

**How to install on Debian/Ubuntu**

```c
# or use
# sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys BA300B7755AFCFAE
wget -qO - https://typora.io/linux/public-key.asc | sudo apt-key add -

# add Typora's repository
sudo add-apt-repository 'deb https://typora.io/linux ./'
sudo apt-get update

# install typora
sudo apt-get install typora
```

**Upgrade Typora**

After installing Typora, the `typora` package will be managed by `apt-get`, so when your system updates installed packages, or you execute `apt-get upgrade`, Typora will be updated to latest version.

```c
# upgrade all packages include Typora
sudo apt-get upgrade
```

*(excerpt from [typora.io](https://typora.io/))*



## Atom

Modern and beautiful editor. Has an infinite amount of user add on packages for quite every purpose.


**Debian and Ubuntu (deb/apt)**

You can install Atom on Linux using your distribution's package  manager by configuring it to use one of our official package  repositories. This will also enable you to update Atom when new releases  are published.

To install Atom on Debian, Ubuntu, or related distributions, add our official
 package repository to your system by running the following commands:

```bash
wget -qO - https://packagecloud.io/AtomEditor/atom/gpgkey | sudo apt-key add -
sudo sh -c 'echo "deb [arch=amd64] https://packagecloud.io/AtomEditor/atom/any/ any main" > /etc/apt/sources.list.d/atom.list'
sudo apt-get update
```

You can now install Atom using `apt-get` (or `apt` on Ubuntu):

```bash
# Install Atom
sudo apt-get install atom
# Install Atom Beta
sudo apt-get install atom-beta
```

Alternatively, you can download the [Atom .deb package](https://atom.io/download/deb) and install it directly:

```bash
# Install Atom
sudo dpkg -i atom-amd64.deb
# Install Atom's dependencies if they are missing
sudo apt-get -f install
```

*(excerpt from [atom.io](https://flight-manual.atom.io/getting-started/sections/installing-atom/))*

## Anaconda

For x86 systems.

1. In your browser, download the [Anaconda installer for Linux](https://www.anaconda.com/download/#linux).

2. Optional: [Verify data integrity with MD5 or SHA-256](https://docs.anaconda.com/anaconda/install/hashes/). (For more information on hashes, see [cryptographic hash validation](https://conda.io/projects/conda/en/latest/user-guide/install/download.html#cryptographic-hash-verification).)

   1. Run the following:

      ```bash
      md5sum /path/filename
      ```

      OR:

      ```bash
      sha256sum /path/filename
      ```

      NOTE: Replace `/path/filename` with the actual path and filename of the file you downloaded.

   2. Optional: Verify results against [the proper hash page](https://docs.anaconda.com/anaconda/install/hashes/) to make sure the hashes match.

3. Enter the following to install Anaconda for Python 3.7:

   ```bash
   bash ~/Downloads/Anaconda3-5.3.0-Linux-x86_64.sh
   ```

   OR Enter the following to install Anaconda for Python 2.7:

   ```bash
   bash ~/Downloads/Anaconda2-5.3.0-Linux-x86_64.sh
   ```

   NOTE: Include the `bash` command regardless of whether or not you are using Bash shell.

   NOTE: If you did not download to your Downloads directory, replace `~/Downloads/` with the path to the file you downloaded.

   NOTE: Choose “Install Anaconda as a user” unless root privileges are required.

4. The installer prompts “In order to continue the installation process, please review the license agreement.” Click Enter to view license terms.

5. Scroll to the bottom of the license terms and enter “Yes” to agree.

6. The installer prompts you to click Enter to accept the default install location, CTRL-C to cancel the installation, or specify an alternate installation directory. If you accept the default install location, the installer displays “PREFIX=/home/<user>/anaconda<2 or 3>” and continues the installation. It may take a few minutes to complete.

7. The installer prompts “Do you wish the installer to prepend the Anaconda<2 or 3> install location to PATH in your /home/<user>/.bashrc ?” Enter `Yes`.

   NOTE: If you enter “No”, you must manually add the path to Anaconda or conda will not work. See [FAQ](https://docs.anaconda.com/anaconda/user-guide/faq/#distribution-faq-linux-path).

8. The installer describes Microsoft VS Code and asks if you would like to install VS Code. Enter `yes` or `no`. If you selected `yes`, follow the instructions on screen to complete the VS Code installation.

   NOTE: Installing VS Code with the Anaconda installer requires an internet connection. Offline users may be able to find an offline VS Code installer from Microsoft.

9. The installer finishes and displays “Thank you for installing Anaconda<2 or 3>!”

10. Close and open your terminal window for the installation to take effect, or you can enter the command `source ~/.bashrc`.

11. After your install is complete, verify it by opening Anaconda Navigator, a program that is included with Anaconda: Open a Terminal window and type `anaconda-navigator`. If Navigator opens, you have successfully installed Anaconda. If not, check that you completed each step above, then see our Help page.

    TIP: For more information about Anaconda Navigator, see [Navigator](https://docs.anaconda.com/anaconda/navigator/).

After your install completes, start using Anaconda with the instructions in [Getting started with Anaconda](https://docs.anaconda.com/anaconda/user-guide/getting-started/).

NOTE: If you install multiple versions of Anaconda, the system defaults to the most current version, as long as you haven’t altered the default install path.

*(excerpt from [anaconda.com](https://docs.anaconda.com/anaconda/install/linux/))*



## Android Studio

## Tex Studio

## Notepadqq

## Eclipse

## Blender

Blender is the free and open source 3D creation suite. It supports the
entirety of the 3D pipeline—modeling, rigging, animation, simulation,
rendering, compositing and motion tracking, even video editing and game
creation.

```bash
sudo apt-get install blender
```

*(excerpt from [blender.com](https://www.blender.org/))*

## Git

## Jekyll
