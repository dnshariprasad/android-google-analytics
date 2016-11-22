# Google Analytics


#### Stept 1 :

Update project's AndroidManifest.xml file to include the INTERNET and ACCESS_NETWORK_STATE permissions.

```
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
```

#### Step 2 :

Update project and module level build.gradle files with required dependencies.

1 . Add the dependency to your project-level build.gradle:
```
classpath 'com.google.gms:google-services:3.0.0'
```
2 . Add the plugin to the bottom of your app-level build.gradle:
```
apply plugin: 'com.google.gms.google-services'
```
3 . Now, you need to add a dependency for Google Play Services. Inside your app's build.gradle add:
```
compile 'com.google.android.gms:play-services-analytics:9.2.0'
```

#### Step 3 :

Get a configuration file (google-services.json) and put in corresponding module.

#### Step 4 :

Add screen tracking.

---
#### References : 

* [Googl Developers Site](https://developers.google.com/analytics/devguides/collection/android/v4/)

