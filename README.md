<img src="https://i.ibb.co/wz7mzcF/Artboard.png">

# Yellow Qube : Chat and Messaging Platform

[![][license img]][license]

## Overview

Android Chat SDK / Messaging SDK that lets you add real time chat and in-app messaging in your mobile (android, iOS) applications and website.

## Getting Started

### Step 1 : Add the following in your project build.gradle repositories:
```sh
allprojects {
    repositories {
         maven {
            url  "https://dl.bintray.com/yellowqube/maven"
        }
    }
}
```

### Step 2 : Add the following in your module build.gradle dependencies:
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

### Step 2 : add to Application class
```kotlin
    YellowQube.startInit(this,"[APP_ID]")
```

# License

- http://yellowqube.app



[license]:LICENSE-2.0.txt
[license img]:https://img.shields.io/badge/License-Apache%202-blue.svg
