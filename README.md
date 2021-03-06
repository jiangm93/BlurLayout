# BlurLayout
A fast blur layout based on FrameLayout for Android platform.

This layout can be used for realtime bluring, for example blur some area of live camera. <br/>
Or you can use it for blur some/full area of background.

![BlurLayout](https://raw.githubusercontent.com/dpproduction/BlurLayout/master/screen.png)

Usage
-----
```xml
  <com.dgroup.views.BlurLayout
        android:layout_width="match_parent"
        android:layout_height="200dp"
        android:layout_gravity="center"
        app:cropSubArea="true"
        app:blurRadius="3"
        app:scaleFactor="10"
        app:targetView="@+id/image"/>
```

BlurLayout provides next custom properties:

Attrs
-----
```xml
  	<attr name="blurRadius" format="integer"/>
        <attr name="scaleFactor" format="float"/>
        <attr name="targetView" format="reference"/>
        <attr name="cropSubArea" format="boolean"/>
        <attr name="updateFrequency" format="integer"/>
```

By default `updateFrequency` equals 0. It means that only one bluring snapshot will be taken (first available).
`updateFrequency="100"` means that snapshots will be taken every 100 milliseconds.

Pull Requests are welcome!
