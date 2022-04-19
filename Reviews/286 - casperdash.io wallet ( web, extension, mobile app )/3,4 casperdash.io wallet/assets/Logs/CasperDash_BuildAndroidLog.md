# Casper Dash build and test information logging
## Build log for IOS
### Command: 

```
yarn android
```

### Result:
 
 ```
➜ yarn android
yarn run v1.22.17
$ react-native run-android
warn Package d3-shape has been ignored because it contains invalid configuration. Reason: Package subpath './package.json' is not defined by "exports" in /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/d3-shape/package.json
info Running jetifier to migrate libraries to AndroidX. You can disable it using "--no-jetifier" flag.
Jetifier found 1433 file(s) to forward-jetify. Using 8 workers...
info JS server already running.
* daemon not running; starting now at tcp:5037
* daemon started successfully
info Installing the app...
Starting a Gradle Daemon (subsequent builds will be faster)

> Configure project :react-native-orientation
WARNING:: Configuration 'compile' is obsolete and has been replaced with 'implementation' and 'api'.
It will be removed in version 7.0 of the Android Gradle plugin.
For more information, see http://d.android.com/r/tools/update-dependency-configurations.html.

> Task :react-native-async-storage_async-storage:compileDebugJavaWithJavac

> Task :react-native-background-timer:compileDebugJavaWithJavac

> Task :react-native-clipboard_clipboard:compileDebugJavaWithJavac

> Task :react-native-community_cameraroll:compileDebugJavaWithJavac

> Task :react-native-community_datetimepicker:compileDebugJavaWithJavac

> Task :react-native-device-info:compileDebugJavaWithJavac

> Task :react-native-fast-image:compileDebugJavaWithJavac

> Task :react-native-gesture-handler:compileDebugJavaWithJavac

> Task :react-native-image-base64:compileDebugJavaWithJavac

> Task :react-native-image-crop-picker:compileDebugJavaWithJavac

> Task :react-native-localize:compileDebugJavaWithJavac

> Task :react-native-pager-view:compileDebugKotlin
w: Runtime JAR files in the classpath should have the same version. These files were found in the classpath:
    /Users/gaupoit/.gradle/caches/transforms-3/f28135687ec29fd0a9846d3bbfa908d2/transformed/jetified-kotlin-stdlib-jdk8-1.4.10.jar (version 1.4)
    /Users/gaupoit/.gradle/caches/transforms-3/91321da7bd0dc1f16cd547b731b3e152/transformed/jetified-kotlin-stdlib-jdk7-1.4.10.jar (version 1.4)
    /Users/gaupoit/.gradle/caches/transforms-3/435f5819f484e16ea4c54ebd068bb213/transformed/jetified-kotlin-stdlib-1.5.30.jar (version 1.5)
    /Users/gaupoit/.gradle/caches/transforms-3/5b951b31dd76ab96e00ac91b57666444/transformed/jetified-kotlin-stdlib-common-1.5.30.jar (version 1.5)
w: Some runtime JAR files in the classpath have an incompatible version. Consider removing them from the classpath
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/PagerViewViewManager.kt: (215, 11): 'receiveCommand(T, Int, ReadableArray?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollEvent.kt: (6, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollEvent.kt: (21, 82): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollEvent.kt: (27, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollEvent.kt: (28, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollStateChangedEvent.kt: (6, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollStateChangedEvent.kt: (15, 89): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollStateChangedEvent.kt: (20, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageScrollStateChangedEvent.kt: (21, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageSelectedEvent.kt: (6, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageSelectedEvent.kt: (15, 69): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageSelectedEvent.kt: (20, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-pager-view/android/src/main/java/com/reactnativepagerview/event/PageSelectedEvent.kt: (21, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java

> Task :react-native-orientation:compileDebugJavaWithJavac

> Task :react-native-push-notification:compileDebugJavaWithJavac

> Task :react-native-safe-area-context:compileDebugJavaWithJavac
<========-----> 66% EXECUTING [1m 37s]
> IDLE
> IDLE
> IDLE
> IDLE
> IDLE
> IDLE
> :react-native-screens:compileDebugKotlin
> IDLE
....
> Task :react-native-sensitive-info:compileDebugJavaWithJavac

> Task :react-native-share:compileDebugJavaWithJavac

> Task :react-native-svg:compileDebugJavaWithJavac

> Task :react-native-video:compileDebugJavaWithJavac

> Task :react-native-webview:compileDebugKotlin
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopHttpErrorEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopHttpErrorEvent.kt: (11, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopHttpErrorEvent.kt: (22, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopHttpErrorEvent.kt: (23, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingErrorEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingErrorEvent.kt: (11, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingErrorEvent.kt: (22, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingErrorEvent.kt: (23, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingFinishEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingFinishEvent.kt: (11, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingFinishEvent.kt: (22, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingFinishEvent.kt: (23, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingProgressEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingProgressEvent.kt: (11, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingProgressEvent.kt: (22, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingProgressEvent.kt: (23, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingStartEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingStartEvent.kt: (11, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingStartEvent.kt: (22, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopLoadingStartEvent.kt: (23, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopMessageEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopMessageEvent.kt: (10, 75): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopMessageEvent.kt: (21, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopMessageEvent.kt: (22, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopRenderProcessGoneEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopRenderProcessGoneEvent.kt: (12, 3): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopRenderProcessGoneEvent.kt: (23, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopRenderProcessGoneEvent.kt: (24, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopShouldStartLoadWithRequestEvent.kt: (5, 44): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopShouldStartLoadWithRequestEvent.kt: (10, 89): 'constructor Event<T : Event<(raw) Event<*>>!>(Int)' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopShouldStartLoadWithRequestEvent.kt: (27, 42): 'RCTEventEmitter' is deprecated. Deprecated in Java
w: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/events/TopShouldStartLoadWithRequestEvent.kt: (28, 21): 'receiveEvent(Int, String!, WritableMap?): Unit' is deprecated. Deprecated in Java

> Task :react-native-webview:compileDebugJavaWithJavac

> Task :rn-fetch-blob:compileDebugJavaWithJavac

> Task :app:compileDebugJavaWithJavac

> Task :app:stripDebugDebugSymbols
Unable to strip the following libraries, packaging them as they are: libbetter.so, libc++_shared.so, libevent-2.1.so, libevent_core-2.1.so, libevent_extra-2.1.so, libfabricjni.so, libfb.so, libfbjni.so, libflipper.so, libfolly_futures.so, libfolly_json.so, libglog.so, libglog_init.so, libhermes-executor-common-debug.so, libhermes-executor-common-release.so, libhermes-executor-debug.so, libhermes-executor-release.so, libhermes-inspector.so, libimagepipeline.so, libjsc.so, libjscexecutor.so, libjsi.so, libjsijniprofiler.so, libjsinspector.so, liblogger.so, libmapbufferjni.so, libnative-filters.so, libnative-imagetranscoder.so, libreact_codegen_rncore.so, libreact_debug.so, libreact_nativemodule_core.so, libreact_render_animations.so, libreact_render_attributedstring.so, libreact_render_componentregistry.so, libreact_render_core.so, libreact_render_debug.so, libreact_render_graphics.so, libreact_render_imagemanager.so, libreact_render_leakchecker.so, libreact_render_mapbuffer.so, libreact_render_mounting.so, libreact_render_runtimescheduler.so, libreact_render_scheduler.so, libreact_render_telemetry.so, libreact_render_templateprocessor.so, libreact_render_textlayoutmanager.so, libreact_render_uimanager.so, libreact_utils.so, libreactconfig.so, libreactnativeblob.so, libreactnativejni.so, libreactnativeutilsjni.so, libreactperfloggerjni.so, libreanimated.so, librrc_image.so, librrc_modal.so, librrc_progressbar.so, librrc_root.so, librrc_scrollview.so, librrc_slider.so, librrc_switch.so, librrc_text.so, librrc_textinput.so, librrc_unimplementedview.so, librrc_view.so, libturbomodulejsijni.so, libucrop.so, libyoga.so.

> Task :app:installDebug FAILED
w: Detected multiple Kotlin daemon sessions at build/kotlin/sessions

Deprecated Gradle features were used in this build, making it incompatible with Gradle 7.0.
Use '--warning-mode all' to show the individual deprecation warnings.
See https://docs.gradle.org/6.9/userguide/command_line_interface.html#sec:command_line_warnings
581 actionable tasks: 581 executed
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-async-storage/async-storage/android/src/main/java/com/reactnativecommunity/asyncstorage/AsyncStorageModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-async-storage/async-storage/android/src/main/java/com/reactnativecommunity/asyncstorage/AsyncStoragePackage.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-background-timer/android/src/main/java/com/ocetnik/timer/BackgroundTimerModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-clipboard/clipboard/android/src/main/java/com/reactnativecommunity/clipboard/ClipboardModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-community/cameraroll/android/src/main/java/com/reactnativecommunity/cameraroll/CameraRollModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: [2] Wrote GeneratedAppGlideModule with: [com.bumptech.glide.integration.okhttp3.OkHttpLibraryGlideModule, com.dylanvann.fastimage.FastImageOkHttpProgressGlideModule]
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-base64/android/src/main/java/fr/snapp/imagebase64/RNImgToBase64Module.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-localize/android/src/main/java/com/zoontek/rnlocalize/RNLocalizeModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-orientation/android/src/main/java/com/github/yamill/orientation/OrientationModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-push-notification/android/src/main/java/com/dieam/reactnativepushnotification/modules/RNPushNotification.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-sensitive-info/android/src/main/java/br/com/classapp/RNSensitiveInfo/RNSensitiveInfoModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-share/android/src/main/java/cl/json/RNSharePathUtil.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-svg/android/src/main/java/com/horcrux/svg/VirtualView.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-video/android/src/main/java/com/brentvatne/react/ReactVideoViewManager.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/RNCWebViewManager.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/android/app/src/debug/java/com/monoly/ReactNativeFlipper.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':app:installDebug'.
> com.android.builder.testing.api.DeviceException: No connected devices!

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output. Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 2m 30s

error Failed to install the app. Make sure you have an Android emulator running or a device connected.
Error: Command failed: ./gradlew app:installDebug -PreactNativeDevServerPort=8081
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-async-storage/async-storage/android/src/main/java/com/reactnativecommunity/asyncstorage/AsyncStorageModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-async-storage/async-storage/android/src/main/java/com/reactnativecommunity/asyncstorage/AsyncStoragePackage.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-background-timer/android/src/main/java/com/ocetnik/timer/BackgroundTimerModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-clipboard/clipboard/android/src/main/java/com/reactnativecommunity/clipboard/ClipboardModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/@react-native-community/cameraroll/android/src/main/java/com/reactnativecommunity/cameraroll/CameraRollModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: [2] Wrote GeneratedAppGlideModule with: [com.bumptech.glide.integration.okhttp3.OkHttpLibraryGlideModule, com.dylanvann.fastimage.FastImageOkHttpProgressGlideModule]
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-base64/android/src/main/java/fr/snapp/imagebase64/RNImgToBase64Module.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-localize/android/src/main/java/com/zoontek/rnlocalize/RNLocalizeModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-orientation/android/src/main/java/com/github/yamill/orientation/OrientationModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-push-notification/android/src/main/java/com/dieam/reactnativepushnotification/modules/RNPushNotification.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-sensitive-info/android/src/main/java/br/com/classapp/RNSensitiveInfo/RNSensitiveInfoModule.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-share/android/src/main/java/cl/json/RNSharePathUtil.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-svg/android/src/main/java/com/horcrux/svg/VirtualView.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-video/android/src/main/java/com/brentvatne/react/ReactVideoViewManager.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-webview/android/src/main/java/com/reactnativecommunity/webview/RNCWebViewManager.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/android/app/src/debug/java/com/monoly/ReactNativeFlipper.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
...
success Successfully launched the app on the simulator
✨  Done in 2m 30s.
 ```
