# React-Electron Desktop Application

## Working Demo
A working demo can be found at the following for download:

https://github.com/AncientAbysswalker/Electron-React-Desktop-Overlay/tree/master/build

## Problem Statement
I used to play around with Rainmeter to make custom desktop skins. More recently I was considering the feasibility of doing similar with more complete programming languages (no LUA, not you). I set out to see if it was possible to make something remotely viable. There are several key features that are required to be useful:

* It should be possible to render the application as something other than a standard rectangular window
* It should be possible to drag parts of the application around to rearrange the application(s)
* Parts of the application may need to be click-through enabled
* Application should not interfere with standard OS UI commands, like double or right clicking items on the desktop

This repository is a mirror of the key features I have developed in getting the basic functionality operational. There are bugs in this implementation and they will be addressed as I develop in my [main code base](https://github.com/AncientAbysswalker/Elysian-Cannon).

## Implementation

The implementation that I am currently working with is a React-Electron Application. This affords very flexible development of UI elements. As Electron is a chromium extension, I had also to make the window and frame transparent and encompass the entire screen. As the screen is across the entire screen, additional code is required to pass-through mouse events. The UI elements can be made draggable using [React-Draggable](https://www.npmjs.com/package/react-draggable).

![Example Functionality](https://raw.githubusercontent.com/AncientAbysswalker/Electron-React-Desktop-Overlay/master/md/example.gif)
