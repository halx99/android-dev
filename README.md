# android-dev

## ndk-r23 LTS 16K page size support

- https://ci.android.com/builds/submitted/12186248/win64/latest/android-ndk-12186248-windows-x86_64.zip
- https://ci.android.com/builds/submitted/12186248/linux/latest/android-ndk-12186248-linux-x86_64.zip
- https://ci.android.com/builds/submitted/12186248/darwin_mac/latest/android-ndk-12186248-darwin-x86_64.zip

## adt-bundle-windows
https://dl.google.com/android/adt/adt-bundle-windows-x86_64-20140702.zip?utm_source=androiddevtools&utm_medium=website

## android studio
* v4.0.1: https://redirector.gvt1.com/edgedl/android/studio/install/4.0.1.0/android-studio-ide-193.6626763-windows.exe
* archieves: https://developer.android.com/studio/archive  

## gradle(can be install by android-studio)
gradle: https://services.gradle.org/distributions/gradle-{revision}-all.zip  

## build-tools(can be install by android-studio)
build-tools: https://dl.google.com/android/repository/build-tools_r{revision}-windows.zip  

## Android SDK Platform
sdk-platform: https://dl.google.com/android/repository/platform-{num}_r{revision}.zip  

## ndk repos(can be install by android-studio)
* direct links
  - windows: https://dl.google.com/android/repository/android-ndk-{revision}-windows-x86_64.zip  
  - linux: https://dl.google.com/android/repository/android-ndk-{revision}-linux-x86_64.zip  
  - darwin: https://dl.google.com/android/repository/android-ndk-{revision}-darwin-x86_64.zip
* direct links r23+
  - windows: https://dl.google.com/android/repository/android-ndk-{revision}-windows.zip  
  - linux: https://dl.google.com/android/repository/android-ndk-{revision}-linux.zip  
  - darwin: https://dl.google.com/android/repository/android-ndk-{revision}-darwin.zip
* webpage
  - latest: https://developer.android.google.cn/ndk/downloads
  - older: https://developer.android.google.cn/ndk/downloads/older_releases
* googlesource url: https://android.googlesource.com/platform/prebuilts/ndk

## ninja
The cmake in android-studio may contains ninja, if you install cmake by your self,  
you may need download at https://github.com/ninja-build/ninja/releases, and copy to directory of cmake.exe

## gradle plugin(can be install by android-studio)
https://dl.google.com/android/studio/plugins/android-gradle/preview/offline-android-gradle-plugin-preview.zip  

## gmaven offline(can be install by android-studio)
https://dl.google.com/android/studio/maven-google-com/stable/offline-gmaven-stable.zip  

## gradle mirror in china
```gradle
buildscript {
    repositories {
        maven { url 'https://maven.aliyun.com/repository/google/' }
        maven { url 'https://maven.aliyun.com/repository/jcenter/'}
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:4.0.1'

        // NOTE: Do not place your application dependencies here; they belong
        // in the individual module build.gradle files
    }        
}

allprojects {
    repositories {
        maven { url 'https://maven.aliyun.com/repository/google/' }
        maven { url 'https://maven.aliyun.com/repository/jcenter/'}
    }
}
```

## gradle-wrapper.properties
```gradle
distributionBase=GRADLE_USER_HOME
distributionPath=wrapper/dists
zipStoreBase=GRADLE_USER_HOME
zipStorePath=wrapper/dists
distributionUrl=file:///d:/dev/adt/gradle-5.1.1-all.zip
```



