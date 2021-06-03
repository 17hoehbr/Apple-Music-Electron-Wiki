## Troubleshooting
Troubleshooting can be done in a series of ways. Below is a list of the current methods you can troubleshoot issues with the application.

**Log File**
* The logging file can be found at `%APPDATA%\Apple Music\logs\main.log`. This file should contain all you need to see what is causing issues in the application. The log file will show you what active function is being run and when CSS/JS is loaded. It overrides the `console.log` function, so if you add them in your code, it will be logged to the file. 

**Clean Installation**
* A simple clean installation can be done by uninstalling the application (on Windows this can be done the System Setting) and clearing all application data:
* After you have uninstalled the application, you can begin by deleting the following folders if they exist:
* `%APPDATA%\Apple Music`
* `%LOCALAPPDATA%\Programs\apple-music-electron`
* `%LOCALAPPDATA%\apple-music-electron-updater`
* Then reinstall the application from [here](https://github.com/cryptofyre/Apple-Music-Electron/releases/latest).

## Troubleshooting Advanced

**Enabling DevTools**
* It is advised to turn on `allowSetMenu` variable in advanced section in [config.json](https://github.com/cryptofyre/Apple-Music-Electron/blob/master/config.json#L41) for troubleshooting. This will allow the Chrome DevTools like inspect element and access to the renderer console, this can all be done by doing `CTRL + SHIFT + I`. 
* You can find all the documentation for the Chrome Dev Tools [here](https://developer.chrome.com/docs/devtools/).

**JS Troubleshooting**
* If you are creating a JavaScript file that you want to inject into the application, most errors will be moved into the renderer's console. JavaScript can also be run in the console if you'd like to test it first. 
* It is also recommended that you try-catch all your code as this assists in narrowing down the cause of errors.

**CSS Troubleshooting**
* This is round about the same as it is for JS Troubleshooting. However, you cannot run CSS in the console (unless it is being done through a JS Function). CSS can be edited in Inspect Element and you can adjust global variables in the Inspect Element page, more information can be found in the DevTools documentation.