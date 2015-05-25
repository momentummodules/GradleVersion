# Versioning
Simple gradle scripts for android build versioning. It generates a
unified versionCode and versionName.

## Installation
Simply add this script to your build.gradle with this command

```apply from: 'https://raw.githubusercontent.com/momentummodules/Versioning/master/version.gradle'```

Then override (insert) the 3 version values globally

```versionMajor = 0
versionMinor = 0
versionPatch = 10```

Finally apply the 2 functions like this in your defaultConfig

```
...
versionCode genVersionCode()
versionName genVersionName()
...
```