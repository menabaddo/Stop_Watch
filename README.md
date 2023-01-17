# Stopwatch App
This is a simple stopwatch application for Android devices. It is written in Java and allows users to start, stop, and reset a timer. The App also saves the state of the timer even when the app is closed or the device is rotated.
## Features
* Start, stop, and reset functionality
* Saving timer state even when app is closed or device is rotated
* easy to use interface

## Screenshot
![stopwatch](https://user-images.githubusercontent.com/104861566/213002372-d532f736-9ea5-43a0-916d-fae2a045ee46.PNG)

## Getting Started
1. Clone or download the repository
2. Open the project in Android Studio
3. Connect an Android device or use an emulator
4. Build and run the app on the device/emulator

## Usage
* Press the "Start" button to begin timing
* Press the "Stop" button to stop the timer
* Press the "Reset" button to reset the timer to zero
* The app saves the state of the timer even when the app is closed or device is rotated

## Code Highlight
The App uses onSaveInstanceState and onCreate method to save and restore the state of the timer <br/>
```java
if(savedInstanceState != null){ 
            savedInstanceState.getInt("seconds");
            savedInstanceState.getBoolean("running");
            savedInstanceState.getBoolean("wasRunning");
    }
   ```
```java    
@Override
    public void onSaveInstanceState(@NonNull Bundle outState) {
        super.onSaveInstanceState(outState);
        outState.putInt("seconds", seconds);
        outState.putBoolean("running", running);
        outState.putBoolean("wasRunning", wasRunning);
    }
```
## Contributing 
If you wish to contribute to this project, please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details

## Acknowledgements
* Hat tip to anyone whose code was used
* Inspiration
* etc

Please let me know if there is anything else you would like me to include.
    
    
