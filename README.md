# Converts macOS keybindings to Microsoft Remote Desktop

I forked this from the orignal repository because the key mappings there were wrong. All else remains the same.

## What this repository for?

When connecting to Linux from MacOs Microsoft Remote Desktop transforms CMD key to Windows key.
This is not usefull, when you want to have remote Intelliji IDEA with standart bindings.
This file helps transform CMD key to Cntrl so you haven't change default key layout in IDE or change modifier keys in mac preferences

## How to setup?

1. Copy file  `ClipboardActionTransformations.xml` file into `/Applications/Microsoft\ Remote\ Desktop.app/Contents/Resources/Keyboard/` (requires sudo). You may use the following command:

```{bash}
sudo cp ClipboardActionTransformations.xml /Applications/Microsoft\ Remote\ Desktop.app/Contents/Resources/Keyboard
```

3. Restart `Microsoft Remote Desktop` app
4. Open `Microsoft Remote Desktop` prefereces and check `Use Mac shortcuts for copy, cut, paste and select all, undo and find`
5. Connect to your remote machine, now all shortcuts with `CMD+` transformed to `Cntrl+` shortcuts


![Screenshot 2022-01-20 at 15 05 36](https://user-images.githubusercontent.com/1608994/150335678-91a0b0e5-27f7-41e1-8c97-2859defa59c1.png)
