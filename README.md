# Versioning
Simple gradle scripts for android build versioning

This script helps creating a unified versionCode and versionName
Timply add this script to your build.gradle with this command

```apply from: 'X:/gradle/version.gradle'```

Then override the 3 version values globally

```versionMajor = 0
versionMinor = 0
versionPatch = 10```

Finally apply the 2 functions like this

```...
versionCode genVersionCode()
versionName genVersionName()
...```