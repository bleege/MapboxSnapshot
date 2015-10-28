# MapboxSnapshot
Demo Of Adding Mapbox Android SNAPSHOT To An App

Mapbox for Android SNAPSHOTS are distributed via Maven Central's SNAPSHOT repository.  To include this in an app:


```
// Add Maven Central SNAPSHOT Repository
build.gradle

allprojects {
    repositories {
        jcenter()
        maven { url "http://oss.sonatype.org/content/repositories/snapshots/" }
    }
}

// Add 2.2.0-SNAPSHOT release to app
app/build.gradle

dependencies {
    compile('com.mapbox.mapboxsdk:mapbox-android-sdk:2.2.0-SNAPSHOT@aar') {
        transitive = true
    }
}
```
