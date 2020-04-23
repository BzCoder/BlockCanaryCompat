# BlockCanaryCompat
[ ![Download](https://api.bintray.com/packages/bzcoder/BlockCanaryCompat/blockcanarycompat-android/images/download.svg?version=0.0.4) ](https://bintray.com/bzcoder/BlockCanaryCompat/blockcanarycompat-android/0.0.4/link)

修改自[BlockCanary](https://github.com/markzhai/AndroidPerformanceMonitor)，适配Android 8.0以上版本。

引入：
```
    debugImplementation('com.github.bzcoder:blockcanarycompat-android:0.0.4')
    releaseImplementation('com.github.bzcoder:blockcanarycompat-android-no-op:0.0.4')
```

兼容：
- 高版本不能获取IMEI的问题
- 高版本不弹出通知问题
- 高版本无法获取CPU信息的问题

新增：
- App是否在前台选项
- GetSingleCpuRateInfoUtils工具类提取CPU信息单独选项
- reportRecentOneMessage选项，作用为限制上报卡顿信息为一条（如果需要采集线上日志，可配合使用）
