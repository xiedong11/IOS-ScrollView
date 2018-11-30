# IOS-ScrollView [![](https://jitpack.io/v/xiedong11/IOS-ScrollView.svg)](https://jitpack.io/#xiedong11/IOS-ScrollView)

扩充安卓原生ScrollView实现仿IOS弹性拖拽回弹效果

![Sample Screenshot](https://github.com/xiedong11/IOS-ScrollView/blob/master/picture/GIF.gif)

## Gradle

``` groovy
项目中添加jitpack仓库

allprojects {
		repositories {
			maven { url 'https://jitpack.io' }
		}
	}

在Module中添加依赖


dependencies {
    implementation 'com.github.xiedong11:IOS-ScrollView:v1.0'
    	}


如果你的项目中引入后，项目目依赖包发生Manifest Merge冲突，请在Module把依赖改成如下：
implementation ('com.github.xiedong11:IOS-ScrollView:v1.0'){
    exclude group: 'com.android.support'
}
```


## Usage
支持Srcollview所有属性，使用方式完全和ScrollView一致，只是扩展了拖动回弹效果

**XML**

``` xml
<com.zhuandian.scrollview.IOSScrollView
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".ImageScrollViewActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical">

        .
        .
        .

    </LinearLayout>
</com.zhuandian.scrollview.IOSScrollView>
```