# Yellow Qube

Chat Platform


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
```
    YellowQube.startInit(this,"[APP_ID]")
```

# License

- http://yellowqube.app
