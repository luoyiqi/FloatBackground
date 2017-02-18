# FloatBackground  

Floating item in background  
在背景上悬浮物体  

## 预览图 Screenshots
![demo1](/screenshot/floatbackground.gif) 

## 集成 Integrate

*  将[library](/library)导入到工程中  // import [library](/library) as a model to your project
  
*  或者将[library](/library)中的`FloatBackground.java`，`FloatObject.java`复制到你的项目中去 // Or copy `FloatBackground.java `,`FloatObject.java` from [library](/library) to your project

## 使用 Usage
####初始化 Initialization
添加`com.dean.overwatchloadingview.OverWatchLoadingView ` 到你的布局文件中  
Add `com.dean.overwatchloadingview.OverWatchLoadingView ` to your layout XML file.

```XML
<com.dean.overwatchloadingview.OverWatchLoadingView
        android:layout_centerInParent="true"
        android:layout_margin="50dp"
        android:id="@+id/loading_view"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:view_color="@color/light_orange" />
```
之后在代码中调用  
Then using in java code

```Java
OverWatchLoadingView loadingView = (OverWatchLoadingView) findViewById(R.id.loading_view);
loadingView.start();
```

####设置颜色 Setting Color
#####xml

```xml
app:view_color="@color/light_orange"
```
#####code
```java
loadingView.setColor(Color.GRAY);
```

####开始／结束／暂停／恢复 start/end/pause/resume
#####开始/start
```java
loadingView.start();
``` 
#####结束/end
```java
loadingView.end();
``` 
#####暂停/pause
```java
loadingView.pause();
``` 
#####恢复/resume
```java
loadingView.resume();
``` 

## License
```
Copyright 2016 Dean Guo

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
