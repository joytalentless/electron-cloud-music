# NeteaseCloudMusic Electron
## Build

```bash
git clone https://github.com/disoul/electron-cloud-music && cd electron-cloud-music
npm install

# Dev

# Start dev server
npm run dev

# run cloudmusic in proj root path
# electron will load from 127.0.0.1:8080(webpack-dev-server
npm start

# Release

vim main.js
# edit main.js like this
//mainWindow.loadURL('http://127.0.0.1:8080');
mainWindow.loadURL('file://' + __dirname + '/index.html');

# build
make release
```
