# SkullMods

1. Download the contents of this folder

2. Navigate to the game in your Steam library.

3. Click on **Properties** -> **Installed Files** -> **Browse**. This will open the game directory. 

4. Open Terminal at this folder. You can do it in two ways:  
    **4.1.** Right click on the folder name at the top -> Click on "common" -> Right click on the game folder name (Skul) -> Select "New Terminal At Folder"  
    **4.2**  Right click on "Skull.app" -> Select "New Terminal At Folder" -> In the Terminal tab run the following line: **cd ../**

5. Run the following line: **chmod u+x run_bepinex.sh**

6. Run **pwd** and copy the output. It should be the path to your game folder.

7. In Steam go to **Properties** -> **General** and find **Launch Options** at the bottom. 

8. Set the launch options to **"\<PWD\>/run_bepinex.sh" %command%** where '\<PWD\>' is the full path to the game folder you got above. 

9. Finally, open the **run_bepinex.sh** file with any text editor. Find the **DOORSTOP_CORLIB_OVERRIDE_PATH** variable. Change \<YOUR_USERNAME\> to your Mac username. It should be the second word in the path that you set in the game Launch Options.   

10. Now, add or remove any plugins you want in the "BepInEx/Plugins" folder. 

### !!!NOTES!!!

If your game folder is on the external drive or the installation path varies, change the path in step 9 accordingly.

Also, MacOS will alert you that you're trying to launch unverified files downloaded from the Internet (libdoorstop.dylib files). In order to allow it you have to go to the **System Settings** -> **Privacy and Security** and allow it from there