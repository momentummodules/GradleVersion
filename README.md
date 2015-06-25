# Versioning
Simple gradle scripts for android build versioning. It generates a
unified versionCode and versionName.

It supports up to 100 minor versions per major version and 1000 patch versions per minor version.

## Installation
Simply add this script to your build.gradle with this command

```Gradle
apply from: 'https://raw.githubusercontent.com/momentummodules/Versioning/master/version.gradle'
```

Then override (insert) the 3 version values globally

```Gradle
versionMajor = 0
versionMinor = 0
versionPatch = 10
```

Finally apply the 2 functions like this in your defaultConfig

```Gradle
...
versionCode genVersionCode()
versionName genVersionName()
...
```