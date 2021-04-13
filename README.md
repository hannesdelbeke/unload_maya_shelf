# Maya unload shelf

Unload a shelf in Autodesk Maya, without changing the original shelf file.
No confirm dialogue for easier use in scripting.
Adapted from the deleteShelfTab function.
To allow easy diff in case of future updates I simply commented out the changes in code.

## Installation
place script in 
```
C:\Program Files\Autodesk\Maya2019\scripts\others
```
or include in your scriptpath

## Usage
call using mel script
```
unloadShelfTab("my_shelf_name");
```

## Note

If your shelf is not manually loaded, but in a shelves folder that is auto loaded on maya startup, your shelf will reappear when restarting maya.
