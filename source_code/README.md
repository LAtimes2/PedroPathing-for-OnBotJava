# PedroPathing Source Code



This folder contains the source code used to create the PedroPathing.jar file. It is a slightly modified version of the files from the [PedroPathing](https://github.com/Pedro-Pathing/PedroPathing), [Telemetry](https://github.com/Pedro-Pathing/Telemetry) and [QuickStart](https://github.com/Pedro-Pathing/Quickstart) repositories.



A quick explanation of jar files: A .jar file in this instance is just a .zip file. You can change the filename extension to .zip to look at the files using standard tools. The .jar file contains .class files. When you build a program in Android Studio or OnBotJava, it converts the .java files to .class files.



A general overview of building the jar file: The current .java files are renamed from src to src\_orig. The PedroPathing .java files are uploaded to OnBotJava and built. The build process creates a .jar file with the .class files. The .jar file is copied off of the Control Hub and possibly edited. The PedroPathing .java files are deleted and the original files renamed from src\_orig back to src.



Instructions for building jar file:

1. You will need to connect this computer to the Control Hub via a USB cable to copy files to and from the Control Hub
2. Make a backup of any .java files on the Control Hub that you want to keep, just in case
   (they should be preserved, but things can go wrong. Also, there are backups on the Control Hub at This PC\\Control Hub v1.0\\Internal shared storage\\FIRST\\java\\srcBackups)
3. On the Control Hub, rename This PC\\Control Hub v1.0\\Internal shared storage\\FIRST\\java src to src\_orig
4. Create the directory structure using 1 of the following:
   a. Upload a file such as DriveTrain.java to OnBotJava using the Web browser and build it (ignore any errors)
   or
   b. Create FIRST\\java\\src\\com\\pedropathing folder
5. Using file explorer, copy the GitHub files from source_code to FIRST\\java\\src\\com\\pedropathing
6. Restart OnBotJava to load the copied files (select Manage, then OnBotJava)
6. In OnBotJava, build the java files. There should not be any errors
7. In the file explorer, go to FIRST\\java\\build\\jars
8. There may be multiple folders starting with onBotJavaJars. Open the one with the latest date/time.
9. Copy OnBotJava.jar to the PC
10. On the PC, rename OnBotJava.jar to pedroPathing.jar
11. In FIRST\\java, delete src and rename src_orig back to src
