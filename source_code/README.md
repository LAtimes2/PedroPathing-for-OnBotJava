# PedroPathing Source Code

# Needs to be updated for PedroPathing3 !!!



This folder contains the source code used to create the PedroPathing.jar file. It is a slightly modified version of the files from the [PedroPathing](https://github.com/Pedro-Pathing/PedroPathing), [Telemetry](https://github.com/Pedro-Pathing/Telemetry) and [QuickStart](https://github.com/Pedro-Pathing/Quickstart) repositories. Modifications include removing imports of org.jetbrains.annotations.NotNull.



A quick explanation of jar files: A .jar file in this instance is just a .zip file. You can change the filename extension to .zip to look at the files using standard tools. The .jar file contains .class files. When you build a program in Android Studio or OnBotJava, it converts the .java files to .class files.



A general overview of building the jar file: The current .java files are renamed from src to src\_orig. The PedroPathing .java files are uploaded to OnBotJava and built. The build process creates a .jar file with the .class files. The .jar file is copied off of the Control Hub and possibly edited. The PedroPathing .java files are deleted and the original files renamed from src\_orig back to src.



If the updated source code is not in this directory, do the following:

1. Copy all directories in PedroPathing repository core\\src\\main\\java\\com\\pedropathing directory to this directory.
2. Copy revhub directory in PedroPathing repository revhub\\src\\main\\java\\com\\pedropathing directory to this directory.
3. Copy Tuning directory in Autotune repository AutoTune\\tree\\main\\Tuning\\src\\main\\java\\com\\pedropathing directory to this directory
4. Copy telemetry directory in Telemetry repository telemetry\\src\\main\\java\\com\\pedropathing directory to this directory. Need to comment out references to NotNull.
5. Copy Constants.java and Tuning.java from QuickStart repository to directory above this one (PedroPathing-for-OnBotJava)
6. If update needed, copy NanoIdUtils.java in jnanoid repository (https://github.com/aventrix/jnanoid) to FIRST\\java\\src\\com\\aventrix\\jnanoid\\jnanoid \[or upload via OnBotJava]
7. repo.dairy.foundation/@/releases/dev/frozenmilk/Sinister. choose latest version (2.3.0). download Sinister-x.x.x.jar



Instructions for building jar file:

1. You will need to connect this computer to the Control Hub via a USB cable to copy files to and from the Control Hub
2. Make a backup of any .java files on the Control Hub that you want to keep, just in case (Download via OnBotJava)
(they should be preserved, but things can go wrong. Also, there are backups on the Control Hub at This PC\\Control Hub v1.0\\Internal shared storage\\FIRST\\java\\srcBackups)
3. Close any connections in the Web browser to OnBotJava
4. On the Control Hub, rename This PC\\Control Hub v1.0\\Internal shared storage\\FIRST\\java src to src\_orig
5. You can re-open OnBotJava any time after this
6. If you have PedroPathing.jar loaded in OnBotJava under ExternalLibraries, delete it
7. Create the directory structure using 1 of the following:
a. Upload a file such as ErrorCalculator.java to OnBotJava using the Web browser and build it (ignore any errors)
or
b. Create FIRST\\java\\src\\com\\pedropathing folder
8. Using file explorer, copy the GitHub files from source\_code to FIRST\\java\\src\\com\\pedropathing
9. Restart OnBotJava to load the copied files (select Manage, then OnBotJava)
10. In OnBotJava, build the java files. There should not be any errors
11. In the file explorer, go to FIRST\\java\\build\\jars
12. There may be multiple folders starting with onBotJavaJar. Open the one with the latest date/time.
13. Copy OnBotJava.jar to the PC in the PedroPathing-for-OnBotJava directory
14. On the PC, rename OnBotJava.jar to PedroPathing.jar
15. Close OnBotJava (go to Manage tab)
16. In FIRST\\java, delete src and rename src\_orig back to src
17. You will have to upload the new PedroPathing.jar file into OnBotJava

