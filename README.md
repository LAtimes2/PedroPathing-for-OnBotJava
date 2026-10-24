# PedroPathing for OnBotJava



This repository provides files that can be uploaded to OnBotJava on an FTC Control Hub to run the [PedroPathing](https://github.com/Pedro-Pathing) path follower library.



## NOTE: PedroPathing version 3

PedroPathing 3 changes how tuning works, using a web page. This is not working with OnBotJava yet, so there are 3 options:

1. Do your tuning using Android Studio QuickStart project, and copy the Constants.java file to OnBotJava
2. Manual tuning similar to version 2. If you are using Pinpoint, there is a Constants.java\_pinpoint that can be renamed to Constants.java as a starting point, but at a minimum the podOffset and podDirction parameters will need to be updated.
3. Use PedroPathing version 2, which can be downloaded by selecting Release v2.1.1 on the right hand side





PedroPathing is usually used in Android Studio, but sometimes a team may want to use OnBotJava instead. The OnBotJava version is the same as the Android Studio version except that Tuning has been removed (since I haven't figured out how to implement kotlin and WebServer in OnBotJava).



Instructions:

1. Upload 2 files from this directory to OnBotJava (PedroPathing.jar, Constants.java)
2. Follow the instructions for PedroPathing. Files from the Visualizer can be used for paths.



This version of PedroPathing.jar is version 3.0.2. See the source\_code folder for the PedroPathing code in the jar file and instructions on how to rebuild the jar file for newer versions.

