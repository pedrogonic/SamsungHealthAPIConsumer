# Samsung Health API Consumer

## Contents

- Description
- Setup
  - Requirements
  - Creating a new project
  - Developer mode
  - Publishing the app
- Next Steps

## Description

A simple 1 screen Android app that consumes data from Samsung Health.

The app first asks for user permission to read data from the Health Database, then simply calls the Samsung Health API to recover the Steps Count information and displays the steps from the current day.

![image](/app/src/main/res/MainActivity.jpeg "")

## Setup

### Requirements

- Android device;
- Android API 23 or above;
- Smartwatch device compatible with Smasung Health;

### Creating a new project

If you wish to create a new project from scratch, you can follow the following steps.

First, you need to install the Samsung Health Android SDK. You can download it and find a detailed instruction at the [Samsung developer website](https://developer.samsung.com/health/android/overview.html). After loggin in, agree to all terms and download the SDK.

Then, Unzip the file and then copy samsung-health-data-a.b.c.jar to the "libs" folder of your new Android Studio project. Right click the file in the "Project" view and click the last option, Add As Library...

After that, just import the classes from the SDK and start using the API.

You can find API reference in this [page](https://img-developer.samsung.com/onlinedocs/health/android/data/index.html).

### Developer mode

In order to connect this app or the one created in the previous step to the data in your Samsung Health Data Store, you'll need to either register your app or enable the developer mode. In the development phase of your app it makes sense to simply enable the [developer mode](https://developer.samsung.com/health/android/data/programing-guide/developer-mode.html), as follows:

1. Open Smasung Health app;
2. go to the menu, at the hamburger icon;
3. open the setting at the cog;
4. click on the app's version, in the Information pane;
5. at last, click on the version number 10 times, in the screen with Terms and Conditions, Privacy Policy, etc. This should display \*(Developer Mode)\* before the version number.

If you wish to disable the Developer mode, you can repeat the process and click 10 more times.

### Publishing the app

To publish your app, you must submit it to Samsung's review, afetr registering for Partner APP. The whole process is described in the [documentation](https://developer.samsung.com/health/android/data/programing-guide/process.html).

## Next Steps

All code is contained in the Main Activity. This should be refactored.
