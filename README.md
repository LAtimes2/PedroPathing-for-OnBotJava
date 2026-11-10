# PedroPathing for OnBotJava



This repository provides files that can be uploaded to OnBotJava on an FTC Control Hub to run the [PedroPathing](https://github.com/Pedro-Pathing) path follower library.



## NOTE: PedroPathing version 3

PedroPathing 3 changes how tuning works, using a web page. This is not working with OnBotJava yet (ever?), so there are 2 options:



1. Do your tuning using OnBotJava (currently only supports Mecanum drivetrain, Pinpoint localizer and Foresight algorithm. More localizers coming soon). Follow the instructions in the Tuning folder in Tuning Instructions.pdf
2. Do your tuning using Android Studio QuickStart project, and copy the Constants.java file to OnBotJava



PedroPathing is usually used in Android Studio, but sometimes a team may want to use OnBotJava instead. The OnBotJava version is the same as the Android Studio version except that Tuning is done differently (since I haven't figured out how to implement kotlin and WebServer in OnBotJava).



Instructions:



1. Perform PedroPathing tuning to create your Constants.java file in the pedro folder in OnBotJava
2. Upload the PedroPathing.jar file from this directory to OnBotJava
3. Follow the instructions for PedroPathing at https://pedropathing.com/docs/pathing/guide/setting-up-auto. Files from the Visualizer (https://visualizer.pedropathing.com/) can be used for paths.



If there are any problems with the documentation on how to do this, you can add an issue in GitHub here: https://github.com/LAtimes2/PedroPathing-for-OnBotJava/issues





This version of PedroPathing.jar is version 3.0.2. See the source\_code folder for the PedroPathing code in the jar file and instructions on how to rebuild the jar file for newer versions.

