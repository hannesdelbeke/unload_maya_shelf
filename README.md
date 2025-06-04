# Maya unload shelf
To remove a shelf in Autodesk Maya, you can use Maya's `deleteShelf` command. But this changes the original shelf file.  
This script let's you simply unload a shelf, without changing the original shelf file.


## Installation
place script in 
```
C:\Program Files\Autodesk\Maya2019\scripts\others
```
or include in your scriptpath

## Usage
call using mel script
```javascript
unloadShelfTab("my_shelf_name");
```

## Note

- No confirm dialogue for easier use in scripting.
- Adapted from the `deleteShelfTab` function.  
  To allow easy diff in case of future updates I simply commented out the changes in code. See [diff](https://github.com/hannesdelbeke/unload_maya_shelf/commit/20c5063494d2657a2165a90a257423204a15769a)
- Unloading a shelf won't be remembered in the next Maya session, if you auto load the shelf on startup (e.g. shelves in the shelves folder). The `unloadShelfTab` command is meant to be used together with `loadNewShelf` command, so you can load and unload shelves in a maya session
