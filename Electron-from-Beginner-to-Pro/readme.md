# Electron From Beginner to Pro  (2017)
__By Christ Griffith and Leif Wells__  

## Chapter 1: Welcome to Electron  
Electron is a blend of two technologies: _Node.js_ and _Chromium_.  

__How Does Electron Work?__  
Electron-based applications run in two distinct processes: the _main process_ and the _render process_. Many of the Node modules that Electron provides are only available within a specific process. For example, access to  the operating system APIs are restricted to just the main process and access to the clipboard is available to both the main and render process.

__Other Solutions__  
The most common alternative to Electron is known as _NW.JS ([nwjs.io](https://nwjs.io)_). Originally known as node-webkit.

## Chapter 2: Installing Electron  
To setup the development environment install the following:
* Node.js
* Git  
* Electron

 __Installing Electron__  
 Install electron globally:    
 ```
 > npm install -g electron  
 ```
 Or install electron locally on a per project basis:  
 ```
 > npm install --save-dev electron
 ```
Check the version of electron installed globally:   
```
> electron -v  
```

## Chapter 3: The Electron Quick Start  
The Electron Quick Start is located at [github.com/electron/electron-quick-start](https://github.com/electron/electron-quick-start).        

Go to [electronjs.org/community#boilerplates](https://www.electronjs.org/community#boilerplates) to explore various electron boiler plates.  
You can also find Components and Tools on the same page.  

There is an _angular-electron_ scaffolding on github: [angular-electron](https://github.com/maximegris/angular-electron)

Start the electron-quick-start app:  
```
> npm start
```  

## Chapter 4: BrowserWindow Basics  
 For Browser Window options see [electron.atom.
io/docs/api/browser-window](https://electron.atom.io/docs/api/browser-window/#class-browserwindow)  

__Frameless Windows__  
A frameless window has no menu bar, title bar or toolbars. To create a frameless window, set the `frame` property to `false` for the option argument of the BrowserWindow constructor.  

__Transparent Windows__  
To get a transparent window, set the `transparent` property of the options object passed to the BrowserWindow constructor to `true`.
__NB:__ This does not work on Windows OS unless the window is frameless.

## Chapter 5: Add Custom Menus  
We have a custom menu, you have to create the entire menu.  

__Defining Keyboard Shortcuts and Menu Item Roles__
You should always follow the platform convention for keyboard shortcuts and menu naming. Refer to each platform’s user interface guidelines for further information.
