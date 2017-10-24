# MacType VSCode hack
## Flags
This guide works as of `mactype-1.2017.628.0` and `vscode-1.16.1`, both on `x64`.

Mactype can be found [here](https://github.com/snowie2000/mactype).

VSCode requires the following flags to be passed for MacType to work correctly:

```
--disable-lcd-text
--disable-gpu
--disable-directwrite-for-ui
--disable-font-antialiasing
```
You can pass these in two ways.
## Shortcut
Add them to the shortcut, like this:

![shortcut window](https://vgy.me/M2mRG7.png)
## Inside the `settings.json`
Add the settings to your `settings.json` file. 

Inside this repository is a copy of my user-specific `settings.json` with the require flags.
        
