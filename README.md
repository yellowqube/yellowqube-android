<img src="https://i.ibb.co/80ww6wR/Artboard.png">

# Yellow Qube : Chat SDK

Chat Platform

[![][license img]][license]


## Last Version

 - v0.0.1
 
## Installation

 - add to project `build.gradle`
```sh
allprojects {
    repositories {
        .
        .
         maven {
            url  "https://dl.bintray.com/yellowqube/maven"
        }
      .
      .
    }
}
```

 - to use payment add to app `build.gradle`
```sh
    dependencies {
    
         implementation("app.yellowqube:yellowqube-sdk:0.0.1@aar") {
            // excluding org.json which is provided by Android
             exclude group: 'org.json', module: 'json'
         }
         .
         .
    }
```

 - add to Application class
```kotlin
    YellowQube.startInit(this,"[APP_ID]")
```

# License

- http://yellowqube.app



[license]:LICENSE-2.0.txt
[license img]:https://img.shields.io/badge/License-Apache%202-blue.svg
