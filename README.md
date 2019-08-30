# gradle-scripts

```
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/kotlin.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/appcompat.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/dagger.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/glide.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/retrofit.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/lifecycle.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/room.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/navigation.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/paging.gradle'
apply from: 'https://raw.githubusercontent.com/MoshDev/gradle-scripts/master/testing.gradle'
```

#Root Build Script

```
buildscript {
    ext.kotlin_version = '1.3.50'
    repositories {
        google()
        jcenter()
        
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:3.5.0'
        classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version"
        //def nav_version = "2.2.0-alpha01" // to enable navigation safe args
        //classpath "androidx.navigation:navigation-safe-args-gradle-plugin:$nav_version"
    }
}
```

# Proguard
 ```
 proguardFiles fileTree('../proguard').asList().toArray()
 ```