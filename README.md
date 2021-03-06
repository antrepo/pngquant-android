## pngquant-android

[pngquant](https://pngquant.org/) with basic Java bindings for Android.
![pngquant](https://pngquant.org/pngquant-logo.png)

###Usage:
In your build.gradle:
```groovy
dependencies {
    compile 'com.ndahlquist:pngquant-android:0.2'
}

```

In your Android app:
```java
File inputPngFile = getYourPng();
File outputPngFile = getOutputFile();
new LibPngQuant().pngQuantFile(inputFile, outputFile);
```

###Building:
- This project includes git submodules; please make sure to `git clone --recursive`. Alternatively, `git submodule init; git submodule update`.
- On OS X, please install wget: `brew install wget`.
- From the top-level directory, run `./gradlew installDebug`. This will download all dependencies, build the library, and install a test application to a connected Android device.
