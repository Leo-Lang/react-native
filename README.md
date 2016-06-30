# React Native Rokid Module

## Introduction

  为Rokid定制的react native版本

## Installation

```
npm i --save react-native-rokid-module
```
**on Android:**

####1. `android/settings.gradle`:: Add the following snippet

```
include ':RNFA',':react-native-rokid-module'
project(':react-native-rokid-module').projectDir = new File(rootProject.projectDir,'../node_modules/react-native-rokid-module/ReactAndroid')
```
####2. `android/app/build.gradle`: Add in dependencies block.

```
//  compile 'com.facebook.react:react-native:+'
    compile project(':react-native-rokid-module')
```

####3. `android/local.properties`.
```
ndk.dir=指向android ndk目录的绝对路径
```

####4. `android/build.gradle`: Add in dependencies block.

```
 //添加gradle-download-task依赖
 dependencies {
        classpath 'com.android.tools.build:gradle:2.1.0'
        classpath 'de.undercouch:gradle-download-task:2.0.0'
        // NOTE: Do not place your application dependencies here; they belong
        // in the individual module build.gradle files
    }
```


