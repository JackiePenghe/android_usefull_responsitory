# android_usefull_responsitory
# 安卓好用的第三方仓库（因为jcenter仓库已经停止维护，故不包含jcenter仓库中的信息）

jitpack仓库依赖

```
  //jitpack仓库
  maven {
    url 'https://jitpack.io'
  }
```

## 常用的基础库(https://gitee.com/sscl/baselibrary-for-kotlin)[https://gitee.com/sscl/baselibrary-for-kotlin]

```
    /* * * * * * * * * * * * * * * * * * * 基础库开始 * * * * * * * * * * * * * * * * * * */
    //常用基础库 
    implementation 'com.gitee.sscl:baselibrary-for-kotlin:2.3.14'
    //使用AutoSwipeRefreshLayout需要引入SwipeRefreshLayout库
    implementation 'androidx.swiperefreshlayout:swiperefreshlayout:1.1.0'
    //使用BaseSplashActivity需要引入SplashScreen库
    implementation 'androidx.core:core-splashscreen:1.0.0'
    /* * * * * * * * * * * * * * * * * * * 基础库结束 * * * * * * * * * * * * * * * * * * */
```
