### how to create electron app

create a new project

	npm init
	
add electron library to your project

	npm install --save electron
	
add index.html and index.js -- basic js setup

```
  const electron = require('electron');
  const {app, BrowserWindow} = electron;
  
  app.on('ready', () => {
      const mainWindow = new BrowserWindow({});
      mainWindow.loadURL(`file://${__dirname}/index.html`)
  });
```
	
add npn script to run electron app

	"scripts": {
        "electron": "electron ."
    }
    
run app
    
 	npm run electron