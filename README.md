
# Gravite Plugin for BackFill in Yieldlove AdIntegration SDK 


**Version:** 0.1.0

  

This repository contains the **Gravite Plugin** for **Backfill** in the **Yieldlove AdIntegration SDK**.

  

•  **Compatibility**: This plugin is compatible with **Yieldlove AdIntegration version 6.22.0** and above.


The Gravite Plugin enhances the functionality of the Yieldlove AdIntegration SDK by enabling backfill support, ensuring optimized ad delivery and monetization.

  
## How to integrate the Gravite Plugin.


### How to set up in a 'build.gradle' file.

```gradle
repositories {
    // Yieldlove Ad Integration repository
    maven {
        url 'https://slabs-yieldlove-ad-integration.s3.eu-central-1.amazonaws.com/android'
    }
    
    // GitHub repository for StroeerAdSDK-GravitePlugin (raw content)
    maven {
        url 'https://github.com/mbrtargeting/StroeerAdSDK-GravitePlugin/raw/main'
    }
    
    // AATKit SDK repository
    maven {
        url 'https://android-sdk.aatkit.com/maven/'
    }
    
    // Smaato SDK repository
    maven {
        url "https://s3.amazonaws.com/smaato-sdk-releases/"
    }
    
    // SmartAdServer repository
    maven {
        url 'https://packagecloud.io/smartadserver/android/maven2'
    }
    
    // PubNative repository (Verve)
    maven {
        url 'https://verve.jfrog.io/artifactory/verve-gradle-release'
    }
    
    // ironSource repository
    maven {
        url 'https://android-sdk.is.com/'
    }
    
    // Ogury repository
    maven {
        url 'https://maven.ogury.co'
    }
    
    // GraviteRTB repository
    maven {
        url 'https://android-sdk-rtb.gravite.net/maven'
    }
    
    // Mintegral repository
    maven {
        url "https://dl-maven-android.mintegral.com/repository/mbridge_android_sdk_oversea"
    }
    
    // Google Maven repository (Android dependencies)
    google()
    
    // Maven Central repository
    mavenCentral()
}

dependencies {
    // Gravite Plugin from Stroeer Backfill
    implementation 'com.stroeer.backfill:graviteplugin:0.1.0'
}
```


### How to Set Up in Your Application
```Java
// [ApplicationName]: ApplicationName
// BackFillSetting.enabled
// this: The current activity
Yieldlove.setup("[ApplicationName]", BackFillSetting.enabled, this);
