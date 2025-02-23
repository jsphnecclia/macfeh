# macfeh

![Screenshot](https://raw.githubusercontent.com/DrabWeb/macfeh/master/screenshot.png)

Like feh, but on macOS

* Commented out aspect ratio line to play better with tiling wm
* Set up a cute lil' icon

## Requirements
macOS 10.11+ (tested on 10.12)


## Features
* Borderless rounded viewer
* Zoom and scroll
* Toggle viewer background/shadows
* Command line support

## Compiling
* **Requirements**: Xcode 9
* Open `macfeh.xcodeproj` in Xcode.
* Select the `macfeh Release` scheme from the pop up button in the top left.
* Press the Run button, macfeh will compile and launch.
* Once launched, ⌘+left click the macfeh icon in the dock.
* Finder will show and select `macfeh.app` which you can now copy to your `/Applications/` folder or other.

## Command line
To use macfeh from the command line, add 

```bash
function macfeh() {
    open -b "drabweb.macfeh" "$@"
}
```

to your shell rc, and use `macfeh [file1] [file2] [file3]...`
