# things-bluetooth-audio
This app can connect and play audio in your Android Things device.

## Pre-requisites

- Android Things compatible board
- Android Studio 2.2+
- (optional) a speaker or headsets, so that you can listen to the audio and
  notifications.
- (optional) Two buttons connected to the GPIO pins, so that you can control the
  sample at runtime. Without the buttons, you can use a keyboard or adb. For
  more on this, look at the main activity, where the supported commands are
  described.
  
  ## Build and install

On Android Studio, click on the "Run" button.

If you prefer to run on the command line, type

```bash
./gradlew installDebug
adb shell am start com.example.androidthings.bluetooth.audio/.A2dpSinkActivity
```
