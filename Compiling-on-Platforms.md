## How to compile Apple Music Electron
For most platforms, this is extremely straightforward as it only requires 3 simple CLI commands to get it up and running.

Run the below commands to compile but if that doesn't work continue reading.

### Requirements:
* [Node.JS](https://nodejs.org/) (13+ preferably.)
* [yarn](https://www.npmjs.com/package/yarn)
* [Visual Studio](https://visualstudio.microsoft.com/) (if on Windows)
* Simple Command Line Knowledge

Once you have those items on your machine, enter the commands below. However, if you run into compilation issues please report them in [Issues](https://github.com/cryptofyre/Apple-Music-Electron/issues)
<br />



```
git clone https://github.com/cryptofyre/Apple-Music-Electron.git

yarn install

yarn dist
```
After you compile your app, it should be in the source directory inside the `dist` folder.