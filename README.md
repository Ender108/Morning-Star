# Morning Star
Ascendance is a modlist that focuses on improving Skyrim’s gameplay and visuals.

**Modlist Support: [Waking Dreams](https://discord.gg/4WwqfK5yHg)**

>[!IMPORTANT]
>Morning Star requires the four free AE mods (Fishing, Rare Curios, Survival Mode, and Saints and Seducers) included in the Skyrim Anniversary Edition update from November 2021. This modlist does **NOT** utilize the AE DLC, only these four free AE mods are used.

>[!WARNING]
>You must update Skyrim to the latest version (1.6.1170) on Steam to install this list.

# Installation

Installing Morning Star is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

## Pre-Installation

These steps are only required for installing the modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 9.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

### Setting Shader Cache Size (NVIDIA Users Only)

>[!IMPORTANT]
>For NVIDIA users, it is recommended to boost the size of the shader cache. These settings have been shown to improve stability, while it may not be entirely necessary, it is still recommended.

**To do this:**

- Right-click on your desktop and select `NVIDIA Control Panel`
- Navigate and click `Manage 3D Settings`
- Scroll down the **Global Settings** tab until you see **Shader Cache Size**
- Double-click `Driver Default` to the right of **Shader Cache Size** and select `10 GB`
- Click `Apply` in the bottom right hand corner
- Exit out of the application
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

### Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Skyrim so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Skyrim SE and click on properties, untick the `Enable Steam Overlay while in-game.`
 3. Please ensure you follow the steps outlined in the [Installing Creation Club Files](#installing-creation-club-files) section. **DO NOT SKIP THIS STEP OR YOUR INSTALL WILL FAIL.**

### Changing the Game Language

>[!WARNING]
>**The English Steam version of Skyrim SE is the only supported version.**

I understand that this may be frustrating for non-English speaking users or users with the GOG/Bethesda.net versions, but due to the core file differences between the different versions, I am only able to support one game version.

To change your Skyrim SE's language:

 1. Right click on Skyrim SE in Steam
 2. Click `Properties`
 3. Click `Language`
 4. Set the Language to `English`

### Installing Creation Club Files
>
>[!WARNING]
> ***Do NOT skip this step or your install may fail!***

Since the 1.6.1130 update (January 17, 2024), Steam has begun including the free Creation Club (CC) files with the base installation of Skyrim. However, these files do not have the same file hash as the files that are downloaded from the in-game **Creations** menu for Anniversary Edition (AE) users. In order to comply with Wabbajack policy and minimize issues for users who own the AE update, Morning Star is compiled using the versions of the CC content that are obtained from the in-game **Creations** menu.  

As a result of this, for users who do not own the AE, you must ensure that you download the correct version of the CC files. Steps below:

 - Navigate to your Skyrim SE's Steam Data folder
    - i.e. `D:\SteamLibrary\steamapps\common\Skyrim Special Edition\data`
 - Delete *both* Rare Curios files:
    - `ccbgssse037-curios.bsa`
    - `ccbgssse037-curios.esl`
 - Launch Skyrim SE from Steam and select **Creations** at the main menu
 - Select **Search** at the bottom and search for `Rare Curios`
 - Select the card titled `Rare Curios` and press **Download**
 - Once it is done, accept Bethesda's load order message and exit the game

![](https://cdn.discordapp.com/attachments/1008055818782003421/1263168806054920283/Rare_Curios.png?ex=673cbb1f&is=673b699f&hm=1f79621666901b9b4fd93a5a1eb0732779388c4fa3fe4bb77d2211ffb6ab881b&)

>[!IMPORTANT]
>
>- **DO NOT** Alt+Tab during this process or it will fail to properly download these files.
>- **DO NOT** verify your game files after doing the steps above as it will revert the "correct" file hashes for the CC files you downloaded in this step.

## Wabbajack Installation

### Installing Wabbajack

Once you have completed the pre-installation section, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), in your Skyrim's Steam folder, or in any folders related to the modlist itself (the downloads or install folder).**
    > - The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be on an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

>[!IMPORTANT]
>The list requires Wabbajack version **4.0.0.0 or later**. Installing the modlist on older versions of Wabbajack will result in issues.

### Downloading and Installing Morning Star

>[!CAUTION]
>**A legal copy of Skyrim Special Edition is required.** Pirated copies of the game will cause the installation to fail and even if you manage to somehow get around Wabbajack's built-in piracy prevention measures, SKSE does not work with the cracked exes.  

Downloading and installing Morning Star can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the **Slow Download** button for each mod.

To install Morning Star, complete the following steps:

 1. Open Wabbajack and click `Browse lists`
 2. Pick the **Skyrim Special Edition** option from the game filter drop-down box (or use the search bar to find the modlist).
 3. Press the download arrow on the Morning Star UI card and wait for it to download
 4. Set the `Installation Location` to a folder such as `C:\Morning Star`.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Skyrim's Steam folder**
    > - The `Downloads Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
 5. Press the `Install` button.
 6. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again.
 7. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow the tips below or the [discord server](https://discord.gg/4WwqfK5yHg) for support.
