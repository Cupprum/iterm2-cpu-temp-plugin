# iterm2-cpu-temp-plugin
Display cpu temperature in the status bar of iTerm2

## Based on [osx-cpu-temp](https://github.com/lavoiesl/osx-cpu-temp)

# How to Install

1. Install osx-cpu-temp `brew install osx-cpu-temp`
2. Clone this repository
3. You’ll need to place the script in ~/Library/Application Support/iTerm2/Scripts/AutoLaunch. 
4. Then manually launch it or restart the app.
5. Then, navigate to Preferences > Profiles > Session. Turn on Status Bar Enabled and select Configure Status Bar. Drag the 🌡x°C component into the bottom section.

# Customisation

You can change the unit into Farenheit by editing the 
```
output = check_output(["/usr/local/bin/osx-cpu-temp"])
```
 by 
 ```
 output = check_output(["/usr/local/bin/osx-cpu-temp"],["-F])
 ```