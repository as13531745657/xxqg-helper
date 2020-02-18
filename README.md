# 公告
* 本助手只供个人**学习Auto.js**使用，不得**传播**和用于**违法或商业用途**，否则造成的一切**后果自负！**
* 为了方便使用，本项目没有分模块，所有代码都在一个js文件中

# 注意事项
* 1.文章根据日期抓取与别的界面混淆问题**尚未解决**，有好的方案请自行修改或建议
* 2.**华为**等部分手机不支持控制台窗口，如报错中含有`console`关键字请将`start_app()`函数中关于`console`的函数删除
* 3.请尽量更新Auto.js版本至**4.0.0beta或 4.0.1beta**,否则部分手机会有兼容性问题
* 4.尽量**不要在凌晨运行**，凌晨主页当天新闻没有刷新，**早上9-10点之后运行**，当天的文章会出来很多
* 5.运行时请保持**网络畅通**，请在**WIFI**网络下使用，否则中途加载页面或控件过慢会报错

# 使用方式 
* 下载Auto.js 4.0.0版本apk并安装
* 打开Auto.js导入最新版xxqg.js文件
* 将**tiku.db**数据库文件放在和js脚本**同一目录下**，通常情况为手机根目录的“**脚本**”文件夹下
* 点击右上角**运行**按钮运行（运行时会提示打开无障碍模式）

# 特别感谢
[lgpersonal](https://github.com/lgpersonal/LazyStudy)

# 更新日志
## v3.1.1
* 新增本地频道（1分），修改挑战答题控制逻辑（app布局更新）
## v3.1.0
* 新增每日答题，修复联播新闻乱串bug，但文章有时仍会乱串
## v3.0.1
* 修复跨年日期错误bug
## v3.0.0
* 新增挑战答题，修复联播视频问题
## v2.8beta2
* 小视频改回新闻联播
## v2.8beta1
* 新增UI界面，可方便自行修改参数
* 修复了一些问题
## v2.7beta3
* 更新了学习步骤：百灵小视频->电台+文章->电台，广播和文章同时进行，大幅缩短时间。
* 新增控制台`console`打印学习进程，之前的`toast`弃用
* 现在凌晨也能学习，找不到当天新闻自动学习昨日新闻
* 新增页面检测，意外情况离开页面会有提示并停止计时，返回界面继续计时
* 修复文章界面有时会加载视频的情况
## v2.6
* 巨大更新，文章学习根据当天日期抓取当天的文章，不再重复学习昨天的文章！
* 修复了某些情况下由于个别手机加载速度慢导致进入文章页抓取不到页面秒退的情况
## v2.5.1
* 修复新闻进入“专题”一栏无法跳出bug
* “电视台”改为“zhongyang广播电视总台”
## v2.5
* app又换了布局导致按钮控件不能用了（无奈），这次又修改了控件抓取，收藏分享评论又能用了
* 评论随机，评论过后删除
* 学习文章时滚动，学习时间随机上下波动10秒
* 分享改为app内分享，不用打开微信
## v2.4
* 新增评论功能，可自行修改commentText评论内容
* 将点赞与分享整合进前两篇文章学习过程中，节约了一定时间，不再视频学习完之后单独点赞分享
## v2.3
* 更新了视频学习逻辑，延长第一个视频（30分钟新闻正片）的学习时间，缩短了下面小新闻片段的学习数量和时间，分数更加准确
* 新增总运行时间统计
## v2.2
* 因为最新版app更换了页面布局,所以更改了按钮控件的抓取
## v2.1
* 新增弹窗函数，防止部分手机息屏
* 新增延时函数，单位由之前毫秒统一为秒
## v2.0
* 基于控件点击,不再基于屏幕坐标点击,更具有通用性
* 新增收藏和微信分享(2分)
* 修复若干bug
* “视听学习”更改为“电视台”

# 可修改的自定义变量
* `aCount`文章学习篇数,`vCount`小视频学习个数,`aTime`每篇文章学习时长(秒),`vTime`每个小视频学习时长(秒),`rTime`广播收听时长(秒), `cCount`收藏和分享次数，`commentText`评论内容，`aCatlog`文章学习类别，`lCount`挑战答题轮数，`qCount`每轮答题数，`dlCount`每日答题轮数

# xxqg-helper
* Auto.js xxqg-helper，文章和视频(24分)、收藏和分享(2分)、评论（2分）、挑战答题（6分）、每日答题（6分）、本地频道（1分）
* 仅限Android系统，需下载Auto.js，手机需开启**无障碍模式**
* Android版本至少在5.0之上，最好**7.0之上**，7.0以下**滑动**等函数不能用
* 测试环境: MIUI 11, Auto.js V4.0.0beta
