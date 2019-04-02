# Run-Scripts-to-Strip-Framework-Unsupported-Platform-Codes
This Bash Script will remove unsupported Code from your Pod/Framwork while Archiving the App to Upload on App Store


## Guide to Use

* Click on your Xcode Prject On Left pan Window
* Then Click on Targets
* Goto Build Phases Settings
* Click on Plus icon and Add "New Run Script Phase"
* Now under the Shell option below is a console box ,Put your script location there
* In my case my script was in my 3rd party framwork(wowzaGoCoderFramwork), so my path is like this

```swift

bash "${BUILT_PRODUCTS_DIR}/${FRAMEWORKS_FOLDER_PATH}/WowzaGoCoderSDK.framework/strip-frameworks.sh"

```

* Thats it now you are done , Start Archiving your project it will strip the unsupported code automatically
* if You want to see the echo messages/Prgress , Click on left Pane and Select Message bubble icon "Report Naviagtor".
