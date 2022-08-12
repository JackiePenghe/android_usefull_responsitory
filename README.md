# android_usefull_responsitory
# 安卓好用的第三方仓库

部分仓库为jcenter库移植，并转为androidx（这些库在对应的位置是写有相关说明的）

使用这些仓库时，一定要先引入jitpack仓库

```
  //jitpack仓库
  maven {
    url 'https://jitpack.io'
  }
```

## 常用的基础库[https://gitee.com/sscl/baselibrary-for-kotlin](https://gitee.com/sscl/baselibrary-for-kotlin)

```xml
    /* * * * * * * * * * * * * * * * * * * 基础库开始 * * * * * * * * * * * * * * * * * * */
    //常用基础库 
    implementation 'com.gitee.sscl:baselibrary-for-kotlin:2.3.14'
    //使用AutoSwipeRefreshLayout需要引入SwipeRefreshLayout库
    implementation 'androidx.swiperefreshlayout:swiperefreshlayout:1.1.0'
    //使用BaseSplashActivity需要引入SplashScreen库
    implementation 'androidx.core:core-splashscreen:1.0.0'
    /* * * * * * * * * * * * * * * * * * * 基础库结束 * * * * * * * * * * * * * * * * * * */
```

## 网络请求库[https://github.com/liangjingkanji/Net](https://github.com/liangjingkanji/Net)

```xml
    /* * * * * * * * * * * * * * * * * * * 网络请求库开始 * * * * * * * * * * * * * * * * * * */
    //OkHttp库，要求版本在OkHttp4.x以上
    implementation 'com.squareup.okhttp3:okhttp:4.9.3'
    //网络请求库 https://github.com/liangjingkanji/Net
    implementation 'com.github.liangjingkanji:Net:3.4.12'
    //网络请求库要求使用kotlin协程库
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:1.6.0"
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.6.0'
    /* * * * * * * * * * * * * * * * * * * 网络请求库结束 * * * * * * * * * * * * * * * * * * */
```

## ViewModel(一般与databinding配合使用)

```xml
    /* * * * * * * * * * * * * * * * * * * ViewModel库开始 * * * * * * * * * * * * * * * * * * */
    //ViewModel库基本
    implementation 'androidx.lifecycle:lifecycle-viewmodel-ktx:2.3.1'
    //ViewModel库高级
    implementation "androidx.activity:activity-ktx:1.3.1"
    /* * * * * * * * * * * * * * * * * * * ViewModel库结束 * * * * * * * * * * * * * * * * * * */
```
dataBiding开启（buid.gradle中）
```xml
    android {
        ...
        //开启dataBinding
        dataBinding {
            enabled = true
        }
        ...
    }
```

## RecyclerView适配器库[https://github.com/CymChad/BaseRecyclerViewAdapterHelper](https://github.com/CymChad/BaseRecyclerViewAdapterHelper)
```xml
    /* * * * * * * * * * * * * * * * * * * RecyclerView适配器库开始 * * * * * * * * * * * * * * * * * * */
    //RecyclerView适配器库 
    implementation 'com.github.CymChad:BaseRecyclerViewAdapterHelper:3.0.7'
    //RecyclerView适配器库要求RecyclerView版本在1.2.1及以上
    implementation 'androidx.recyclerview:recyclerview:1.2.1'
    /* * * * * * * * * * * * * * * * * * * RecyclerView适配器库结束 * * * * * * * * * * * * * * * * * * */
```

## Gson(json数据解析库)
```xml
  implementation 'com.google.code.gson:gson:2.9.0'
```

## zbar 二维码扫描库[https://github.com/bingoogolapple/BGAQRCode-Android](https://github.com/bingoogolapple/BGAQRCode-Android)
```xml
  implementation 'com.github.bingoogolapple.BGAQRCode-Android:zbar:1.3.8'
```

## 二维码库(我大多用于生成二维码，轻量级的二维码库)[https://github.com/jenly1314/ZXingLite](https://github.com/jenly1314/ZXingLite)
```xml
  implementation 'com.github.jenly1314:zxing-lite:2.2.1'
```

## glide图片加载库
```xml
    implementation 'com.github.bumptech.glide:glide:4.13.1'
    //java使用annotationProcessor从而使@GlideModule注解生效
    annotationProcessor 'com.github.bumptech.glide:compiler:4.13.1'
    //Kotlin使用kapt从而使@GlideModule注解生效(需要使用 plugin 'kotlin-kapt')
    kapt 'com.github.bumptech.glide:compiler:4.13.1'
```

## 富文本加载框架[https://gitee.com/sscl/RichText](https://gitee.com/sscl/RichText)
此库本为jcenter仓库，源库地址为[https://github.com/zzhoujay/RichText](https://github.com/zzhoujay/RichText)
我克隆了此仓库并发布到jitpack中（同时转为androidx库，源库用的是support库）
```xml
  implementation 'com.gitee.sscl:RichText:1.0.1'
```

## 屏幕适配库[https://github.com/JessYanCoding/AndroidAutoSize](https://github.com/JessYanCoding/AndroidAutoSize)
```xml
implementation 'com.github.JessYanCoding:AndroidAutoSize:v1.2.1'
```

## websocket库[https://github.com/TooTallNate/Java-WebSocket](https://github.com/TooTallNate/Java-WebSocket)
```xml
   implementation 'org.java-websocket:Java-WebSocket:1.5.2'
```

## EventBus
```xml
 implementation 'org.greenrobot:eventbus:3.3.1'
```

## 安卓串口库[https://gitee.com/sscl/SerialPortLibrary](https://gitee.com/sscl/SerialPortLibrary)
```xml
implementation 'com.gitee.sscl:SerialPortLibrary:1.0.4'
```

## 图片选择器[https://gitee.com/sscl/image-picker](https://gitee.com/sscl/image-picker)
此库本为jcenter仓库，源库地址为[https://github.com/jeasonlzy/ImagePicker](https://github.com/jeasonlzy/ImagePicker)
我克隆了此仓库并发布到jitpack中（同时转为androidx库，源库用的是support库）
```xml
implementation 'com.gitee.sscl:image-picker:1.0.0'
```

