# DayDayNews
![enter image description here](https://img.shields.io/badge/build-passing-red.svg)
![enter image description here](https://img.shields.io/badge/language-iOS-brightgreen.svg)
![enter image description here](https://img.shields.io/badge/platform-iOS%207.0%2B-ff69b4.svg)

仿网易新闻客户端，实现新闻浏览，视频播放，抓取百度图片，瀑布流显示,自定义视频播放，横屏竖屏切换自如,设置界面优化，第三方登录以及注销，新闻数据以及图片的收藏与分享。

##Demo扫码安装
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/wcnS.png)<br>
ipa上传到蒲公英分发平台，扫码根据提示等待就可以按照完毕 <br>
安装完成之后第一次打开会出现未受信任的企业级开发者。 解决方法：在设置->通用->设备管理，点击信任即可


##GIF
![gif](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/news.gif)


##导航
1. [Update Log](https://github.com/gaoyuhang/DayDayNews#update-log)
2. [首页以及顶部新闻详情](https://github.com/gaoyuhang/DayDayNews#首页以及顶部新闻详情高仿网易) 
3. [天气预报的功能](https://github.com/gaoyuhang/DayDayNews#https://github.com/gaoyuhang/DayDayNews#增加了天气预报的功能可以实现定位到当前城市动画效果也没有放过)
4. [图片界面，采用瀑布流展示](https://github.com/gaoyuhang/DayDayNews#使用瀑布流实现图片可以选择分类)
5. [视频界面](https://github.com/gaoyuhang/DayDayNews#视频)
6. [我的界面，包括第三方登录，夜间模式，清除缓存，环信聊天](https://github.com/gaoyuhang/DayDayNews#我的界面实现第三方登陆以及注销界面优化)
 1. [夜间模式和收藏功能](https://github.com/gaoyuhang/DayDayNews#夜间模式和收藏功能)
 2. [环信即时通讯](https://github.com/gaoyuhang/DayDayNews#帮助与反馈界面环信即时通讯)
7. [项目结构](https://github.com/gaoyuhang/DayDayNews#项目结构)
8. [项目所用API](https://github.com/gaoyuhang/DayDayNews#项目所用API)
9. [About](https://github.com/gaoyuhang/DayDayNews#about)
10. [Support](https://github.com/gaoyuhang/DayDayNews#support)
 1. [简书地址](http://www.jianshu.com/users/85973c3d2045/latest_articles)


##Update Log
- 适配了iOS9<br />
- 增加了点击tabbar刷新当前页面的功能<br />
- 2016-1-2 修改了首页顶部滚动条的接口 <br />
- 2016-1-14 处理天气预报加载时间长，没页面显示的问题。<br />
- 2016-1-19 更换了corelocation定位，系统定位繁琐速度慢。更换为INTULocationManager第三方定位，block调用简单有效<br />
- 2016-1-20 更改了首页顶部滚动条详情不显示的问题。<br />
- 2016-2-10 优化天气预报城市缓存问题 <br>
- 2016-3-2  完善”我的“界面，实现第三方登录以及注销功能<br>
- 2016-3-3 修改了首页社会的显示数据，抓取网易的数据，并进行解析。 把下拉刷新改成动画效果，更美观<br>
- 2016-3-7 修改了首页imagesCell有时数据不显示的问题<br>
- 2016-4-16 完善了夜间模式的设置。<br>
- 2016-4-25 增加了收藏<br>
- 2016-4-26 初步完善了收藏，现在支持首页新闻模式的收藏。<br>
- 2016-4-29 终结了收藏功能 <br>
- 2016-5-7  在帮助与反馈界面初步增加了环信即时通讯
- 2016-5-9  在设置界面显示当前未读的消息数，实时监听并改变
- 2016-5-9  增加了本地通知
- 2016-5-12 新增图片收藏，属性列表存储,实时刷新收藏数据
- 2016-6-10 由于网易有小改动，修改了首页的显示模式 
- 2016-6-25 修改了图片模块，大图展示图片可以拉伸和缩小


###修改了视频显示方式
- 点击当前cell播放视频在当前cell上，监听屏幕转动，当屏幕转动的时候，视频自动横屏全屏播放，当屏幕为正的时候，播放在当前cell上<br />
- 增加了活动指示器，采取搜狐视频活动指示器

![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/加载.png)
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/播放.png)
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/横屏.png)
_<br />_<br />


##首页以及顶部新闻详情，高仿网易
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/newsfresh.png)
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/newsdata.png)

##使用瀑布流实现图片，可以选择分类
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/photo.png)

##增加了天气预报的功能，可以实现定位到当前城市。动画效果也没有放过。
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/detail.png)
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/weather.PNG)

##视频
- 自定义视频界面（后续修改）<br>
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/video.png)


##我的界面实现第三方登陆以及注销，界面优化。
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/login.png)
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/me.png)


##夜间模式和收藏功能
![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/yejian.png)
![图片收藏](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/photocollect.png)

##帮助与反馈界面《环信即时通讯》
设计的思路是在用户第三方登录成功的时候，利用uid去注册环信账户，注册成功就登录，如果是第二次登录，现在做的还是首先是注册，判断是否是因为账号存在而失败，如果是就进行登录，登录成功之后，在帮助与反馈界面才能进行即时通讯。 <br>
没有加好友，直接利用好友的名字来进行聊天，现在所有登录上的账户都是直接和gaoyuhang这个账号进行通信的。<br>
进入程序的时候获取当前用户未读的消息数，如果有改变实时显示出来
后期如果有需要，可以增加更多功能。<br><br>
关于环信即时通讯，请参考我另外一个demo[环信3.0Demo](https://github.com/gaoyuhang/HuanXinTest) <br>

![image](https://raw.githubusercontent.com/gaoyuhang/DayDayNews/master/photo/chat.png)


##项目结构

##项目所用API
附上部分功能API，只做学习交流。具体使用请见`Demo`
- 新闻顶部轮播图数据
  ```
  http://c.m.163.com/nc/article/headline/T1348647853363/0-10.html
  ```
- 首页新闻数据
 ```
 http://c.m.163.com/nc/article/headline/T1348647853363/0-20.html
 ```
- 天气预报接口
 ```
 http://c.3g.163.com/nc/weather/省份|城市.html
 ```
- 图片接口
 ```
 http://image.baidu.com/wisebrowse/data?tag1=一级分类&tag2=二级分类
 ```
- 视频接口
 ```
 http://c.m.163.com/nc/video/home/0-10.html
 ```

##About
本项目只供学习交流，严禁进行商业用途。:joy:

##Support
- Email：yugao5971@qq.com / gyhbsdo@163.com
- [简书地址](http://www.jianshu.com/users/85973c3d2045/latest_articles)






