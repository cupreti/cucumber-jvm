### Prerequisites *(taken from the [maven-android-plugin](https://code.google.com/p/maven-android-plugin) documentation)*

1. JDK 1.6+ installed as required for Android development
2. [Android SDK](http://developer.android.com/sdk/index.html) (r17 or later, latest is best supported) installed, preferably with all platforms.
3. [Maven 3.0.3+](http://maven.apache.org/download.html) installed
4. Set environment variable `ANDROID_HOME` to the path of your installed Android SDK and add `$ANDROID_HOME/tools` as well as `$ANDROID_HOME/platform-tools` to your `$PATH`.

On Windows: use `%ANDROID_HOME%\tools` and `%ANDROID_HOME%\platform-tools` instead.

On OS X: Note that for the path to work on the commandline and in IDE's started by launchd you have to set it in `/etc/launchd.conf` and **NOT** in .bashrc or something else.

The generated target artifacts are an [apklib](https://code.google.com/p/maven-android-plugin/wiki/ApkLib) file and a regular .jar.

Tests are in `../cucumber-test/`.

## Developers

When running the test app, logs can be read with:

```
adb logcat
```
