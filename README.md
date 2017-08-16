
# react-native-bubbles-react-bridge

## Getting started

`$ npm i @the-bubbles-company/bubbles-react-native-bridge -S`

### Mostly automatic installation

`$ react-native link @the-bubbles-company/bubbles-react-native-bridge`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `@the-bubbles-company/bubbles-react-native-bridge` and add `RNBubblesReactBridge.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNBubblesReactBridge.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNBubblesReactBridgePackage;` to the imports at the top of the file
  - Add `new RNBubblesReactBridgePackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-bubbles-react-bridge'
  	project(':react-native-bubbles-react-bridge').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-bubbles-react-bridge/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-bubbles-react-bridge')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNBubblesReactBridge.sln` in `node_modules/@the-bubbles-company/bubbles-react-native-bridge/windows/RNBubblesReactBridge.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Com.Reactlibrary.RNBubblesReactBridge;` to the usings at the top of the file
  - Add `new RNBubblesReactBridgePackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNBubblesReactBridge from '@the-bubbles-company/bubbles-react-native-bridge';

// TODO: What to do with the module?
RNBubblesReactBridge;
```
  