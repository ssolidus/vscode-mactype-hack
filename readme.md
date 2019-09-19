# MacType VSCode hack
**__UPDATE__**: The latest version of MacType supports DirectWrite, so you don't need this guide anymore.

## For versions 1.16.1 and above
### Mactype
- Download and install [Mactype](http://mactype.net/).
- Download and install [MactypePatch](https://silightblog.develuck.com/MacTypePatch_1.26.zip), from the user **silight**. This patches MacType to also intercept DirectWrite hooks.

The blog can be found [here](https://silight.hatenablog.jp/entry/MacTypePatch).


## For versions beloe 1.16.1
**This guide no longer works as of `vscode-1.18.0` due to the latest version of Chromium dropping support for the `--disable-directwrite` flag. Consider switching to Sublime Text or not updating**


This guide works as of `mactype-1.2017.628.0` and `vscode-1.16.1`, both on `x64`.


## Flags
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
        
