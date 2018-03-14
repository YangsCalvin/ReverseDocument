# Reverse Document

[![](https://travis-ci.org/Alamofire/Alamofire.svg?branch=master)](http://www.yangziyao.top)
[![GitHub issue author](https://img.shields.io/github/issues/detail/u/badges/shields/979.svg)](https://weibo.com/5905837515/profile?topnav=1&wvr=6)
[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php) 
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/CodyCalvin/WebCrawler) 

逆向工程的目的
-----
1. 分析竞品的最新研究或者产品原型（包括所用的技术，所使用的框架）

2. 有助于进一步的认识iOS从而提升自己／学习目的。

3. 破解应用的使用权限

4. 识别竞品潜在的侵权行为

逆向工程的分析工具
------

* 进行iOS逆向工程的一个关键就是工具的使用，工欲善其事，必先利其器。


|工具分类|  工具名称  |
| -----|:---------:|
|越狱工具| [盘古越狱](http://www.pangu.io) |
|查看文件工具| [PP助手](https://pro.25pp.com)，[iExplorer](https://iexplorer.en.softonic.com)，[iFunbox](http://www.i-funbox.com/zh-cn_index.html)，[iTool](https://www.itools.cn)|
|砸壳工具| [dumpdecrypted](https://github.com/stefanesser/dumpdecrypted)，[Clutch](https://github.com/KJCracks/Clutch)|
|查看头文件工具| [class-dump](https://github.com/nygard/class-dump)|
|反汇编工具| [Hopper](https://www.hopperapp.com)，[IDA Pro](https://www.hex-rays.com)|
|调试器| [HCycript](http://iphonedevwiki.net/index.php/Cycript_Tricks "插件Cydia安装")，[gdb](http://www.gnu.org/software/gdb/ "插件Cydia安装")|
|UI分析工具| [Reveal](https://revealapp.com)|
|网络分析工具| [Charles](https://www.charlesproxy.com)|

1.准备阶段
-------

先上 iOS 逆向的三板斧，这是每次要逆向破解前都需要做的步骤。如果你不了解iOS逆向的话你可以参考一下文章[iOS逆向工程准备工作](https://www.jianshu.com/p/0cb76f7203b3)或者阅读[iOS应用逆向工程](https://book.douban.com/subject/25826902/)书籍当然也有PDF版[iOS应用逆向工程pdf版](http://www.cocoachina.com/bbs/read.php?tid-1677433.html)

首先，请确保你的手机已经越狱，同时已经安装好 theos 开发环境，当然如果你做的`Tweak`比较简单的话那么你可以使用[MokeyDev](https://github.com/AloneMonkey/MonkeyDev)来开发调试。

2.砸壳
-------

如果是从 AppStore 上面下载的 App，都要先进行砸壳，否则是没办法进行下一步的。如果你懒得做这一步，就直接去其它助手类应该上面进行下载，那些都是砸过壳的，可以直接使用。

砸壳可以使用的工具有两种：

[dumpdecrypted](https://github.com/stefanesser/dumpdecrypted)，使用方法请参考[dumpdecrypted砸壳](http://www.swiftyper.com/2016/05/02/iOS-reverse-step-by-step-part-1-class-dump/)

[Clutch](https://github.com/KJCracks/Clutch)，使用方法请参考[Clutch砸壳](http://www.swiftyper.com/2016/12/26/wechat-redenvelop-tweak-for-non-jailbroken-iphone/)

大多数App可以直接在PP助手在这里，我们这里以逆向陌陌为例就直接用PP助手下载陌陌越狱版省去砸壳步骤.具体流程请看下图
