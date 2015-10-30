#ViewServer

ViewServer enables [HierarchyViewer](http://developer.android.com/tools/debugging/debugging-ui.html#HierarchyViewer) inspection tool in your application, on any device.

It's a very lighweight, simple class.

##Setup
First, check that your app has INTERNET permission in `AndroidManifest.xml`
```xml

<manifest ...>
    <uses-permission android:name="android.permission.INTERNET"/>
    ...
</manifest>
```
This permission is needed to let ViewServer communicate through adb with HierarchyViewer.

Then, add [ViewServer.java](https://github.com/romainguy/ViewServer/blob/master/viewserver/src/main/java/com/android/debug/hv/ViewServer.java) to your app project.
If you use [AndroidAnnotations](http://androidannotations.org), this class is already included in the library, and you can use it on Enhanced Activities. However, the AA version, isn't up to date for now (but is working), so you may want to use this version until [this issue](https://github.com/excilys/androidannotations/issues/1610) is closed.


Old doc:
>ViewServer is a simple class you can use in your Android application
>to use the HierarchyViewer inspection tool.

>ViewServer requires the Android SDK r12 or higher.
>http://developer.android.com/sdk/index.html

>Please refer to the documentation in ViewServer.java for more info.
