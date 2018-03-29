# Google Maps In Android
This guide is a quick start to adding a map to an Android app. Android Studio is the recommended development environment for building an app with the Google Maps Android API.

Step 1. Download Android Studio

Step 2. Install the Google Play services SDK

Step 3. Create a Google Maps project
Follow these steps to create a new app project including a map activity:

Start Android Studio.
Create a new project as follows:

If you see the Welcome to Android Studio dialog, choose Start a new Android Studio project, available under 'Quick Start' on the right of the dialog.
Otherwise, click File in the Android Studio menu bar, then New, New Project.
Enter your app name, company domain, and project location, as prompted. Then click Next.

Select the form factors you need for your app. If you're not sure what you need, just select Phone and Tablet. Then click Next.
Select Google Maps Activity in the 'Add an activity to Mobile' dialog. Then click Next.
Enter the activity name, layout name and title as prompted. The default values are fine. Then click Finish.
Android Studio starts Gradle and builds your project. This may take a few seconds. For more information about creating a project in Android Studio, see the Android Studio documentation.
When the build is finished, Android Studio opens the google_maps_api.xml and the MapsActivity.java files in the editor. (Note that your activity may have a different name, but it will be the one you configured during setup.) Notice that the google_maps_api.xml file contains instructions on getting a Google Maps API key before you try to run the application. The next section describes getting the API key in more detail.

Step 4. Get a Google Maps API key
Your application needs an API key to access the Google Maps servers. The type of key you need is an API key with restriction for Android apps. The key is free. You can use it with any of your applications that call the Google Maps Android API, and it supports an unlimited number of users.
step 5:
 To get one, follow this link, follow the directions and press "Create" at the end:
https://console.developers.google.com/flows/enableapi?apiid=maps_android_backend&keyType=CLIENT_SIDE_ANDROID&r=03:86:4B:7A:25:F9:9B:99:B2:B3:5E:A2:3E:48:A1:26:15:5D:AF:32%3Bcom.example.dellpc.map

Step 6. Connect an Android device
The simplest way to see your app in action is to connect an Android device to your computer. Follow the instructions to enable developer options on your Android device and configure your application and system to detect the device.

Alternatively, you can use the Android Emulator to run your app. Use the Android Virtual Device (AVD) Manager to configure one or more virtual devices which you'll be able to use with the Android Emulator when you build and run your app. When choosing your emulator, ensure that you use Android 4.2.2 or higher, and be careful to pick an image that includes the Google APIs, or the application will not have the requisite runtime APIs in order to execute. Also, take note of the instructions for configuring virtual machine acceleration, which you should use with an x86 target AVD as described in the instructions. This will improve your experience with the emulator.

Step 7. Build and run your app
In Android Studio, click the Run menu option (or the play button icon) to run your app.

When prompted to choose a device, choose one of the following options:

Select the Android device that's connected to your computer.
Alternatively, select the Launch emulator radio button and choose the virtual device that you've previously configured.
Click OK. Android Studio will invoke Gradle to build your app, and then display the results on the device or on the emulator. It could take a couple of minutes before the app opens.

You should see a map with a marker positioned over Sydney, Australia. If you don't see a map, confirm that you've completed all the steps described on this page. In particular, check that you've added an API key as described above.
