# lightzone-plugin-for-gimp
GIMP LightZone Plug-in for Windows, macOS, and Linux.

Derived from original plugin for Windows:
http://steaz.altervista.org/lightzone-plugin-for-gimp/

# Install
## Windows
Download `Lightzone.py` and place it in `C:\Users\USER_NAME\.gimp-2.8\plug-ins\` folder.

## macOS
```
curl -o ~/Library/Application\ Support/GIMP/2.8/plug-ins/Lightzone.py https://raw.githubusercontent.com/ktgw0316/lightzone-plugin-for-gimp/master/Lightzone.py && chmod 755 ~/Library/Application\ Support/GIMP/2.8/plug-ins/Lightzone.py
```

## Linux
```
curl -o ~/.gimp-2.8/plug-ins/Lightzone.py https://raw.githubusercontent.com/ktgw0316/lightzone-plugin-for-gimp/master/Lightzone.py && chmod 755 ~/.gimp-2.8/plug-ins/Lightzone.py
```

## How to use
1. In Gimp menu, select Filter > Photography > LightZone
1. Select a Layer setting, then click _OK_ to open LightZone
1. (If you haven't done yet) go to LightZone Preferences > Save, then
  - Select _Save LightZone files as:_ JPEG
  - Select _Resize To_: Don't limit
1. Edit and Save your image
1. Exit LightZone. Note that you may need to completely quit LightZone using `Ctrl-q` or `Cmd-q` shortcut, especially on macOS.
1. Edited image from LightZone will appeer on the Gimp window.

## Known Issues
- On macOS, it opens another unnecessary LightZone window.
- On macOS, LightZone windows are sometimes in very small size.
- On Gimp 2.9 and later, `pdb.gimp_edit_named_paste_as_new` must be changed to `pdb.gimp_edit_named_paste_as_new_image` to avoid error dialog.
