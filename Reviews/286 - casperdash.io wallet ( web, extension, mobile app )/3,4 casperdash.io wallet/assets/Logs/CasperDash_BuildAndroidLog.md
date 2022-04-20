# Casper Dash build and test information logging
## Build log for IOS
### Command: 

```
yarn android
```

### Result:
 
 ```
yarn run v1.22.17
$ react-native run-android
warn Package d3-shape has been ignored because it contains invalid configuration. Reason: Package subpath './package.json' is not defined by "exports" in /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/d3-shape/package.json
info Running jetifier to migrate libraries to AndroidX. You can disable it using "--no-jetifier" flag.
Jetifier found 1701 file(s) to forward-jetify. Using 8 workers...
info JS server already running.
info Installing the app...
Starting a Gradle Daemon (subsequent builds will be faster)

> Configure project :react-native-orientation
> WARNING:: Configuration 'compile' is obsolete and has been replaced with 'implementation' and 'api'.
> It will be removed in version 7.0 of the Android Gradle plugin.
> For more information, see http://d.android.com/r/tools/update-dependency-configurations.html.

> Task :app:installDebug
> Installing APK 'CasperDash-debug.apk' on 'Pixel_2_API_31(AVD) - 12' for app:debug
> Installed on 1 device.

Deprecated Gradle features were used in this build, making it incompatible with Gradle 7.0.
Use '--warning-mode all' to show the individual deprecation warnings.
See https://docs.gradle.org/6.9/userguide/command_line_interface.html#sec:command_line_warnings

BUILD SUCCESSFUL in 44s
581 actionable tasks: 2 executed, 579 up-to-date
info Connecting to the development server...
8081
info Starting the app on "emulator-5554"...
Starting: Intent { cmp=io.casperdash.casperwallet/.MainActivity }
✨ Done in 52.50s.
 ```
