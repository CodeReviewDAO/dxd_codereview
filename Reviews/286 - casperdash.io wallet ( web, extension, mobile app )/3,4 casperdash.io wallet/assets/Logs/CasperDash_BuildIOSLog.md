# Casper Dash build and test information logging
## Build log for IOS
### Command: 

```
yarn ios
```

### Result:
 
 ```
yarn run v1.22.17
$ react-native run-ios
warn Package d3-shape has been ignored because it contains invalid configuration. Reason: Package subpath './package.json' is not defined by "exports" in /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/d3-shape/package.json
error React Native CLI uses autolinking for native dependencies, but the following modules are linked manually:
  - react-native-ble-plx (to unlink run: "react-native unlink react-native-ble-plx")
  - react-native-splash-screen (to unlink run: "react-native unlink react-native-splash-screen")
  - react-native-vector-icons (to unlink run: "react-native unlink react-native-vector-icons")
This is likely happening when upgrading React Native from below 0.60 to 0.60 or above. Going forward, you can unlink this dependency via "react-native unlink <dependency>" and it will be included in your app automatically. If a library isn't compatible with autolinking, disregard this message and notify the library maintainers.
Read more about autolinking: https://github.com/react-native-community/cli/blob/master/docs/autolinking.md
info Found Xcode workspace "CasperDash.xcworkspace"
info Launching iPhone 13 (iOS 15.2)
info Building (using "xcodebuild -workspace CasperDash.xcworkspace -configuration Debug -scheme CasperDash -destination id=61469768-10B6-42B0-9601-5C794CD118AF")
....
▸ Compiling TurboModuleUtils.cpp
▸ Compiling TurboModulePerfLogger.cpp
▸ Compiling TurboModuleBinding.cpp
▸ Compiling TurboModule.cpp
▸ Compiling TurboCxxModule.cpp
▸ Compiling ReactCommon-dummy.m
▸ Compiling RCTTurboModuleManager.mm
▸ Building library libYogaKit.a
▸ Compiling RCTTurboModule.mm
▸ Compiling RCTBlockGuard.mm
▸ Compiling LongLivedObject.cpp
▸ Running script 'Copy generated compatibility header'
▸ Compiling React-RCTText-dummy.m
▸ Compiling RCTVirtualTextViewManager.m
▸ Compiling RCTVirtualTextShadowView.m
▸ Compiling RCTUITextView.m
▸ Compiling RCTUITextField.m
▸ Compiling RCTTextViewManager.m
▸ Compiling RCTTextView.m
▸ Compiling RCTTextShadowView.m
▸ Compiling RCTTextSelection.m
▸ Compiling RCTTextAttributes.m
▸ Compiling RCTSinglelineTextInputViewManager.m
▸ Compiling RCTSinglelineTextInputView.m
▸ Compiling RCTRawTextViewManager.m
▸ Compiling RCTRawTextShadowView.m
▸ Compiling RCTMultilineTextInputViewManager.m
▸ Compiling RCTMultilineTextInputView.m
▸ Compiling RCTInputAccessoryViewManager.m
▸ Compiling RCTInputAccessoryViewContent.m
▸ Compiling RCTInputAccessoryView.m
▸ Compiling RCTInputAccessoryShadowView.m
▸ Compiling RCTConvert+Text.m
▸ Compiling RCTBaseTextViewManager.m
▸ Compiling RCTBaseTextShadowView.m
▸ Compiling RCTBaseTextInputViewManager.m
▸ Compiling RCTBaseTextInputView.m
▸ Compiling RCTBaseTextInputShadowView.m
▸ Compiling RCTBackedTextInputDelegateAdapter.m
▸ Compiling NSTextStorage+FontScaling.m
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/zh-Hant.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/zh-Hans.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/uk.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/tr.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/sv.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/ru.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/ro.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/pt.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/pl.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/ko.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/ja.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/it.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/fr.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/es.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/en.lproj
▸ Copying /Volumes/Samsung\ SSD\ 860\ EVO\ Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/node_modules/react-native-image-crop-picker/ios/QBImagePicker/QBImagePicker/de.lproj
▸ Compiling QBImagePicker.storyboard
▸ Compiling json_pointer.cpp
▸ Compiling json.cpp
▸ Compiling dynamic.cpp

⚠️  /Volumes/Samsung SSD 860 EVO Media/Workspace/casperdash/blockchain/casperdash-mobile-wallet/ios/Pods/RCT-Folly/folly/dynamic.cpp:475:3: code will never be executed [-Wunreachable-code]

  assume_unreachable();
                                                  ^


▸ Compiling UniqueInstance.cpp
▸ Compiling Unicode.cpp
▸ Compiling ToAscii.cpp
...

▸ Processing Info.plist
▸ Generating 'CasperDash.app.dSYM'
▸ Running script 'Bundle React Native code and images'
▸ Running script '[CP] Embed Pods Frameworks'
▸ Running script '[CP] Copy Pods Resources'
▸ Touching CasperDash.app (in target 'CasperDash' from project 'CasperDash')
▸ Build Succeeded
success Successfully built the app
--- xcodebuild: WARNING: Using the first of multiple matching destinations:
{ platform:iOS Simulator, id:dvtdevice-DVTiOSDeviceSimulatorPlaceholder-iphonesimulator:placeholder, name:Any iOS Simulator Device }
{ platform:iOS Simulator, id:9CD79807-A810-4DCB-95AB-0BE25BBE7BAA, OS:13.7, name:iPhone 8 }
{ platform:iOS Simulator, id:B22D7897-EBB9-4532-8C05-7585699B6800, OS:15.2, name:iPhone 8 }
{ platform:iOS Simulator, id:7D96C136-FFBE-4193-A60B-5225D6E6144F, OS:13.7, name:iPhone 8 Plus }
{ platform:iOS Simulator, id:E98315CE-8994-49A7-A4A7-EE30AAAF1635, OS:15.2, name:iPhone 8 Plus }
{ platform:iOS Simulator, id:4B273284-0BAF-423C-AD18-788541244C4A, OS:13.7, name:iPhone 11 }
{ platform:iOS Simulator, id:FE85556A-FC30-4FA8-B825-B95084B987A1, OS:15.2, name:iPhone 11 }
{ platform:iOS Simulator, id:63EF47DB-1E80-4AC8-AE89-A22DC44CC4EA, OS:13.7, name:iPhone 11 Pro }
{ platform:iOS Simulator, id:C1BEE931-E21D-4EA2-AD3C-50FA2AD00AE1, OS:15.2, name:iPhone 11 Pro }
{ platform:iOS Simulator, id:9FCA6E5F-79AF-477A-9313-B5EA1C07DB43, OS:13.7, name:iPhone 11 Pro Max }
{ platform:iOS Simulator, id:F1C29BA9-93DF-44C0-A83D-8A072B085E59, OS:15.2, name:iPhone 11 Pro Max }
{ platform:iOS Simulator, id:C2FA4AE8-6D09-4DA2-B6DD-3B72952367AE, OS:15.2, name:iPhone 12 }
{ platform:iOS Simulator, id:B50ADF84-CB41-4CB7-AB48-130E2E0DB468, OS:15.2, name:iPhone 12 Pro }
{ platform:iOS Simulator, id:1C482A18-877C-42C6-8D5B-31469F8D055B, OS:15.2, name:iPhone 12 Pro Max }
{ platform:iOS Simulator, id:47F579A7-6716-4C0E-B830-6E69D98FA1CC, OS:15.2, name:iPhone 12 mini }
{ platform:iOS Simulator, id:61469768-10B6-42B0-9601-5C794CD118AF, OS:15.2, name:iPhone 13 }
{ platform:iOS Simulator, id:273CE3B0-E388-40D5-B5DF-FAA345452A5E, OS:15.2, name:iPhone 13 Pro }
{ platform:iOS Simulator, id:B034E458-A212-45CD-A62F-7ED8444E22DB, OS:15.2, name:iPhone 13 Pro Max }
{ platform:iOS Simulator, id:0EBE6E42-01B1-4266-B390-0A28BBEE9C0B, OS:15.2, name:iPhone 13 mini }
{ platform:iOS Simulator, id:F67B0FB1-FFDB-41F5-91CB-253D3C47B4C7, OS:15.2, name:iPod touch (7th generation) }
{ platform:macOS, arch:arm64, variant:Designed for [iPad,iPhone], id:4214BAD4-D5FE-5755-BEDD-1A61D67EECA8 }
{ platform:iOS, id:dvtdevice-DVTiPhonePlaceholder-iphoneos:placeholder, name:Any iOS Device }
info Installing "/Users/gaupoit/Library/Developer/Xcode/DerivedData/CasperDash-atcyjuowmepbthdtsnmjqgtjisuc/Build/Products/Debug-iphonesimulator/CasperDash.app"
info Launching "io.casperdash.casperwallet"
success Successfully launched the app on the simulator
✨  Done in 168.90s.
 ```
