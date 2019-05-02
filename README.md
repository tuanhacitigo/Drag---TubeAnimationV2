# Drag---TubeAnimationV2

## How to make animation like youtube new? This is the demo application for you to answer the above question


This application is built based on my understanding of android, so it may not be really good, I look forward to your contributions and help to make the application more complete and optimal. Thank you!!!

![Alt text](output/ezgif.com-video-to-gif.gif) | ![Alt text](output/Screenshot_20190417-173713.png)  | ![Alt text](output/Screenshot_20190417-173738.png) 
--- | --- | --- 
![Alt text](output/Screenshot_20190417-173732.png) | ![Alt text](output/Screenshot_20190417-173744.png)  | ![Alt text](output/Screenshot_20190417-173721.png) 

#### Download

```java

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
    
    
    	dependencies {
	        implementation 'com.github.hoanganhtuan95ptit:Drag---TubeAnimationV2:1.0.0'
	}
```


#### XML

```java

    <com.hoanganhtuan95ptit.drag.ui.widget.drag.DragFrame
        android:id="@+id/drag_frame"
        android:layout_width="match_parent"
        android:layout_height="match_parent" />
```

#### Add frame top
```java
dragFrame.setTopFragment(getSupportFragmentManager(), PlayFragment.newInstance());
```

#### Add frame bottom
```java
dragFrame.setBottomFragment(getSupportFragmentManager(), DetailFragment.newInstance());
```

#### Listener
```java
dragFrame.setOnDragListener(this);
```

#### Open max
```java
dragFrame.maximize();
```

#### Open min
```java
dragFrame.minimize();
```

#### Close
```java
dragFrame.close();
```

#### Set height waiting frame top - frame top change the size when max
```java
dragFrame.setHeightWaiting(int heightWaiting);
```

#### Set height frame top - Immediately change the size
```java
dragFrame.setHeight(int height);
```

#### Check max
```java
dragFrame.isMaximized();
```

#### Check min
```java
dragFrame.isMinimized();
```

#### Check close
```java
dragFrame.isClosed();
```




## Libraries used on the sample project

* [Butterknife](https://github.com/JakeWharton/butterknife) 
* [CircleImageView](https://github.com/hdodenhof/CircleImageView)
