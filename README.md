# iOS设备、Icon、LaunchImage分辨率 - 含iPhone X

***摘要：***iOS的各种设备的分辨率，以及开发用的Icon、LaunchImage的分辨率。

***文中所有数据均来自网络，及博主个人总结，如有错误，以官方数据为准。***

## iOS设备

iOS设备的屏幕的大小、分辨率以及比例因数（Scale Factor）[1]。

### iPhone

|    设备     | 宽(inch) | 高(inch) | 对角线(inch) | 逻辑分辨率(point) | Scale Factor |      设备分辨率(pixel)      | PPI  |
| :-------: | :-----: | :-----: | :-------: | :----------: | :----------: | :--------------------: | :--: |
|    3GS    |   2.4   |   4.5   |    3.5    |   320X480    |     @1x      |        320X480         | 163  |
|   4/4s    |  2.31   |   4.5   |    3.5    |   320X480    |     @2x      |        640X960         | 326  |
|    5c     |  2.33   |  4.90   |     4     |   320X568    |     @2x      |        640X1136        | 326  |
|   5/5s    |  2.31   |  4.87   |     4     |   320X568    |     @2x      |        640X1136        | 326  |
|  6/6s/7   |  2.64   |  5.44   |    4.7    |   375X667    |     @2x      |        750X1334        | 326  |
| 6+/6s+/7+ |  3.06   |  6.22   |    5.5    |   414X736    |     @3x      | 1080X1920(1242X2208)\* | 401  |
|     X     |  2.79   |  5.65   |    5.8    |   375X812    |     @3x      |      1125 × 2436       | 458  |

\**在iPhone 6 Plush、iPhone 6s Plush以及iPhone 7 Plush中，实际分辨率为1080X1920，在开发中，以1242X2208进行适配。*

### iPad

| 设备名称         |  上市日期   | 屏幕尺寸(inch) | Scale Factor | 设备分辨率(pixel) | PPI  |
| :----------- | :-----: | :--------: | :----------: | :----------: | :--: |
| iPad         | 2010.01 |    9.7     |     @1x      |   1024X768   | 132  |
| iPad2        | 2011.03 |    9.7     |     @1x      |   1024X768   | 132  |
| The new iPad | 2012.05 |    9.7     |     @2x      |  2048X1536   | 264  |
| iPad mini    | 2012.10 |    7.9     |     @1x      |   1024X768   | 163  |
| iPad 4       | 2012.12 |    9.7     |     @2x      |  2048X1536   | 264  |
| iPad Air     | 2013.10 |    9.7     |     @2x      |  2048X1536   | 264  |
| iPad mini 2  | 2013.10 |    7.9     |     @2x      |  2048X1536   | 326  |
| iPad Air2    | 2014.10 |    9.7     |     @2x      |  2048X1536   | 264  |
| iPad mini 3  | 2014.10 |    7.9     |     @2x      |  2048X1536   | 326  |
| iPad mini 4  | 2015.09 |    7.9     |     @2x      |  2048X1536   | 326  |
| iPad Pro     | 2015.11 |    12.9    |     @3x      |  2732X2048   | 264  |

---

**在Xcassets中，图片名称不再重要，只需要将相应的图片放置至对应的位置即可。以下命名只作参考。**

## Icon

iOS应用图标的命名及分辨率大小和用途[2]。

| 名称               | 分辨率(pixel) | 用途                                       |
| :--------------- | :--------: | :--------------------------------------- |
| iTunesArtwork    |  512X512   | iTunes商店应用列表的图标                          |
| iTunesArtwork@2x | 1024X1024  | 视网膜屏幕设备的iTunes商店应用列表的图标                  |
| Icon-60@2x       |  120X120   | 视网膜屏幕的iPhone或iPod Touch的桌面图标             |
| Icon-60@3x       |  180X180   | iPhone 6 Plus的桌面图标                       |
| Icon-76          |   76X76    | iPad的桌面图标                                |
| Icon-76@2x       |  152X152   | 视网膜屏幕的iPad的桌面图标                          |
| Icon-Small-40    |   40X40    | 搜索结果列表的图标                                |
| Icon-Small-40@2x |   80X80    | 视网膜屏幕设备的搜索结果列表的图标                        |
| Icon-Small-40@3x |  120X120   | iPhone 6 Plus的搜索结果列表的图标                  |
| Icon-Small       |   29X29    | 设置中的图标                                   |
| Icon-Small@2x    |   58X58    | 视网膜屏幕设备的设置中的图标                           |
| Icon-Small@3x    |   87X87    | iPhone 6 Plus的设置中的图标                     |
| **iOS 6.1及之前**\* |            |                                          |
| Icon             |   57X57    | iOS 6.1及之前的iPhone和iPod Touch的桌面图标        |
| Icon@2x          |  114X114   | iOS 6.1及之前的视网膜屏幕的iPhone和iPod Touch的桌面图标  |
| Icon-72          |   72X72    | iOS 6.1及之前的iPad的桌面图标                     |
| Icon-72@2x       |  144X144   | iOS 6.1及之前的视网膜屏幕的iPad的桌面图标               |
| Icon-Small       |   29X29    | iOS 6.1及之前的iPhone和iPod Touch的搜索结果列表和设置中的图标 |
| Icon-Small@2x    |   58X58    | iOS 6.1及之前的视网膜屏幕的iPhone和iPod Touch的搜索结果列表和设置中的图标 |
| Icon-Small-50    |   50X50    | iOS 6.1及之前的iPad的搜索结果列表的图标                |
| Icon-Small-50@2x |  100X100   | iOS 6.1及之前的视网膜屏幕的iPad的搜索结果列表的图标          |

\**iOS 6.1及以前的设备已经很少了，所以可以选择适配。*

## LaunchImage

iOS应用的启动页分辨率及用途。

### iPhone

| 名称                        | 分辨率(pixel) | 用途                                       |
| :------------------------ | :--------: | :--------------------------------------- |
| **竖屏(Portrait)**          |            |                                          |
| Default                   |  320X480   | 用于iPhone 3GS                             |
| Default@2x                |  640X960   | 用于iPhone 4/4s                            |
| Default-568h@2x           |  640X1136  | 用于iPhone 5/5c/5s                         |
| Default-Retina@2x         |  640X1136  | 用于iPhone 5/5c/5s                         |
| Default-667h@2x           |  750X1334  | 用于iPhone 6/6s/7/8                        |
| Default-736h@3x           | 1242X2208  | 用于iPhone 6 Plush/6s Plush/7 Plush/8 Plush |
| Default-812h@3x           | 1125X2436  | 用于iPhone X                               |
| **横屏(Landscape)**         |            |                                          |
| Default-736h-Landscape@3x | 2208X1242  | 用于iPhone 6 Plush/6s Plush/7 Plush/8 Plush横屏启动 |
| Default-812h-Landscape@3x | 2436X1125  | 用于iPhone X横屏启动                           |


### iPad

| 名称                                  | 分辨率(pixel) | 备注   |
| :---------------------------------- | :--------: | :--- |
| Default-Landscape~iPad              |  1024X768  | 横屏   |
| Default-Portrait~iPad               |  768X1024  | 竖屏   |
| Default-Landscape~iPad@2x           | 2048X1536  | 横屏   |
| Default-Portrait~iPad@2x            | 1536X2048  | 竖屏   |
| **To-Status-Bar**\*                 |            |      |
| Default-Landscape-StatusBar~iPad    |  1024X748  | 横屏   |
| Default-Portrait-StatusBar~iPad     |  768X1004  | 竖屏   |
| Default-Landscape-StatusBar~iPad@2x | 2048X1496  | 横屏   |
| Default-Portrait-StatusBar~iPad@2x  | 1536X2008  | 竖屏   |

\**to-Status-bar:个人理解为不包含状态栏。*

## 其他相关大小



| 控件（Element）                              | 大小（Size）(points)                     | 备注                               |
| :--------------------------------------- | :----------------------------------- | :------------------------------- |
| Window (including status bar)            | 320 x 480 pts                        | 窗口(包含状态栏)                        |
| Status Bar                               | 20 pts                               | 状态栏                              |
| View inside window(visible status bar)   | 320 x 460                            | 窗口内的视图，不包含状态栏                    |
| Navigation Bar                           | 44 pts                               | 导航栏高度                            |
| Nav Bar Image / Toolbar Image            | up to 20 x 20 pts (transparent PNG)  | 导航栏图标大小，拉伸或压缩至20X20,建议使用透明的PNG图片 |
| Tab Bar                                  | 49 pts                               | 标签栏                              |
| Tab Bar Icon                             | up to 30 x 30 pts (transparent PNGs) | 标签栏图标，拉伸或压缩至30X30，建议使用透明PNG图片    |
| Text Field                               | 31 pts                               | 文本框高度，不可调                        |
| Height of a view inside a navigation bar | 416 pts                              | 有导航栏存在的视图高度                      |
| Height of a view inside a tab bar        | 411 pts                              | 有标签栏存在的视图高度                      |
| Height of a view inside a navbar and a tab bar | 367 pts                              | 导航栏、标签栏同时存在的视图高度                 |
| Portrait Keyboard height                 | 216 pts                              | 竖屏键盘高度                           |
| Landscape Keyboard height                | 140 pts                              | 横屏键盘高度                           |

*此表中大小以单倍比例因数为准。*


## 最后再说几句

### 参考

>[1] 参考自[Apple官网](http://www.apple.com)及[中关村在线](http://www.zol.com.cn)


>[2] 《[App Icons on iPad and iPhone](https://developer.apple.com/library/ios/qa/qa1686/_index.html)》