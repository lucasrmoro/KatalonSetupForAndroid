# Katalon setup for Android

- [Pre-requisites](#pre-requisites)
- [Enviroment setup](#project-setup)
- [Running tests](#running-tests)
- [How to map the screens](#how-to-map-the-screens)
- [How to create tests](#how-to-create-tests)

### Pre-requisites

1. [Install Katalon (It's necessary create an account for it)](https://www.katalon.com/download/)
2. [Install Node JS](https://nodejs.org/en/download/)
3. [Install Appium](https://appium.io/docs/en/about-appium/getting-started/?lang=en)
4. [Install ADB (If you don't have it yet)](https://developer.android.com/studio/releases/platform-tools)

### Enviroment setup

1. Do login with your account in the Katalon
2. In the top toolbar go to `Window -> Katalon Studio Preferences -> Katalon -> Mobile -> Set the Appium Directory`
3. Install the App in your device

### Running tests

1. Open your project
2. Open the Tests Suites folder and go to Main Test Suite
3. In the top of screen, click in the run button
4. Select your device and wait the tests run

### How to map the screens

1. Go to the option `Spy Mobile` that's a green phone icon
2. Select Android Devices
3. Select your device on `Device Name`
	 - Selecting Android App by ID
		- Install the App in your device
        - In `Start with` select Application ID
        - In `Application ID` put `your.android.package.here`
     - Selecting Android App by APK
		- Keep `Start with` on `Application File`
		- In `Application File` tap `Browse` and select the APK file
4. Tap Start
5. In the list `ALL OBJECTS` below `Application ID` we have all objects that the current screen contains
6. Select the object you want to map in the check box at left
7. Rename the `Object Name` to the object name
8. The `Locator Strategy` it's how the software will identify your object (View), select the most detailed type (prefer `ID`)
9. Then click `Add to Object Repository` in the left top corner and select the place that you want to save

_Ps.: To map another screen, go to the desired screen in your device and click on `Capture Object` at side of `Start`._

### How to create tests

1. Create a folder with the name of feature you going to test inside `Test Cases` folder
2. Create a `Test Case` file
3. Inside the file created, click in `Add` button
4. In the `Item` column, choose the action you want to do, `Tap, Set Text, Wait For Element Present, Scroll To Text...`
5. In the `Object` column, choose the object (view) you want to perform this action
6. In the `Input` column, put the desired parameters. For the `Delay` action for example, select the desired delay time

### Links
[**OTP Code generator by token** Plugin](https://store.katalon.com/product/28/TOTP-Generator-Keywords#overview-content)
