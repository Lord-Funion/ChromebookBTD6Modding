# How to Mod BTD6 on a Chromebook

## Steps to Mod Bloons TD6 (BTD6)

1. Press `Ctrl + Alt + T` to open Crosh.
2. Type the following command:
   ```sh
   vmc share borealis Downloads
   ```
3. Enter the virtual shell:
   ```sh
   vsh borealis
   ```
4. Download [Windows File Explorer](https://windows-file-explorer.en.softonic.com/download).
5. In the terminal, move the downloaded file:
   ```sh
   cp /mnt/shared/MyFiles/Downloads/FileExplorer.exe /home/chronos/.local/Steam/steamapps/BloonsTD6
   ```
6. Navigate to the BTD6 directory:
   ```sh
   cd /home/chronos/.local/Steam/steamapps/BloonsTD6
   ```
7. Rename the original game executable:
   ```sh
   mv BloonsTD6.exe BloonsTD6.exe.bak
   ```
8. Replace it with File Explorer:
   ```sh
   mv FileExplorer.exe BloonsTD6.exe
   ```
9. Open Steam and run BTD6.
10. When an installer opens, follow the installation instructions.
11. Remove the replaced executable:
    ```sh
    rm -rf BloonsTD6.exe
    ```

## Installing MelonLoader

12. Download [MelonLoader](https://github.com/LavaGang/MelonLoader/releases/latest/download/MelonLoader.x64.zip).
13. Extract the downloaded file.
14. Copy the extracted files to the BTD6 directory:
    ```sh
    cp /mnt/shared/MyFiles/Downloads/MelonLoader.x64/Melonloader -r /home/chronos/.local/Steam/steamapps/BloonsTD6
    ```
15. Copy the version DLL:
    ```sh
    cp /mnt/shared/MyFiles/Downloads/MelonLoader.x64/version.dll  /home/chronos/.local/Steam/steamapps/BloonsTD6
    ```

## Installing .NET SDK

16. Download [.NET SDK 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-6.0.428-windows-x64-installer).
17. Move it to the game directory:
    ```sh
    cp /mnt/shared/MyFiles/Downloads/dotnet-sdk-6.0.428-win-x64.exe /home/chronos/.local/Steam/steamapps/BloonsTD6
    ```
18. Rename the SDK installer:
    ```sh
    mv dotnet-sdk-6.0.428-win-x64.exe BloonsTD6.exe
    ```
19. Run BTD6 in Steam and follow installation prompts.
20. Remove the installer after installation:
    ```sh
    rm -rf BloonsTD6.exe
    ```

## Installing Visual C++ Redistributable

21. Download [VC Redist](https://aka.ms/vs/16/release/vc_redist.x64.exe).
22. Move it to the game directory:
    ```sh
    cp /mnt/shared/MyFiles/Downloads/VC_redist.x64.exe /home/chronos/.local/Steam/steamapps/BloonsTD6
    ```
23. Rename the installer:
    ```sh
    mv VC_redist.x64.exe BloonsTD6.exe
    ```
24. Run BTD6 and install what it requires.
25. Remove the installer:
    ```sh
    rm -rf BloonsTD6.exe
    ```
26. Restore the original game executable:
    ```sh
    mv BloonsTD6.exe.bak BloonsTD6.exe
    ```
27. Run BTD6 and wait for it to load.
28. Once loading is complete, close the game.

## Installing Mods

29. Download your favorite mods.
30. Move the mod file to the Mods folder (replace `<mod_name>` with the actual mod file name):
    ```sh
    cp /mnt/shared/MyFiles/Downloads/<mod_name> /home/chronos/.local/share/Steam/steamapps/common/BloonsTD6/Mods
    ```

Now you have successfully modded BTD6 on your Chromebook!

