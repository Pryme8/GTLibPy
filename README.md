![cover_logo](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/cover_logo.jpg?raw=true "")

_GTLib**Py**_ is **[Game Trainer](https://en.wikipedia.org/wiki/Trainer_(games)) library/module for _Python in windows_** it provides all the necessary methods to make simple game trainer in
windows using **WIN32-API** with ease.
It uses only **WIN32-API** methods because this is intended to work on **Windows** system only
and not shall be portable or to target other OS like **_Linux_,_MAC OS_** etc.

**NOTE** : This ain't memory scanning,hooking,analyzing library, it won't provide methods for scanning/signature or dumping RAW memory.
 
 **UNDERHOOD WORKING** : _GTLib**Py**_ is actually a wrapper module over [GTLibc](https://github.com/haseeb-heaven/GTLibc) which actually does all the work beneath,this module just converts _Python_ **datatypes,data-structures** to _C-Type_ **data** and passes them to **GTLibc** library and shows result afterwards.
So this has all the features which **GTLibc** had _FindGame,ReadAddress,WriteAddress,SetCheatCodes_ etc.

**AIM** : The aim of this library is only to provide the most efficient way of creating game trainer 
and to provide a layer on top of **WIN-32 API** _cumbersome_ methods and to make reading/writing ,finding Game process easier and convenient.

## **_Your support is needed to keep this project alive, Feel free to donate._**
[![paypal](https://www.payumoney.com/media/images/payby_payumoney/new_buttons/21.png)](https://www.payumoney.com/paybypayumoney/#/C90A30D6E23A691F68F707F3D1D17BBD)

# Main Components :

## Finding game : 

Using **GT_FindGameProcess()** method.

![finding_game_process](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/finding_game_process.jpg?raw=true "")


Using **GT_FindGameWindow()** method.

![finding_game_window](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/finding_game_window.jpg?raw=true "")


## Reading Values : 

using **GT_ReadAddress()** or **GT_ReadAddressoffset()** methods.

![reading_memory](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/reading_memory.jpg?raw=true "")

## Writing Values : 

using **GT_WriteAddress()** or **GT_WriteAddressOffset()** methods.

![writing_memory](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/writing_memory.jpg?raw=true "")

## Creating Hot-keys :

using **GT_HotKeysPressed()** **_MACRO_** or **GT_IsKeyPressed()/GT_IsKeyToggled()** methods.

![hotkeys](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/hotkeys.jpg?raw=true "")

# Additional Components :

## Applying cheat codes : 

using **GT_SetCheatCode()** method.

![set_cheat_code](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/set_cheat_code.jpg?raw=true "")

## Searching offset area : 

using **GT_SearchOffsetArea()** method.

![search_offset_area](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/search_offset_area.jpg?raw=true "")


## Automation scripting  : 

using **GT_DoMousePress()** and **GT_DoKeyPress()** methods.


# GTLibPy Logs and errors :

## Error/Exception Handling :

All the error/exception handling is done by library itself like if you tried read or write from **Invalid Memory section** or if process id,game handle/HWND are invalid  it will automatically handle error.So you don't have to check for any error by yourself

![game_not_found](https://github.com/haseeb-heaven/GTLibc/blob/master/resources/game_not_found.jpg?raw=true "")


![reading_invalid_memory](https://github.com/haseeb-heaven/GTLibc/blob/master/resources/reading_invalid_memory.jpg?raw=true "")


![writing_invalid_memory](https://github.com/haseeb-heaven/GTLibc/blob/master/resources/writing_invalid_memory.jpg?raw=true "")


## Methods Accessibility :

All **Public** and **Semi-Public** methods are accessible . But **Private** methods are not and library will throw error if you tried to access them.

![private_method_error](https://github.com/haseeb-heaven/GTLibc/blob/master/resources/private_method_error.jpg?raw=true "")

## Library Logs :

Logs are **disabled** by default but if you want library to maintain logs use **GT_EnableLogs()** method to **enable** logs.
or if you want to **disable** logs again you can use **GT_DisableLogs()** method.

![enable_disable_logs](https://github.com/haseeb-heaven/GTLibPy/blob/master/resources/enable_disable_logs.jpg?raw=true "")


# Trainer Demo :
As a demo of this module IGI 1 Trainer is included to show demo of all the **GT**LiPy methods and how to use them in making simple game trainer.

# GTLibPy Tutorial on YouTube :
[![GTLibPy Demo](https://img.youtube.com/vi/uOsQ0Yna6zs/0.jpg)](https://www.youtube.com/watch?v=uOsQ0Yna6zs)

# Download from PIP : [GTLibPy](https://pypi.org/project/GT-LibPy/)

**DOCUMENTATION INFO :**
All Public and Semi-Private methods are well documented.
but private methods are not documented as it was not necessary to do so.

**VERSION INFO :**<br/>
GTLibPy Version : V 1.0<br/>  
Dated : 31/05/2019.<br/>

GTLibPy Version : V 1.1<br/>  

**Changelogs**
* Added support for **64bit** games.<br/>
* Added folder for both 32 and 64 bit games in **GTLibcs** <br/>

**Using for 32 and 64 bit games.**
**GTLibcs** containts two file <br/>
* **GTLibc_x86.so** for 32 bit. <br/>
* **GTLibc_x64.so** for 64 bit. <br/>
Just copy the file you need and rename it to **GTLibc.so** and place it in root directory and replace old file with your new file and you are done.</br>

# FAQ </br>
**_Q_** : I am getting this error **OSError: [WinError 193] %1 is not a valid Win32 application** ?</br>
**_A_** : The error states that you are using **32-bit application** but GTLIbPy is **64bit** so use 64bit version of Python.</br>

**_Q_** : When i try to import it to python it says there is no module named **GT_LibPy** ?</br>
**_A_** : Download GTLibPy from Github and place it in your source root directory because pip is not updated.</br>


Dated : 20/05/2020.<br/>
