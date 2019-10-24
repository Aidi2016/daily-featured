# 每日一荐

![历史共访问次数](https://visitor-count-badge.herokuapp.com/total.svg?repo_id=azl397985856.daily-featured)
![今天被访问次数](https://visitor-count-badge.herokuapp.com/today.svg?repo_id=azl397985856.daily-featured)

> 统计数据的时间是从 2019-09-15 16:50 起至今

每天给你推荐一个新奇，好玩，高品质的开源库，好文，观点或言论等。

> 项目主页维护当前月份的内容，想看往期内容，可以翻到下方历史汇总部分，然后选择自己感兴趣的月份点进去即可。

## 新鲜出炉(2019-10)

### 2019-10-24[]

今天是1024程序员节，祝广大的程序员们节日快乐。🎩🎩🎩🎩🎩🎩

之前给大家介绍了一款跨平台的Web平台技术栈检测工具Wappalyzer。这几天我看了下他的源码，觉得很不错，于是就想着推荐给大家。

Wappalyzer的整体架构非常有意思，这里讲一下我发现的主要特点，更多细节等待着你的探索。

- 平台相关的代码放在drivers文件夹下，公共的代码在src/wappalyzer.js
- 特地向了validate脚本来检测代码。
- 将检测逻辑抽离到了src/app.json 中， 以配置文件的形式存放（这个json文件结构设计地很精巧，应该是花了心思的）
- 主要采用正则来检测应用
- 考虑到间接引用，比如框架A引用了B，那么检测到了A也会把B带上

如果想快速上手可以看下ta提供的[测试用例](https://github.com/AliasIO/Wappalyzer/blob/master/src/wappalyzer.spec.js)，非常简洁。

Github地址： https://github.com/AliasIO/Wappalyzer

### 2019-10-23[网站]

今天给广大的前端朋友们介绍一个在线做题的网站，可以瞬间在线知道答案，而且不需要登陆，一共58道题目，不知道后续会不会更新。 这个网站的题目我看了其实没有什么新意，但是不需要登陆而是直接使用LocalStorage来存储你的答题情况对用户来说很轻量，给我的感觉很好，感兴趣的可以试一下。 

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g87wixe9u2j30gk0f93yu.jpg)

(题目列表)

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g87wji13epj30ht0ket8v.jpg)

(题目详情)


网址： https://quiz.typeofnan.dev/



### 2019-10-22[观点]

前一段时间王思聪的股权遭到了冻结，据中新经纬记者计算，王思聪名下冻结股权价值合计已经超过8445万元。

“这种情况一般是王思聪欠别人钱，别人追讨，作为诉讼保全措施冻结的。”金杜律师事务所律师李量接受虎嗅采访时说，“王思聪欠钱可以是直接欠，或和贾跃亭一样，给别人提供担保，承担了连带责任。”

但是实际上这种冻结对于王思聪来说根本起不到作用，他会有很多方法来免除所谓的强制执行，他只要将自己的股权先一步将股权质押给万达集团，这样`质押权人就对被保全的股份有优先权`, 换句话说这`对王思聪来说这种冻结根本无效`。

现实中有很多这样的事情，这些规则似乎是在`限制那些“能力不足”的人，而对社会上这些“制造规则的人”无能为力`。更可悲的是，很多人对这些不知道，不关注。其实越是贫穷的家庭，越是生活在社会底层的人，他们的后代，大概率还会是穷人。其实，我们奋斗的目标无非就是：让子女一出生就站在了别人的肩膀上！

### 2019-10-21[效率]

我是一个有着轻微强迫症的人，社交软件的小红点有时候会打乱我的节奏，将我从专注模式(Focus Mode)强制转化为发散模式（Diffuse Mode）。 这两种模式适合我们做不同类型的工作，因此掌控小红点，避免这种不希望的模式切换是提高效率的一个有效途径。

我的做法是：

- 手机静音
- 电脑关闭红点提醒

mac电脑可以在系统偏好设置 - 通知 - 对应APP - 将标记应用程序的勾去掉

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g82fq7pugoj30hj09vmzb.jpg)

一般而言，你也不用担心会错过什么东西，因为右侧通知还是会有的，比如钉钉的会议提醒等。

经过这样的设置，你就可以自由切换两种模式，而不会被频繁打断，当然还是会有人来打断你，这个问题我们以后再讲。

### 2019-10-18[类库]

UMI的官方定位是`可插拔的企业级 react 应用框架`。其作者云谦也是Ant-Design，dvajs的核心贡献者，同时也是我早期关注的人之一。这个项目的价值绝对不亚于更受大家欢迎的dvajs，是一个值得学习的项目。

说白了，Umi 和 create-react-app（cra）类似，就是现有技术栈的组合，封装细节，让开发者用起来更简单，只写业务代码就可以了，它有几个特点：

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g81gv20dydj30rd0g7gq3.jpg)

- 零配置就是默认选型都给你做好了。
- 开箱即用就是技术栈都固化了。
- 约定大于配置，开发模式也固化好了。

下图是云谦介绍umi的定位的时候贴的一张架构图：

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g7hiqa9s0wj30u00l0ac7.jpg)

项目地址：https://github.com/umijs/umi

### 2019-10-17[工具]

之前分享过《2019-09-23 - 为什么一行80个字符是一个值得遵守的规范，即使你拥有4k显示器？》，里面提到了并排窗口的问题。 多个显示器确实可以提高效率，如果你能高效地利用每一个显示器，效果会更棒。

> 配合4k大屏显示器效果更棒

今天介绍的这款工具就是一款窗口布局工具，能够快速修改当前窗口大小并放置在指定位置，Moom 默认操作点设立在了窗口左上角的绿色按钮上，将鼠标hover在绿钮上就会弹出一个选择菜单，里面有五种尺寸可选，单击选项即可变化窗口大小，并能将窗口移动到指定位置。

> 搭配使用快捷键效果更棒

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g80yebwmr2j30u10fwdhw.jpg)

### 2019-10-16[工具]

今天给大家推荐的是一款非常好用的Chrome插件，可以用来查看网站是由什么技术栈构建的。其实类似的软件也有别的，但是这个是我使用过的最好的一个。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7z2wky65hj30d5093gln.jpg)

（这个是其官网的检测结果）

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7z2wyx0jzj30db09374b.jpg)

（这个是GitHub的检测结果）

项目主页： https://www.wappalyzer.com

### 2019-10-15[技能]

今天给大家分享一个微信小技巧，据说有的人还不知道，所以今天就把它分享出来，大家如果有什么微信使用小技巧也欢迎在下方进行评论。

今天的小技巧是`判断对方是否把你拉黑或者删除`:

1. 给对方转账，是好友会让你输入密码，不是好友都不用你输入密码，直接弹出下图，整个过程好友不知情的！

- 如果拉黑会提示： `请确认你和他（她）的好友关系是否正常`
- 如果删除，则会提示： `你不是收款方的好友`

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7ynsya4cmj306m05wt8l.jpg)

2. 点开好友名片，如果显示左图，说明她真的没有发过一条朋友圈。若显示右图，点开个人相册却什么也看不到，那么你有可能被删除、拉黑、朋友圈屏蔽，或者发过朋友圈但设为私密了。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7yns7ad9uj30k00f0aal.jpg)

为了搞清楚对方是删除还是屏蔽，你就可以用到开头转账的那一招啦！

### 2019-10-14[好文]

如果想做一些高级的东西，编译是一个绕不过的坎，Babel是一个前端的转义工具，Babel有着自己的插件系统，这是个系列文章，通过这个系列你可以学到AST，以及Babel插件相关的东西，并且你可以自己动手写一个Babel插件。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7xhj17ovfj30kv0hhmxq.jpg)

文章地址： 

- [Step-by-step guide for writing a custom babel transformation](https://lihautan.com/step-by-step-guide-for-writing-a-babel-transformation/)
- [Creating custom JavaScript syntax with Babel](https://lihautan.com/creating-custom-javascript-syntax-with-babel/)

### 2019-10-12[工具]

前端在调试兼容性样式的时候是一个很头疼的问题，各个浏览器以及同一个浏览器不同版本支持的css都是不同的，比如有些不支持Grid，有些不支持cal函数。如果你自己根据这些去修改代码肯定是非常低效的，这个Chrome插件就是解决这样的问题，你可以在高级的浏览器上调试，自行禁用一些css特性来debug。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7ucx8rqutj30dv05sq2v.jpg)

仓库地址： https://github.com/keithclark/css-feature-toggle-devtools-extension

chrome插件地址： https://chrome.google.com/webstore/detail/css-feature-toggles/aeinmfddnniiloadoappmdnffcbffnjg


### 2019-10-11[工具]

常用正则大全, 支持vscode扩展插件

值得一提的是它支持VSCode插件形式使用：

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7u0yqfy5nj30jn0eg0t4.jpg)

目前有57个正则：

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7u0zximv9j30b80g3dgg.jpg)


插件地址： https://github.com/any86/any-rule


### 2019-10-10[技能]

傅里叶变换是一种在各个领域都经常使用的数学工具。这个网站将为你介绍傅里叶变换能干什么，为什么傅里叶变换非常有用，以及你如何利用傅里叶变换干漂亮的事。傅立叶变换有很多实际的应用，比如MP3的原理，MP3是如何将声波转化为二进制，并如何进行压缩的？ 比如JPEG的原理等。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7s4pz83xyj30x50kpt9s.jpg)

这个文章（网站）是我见过傅立叶变换最直观的一个解释之一，并且支持交互式操作。 

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7s4pm4mooj307404j0sl.jpg)


网站地址： http://www.jezzamon.com/fourier/zh-cn.html

### 2019-10-09[工具]

VSCode是我经常使用的一个软件，结合自己的开发习惯我也会增加很多配置和插件等，如何将这些插件进行备份以便将来换电脑可以及时同步过来，这里关于VScode的配置我用的是VSCode [setting sync 插件](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)。


这个需要结合Gist使用，具体使用方式请查看官方文档：

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7r455m0zmj30i909dq36.jpg)

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7r4cvxwb5j30rw0gc74r.jpg)

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7r4db2zxbj30tf0kcgm9.jpg)

其实我有一个专门的[开发常用配置文件备份仓库](https://github.com/azl397985856/dev-config)用来存放这些东西，这是我的仓库存放的配置，这样我即使换了电脑也能很快地用到我最舒服的配置。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7r4nhzmjgj30a808ajrb.jpg)

如果大家没有更好的方式，不妨采用这种方式，如果你有更好的方式欢迎给我留言。

### 2019-10-08[工具]

今天是国庆结束的第一天，大家假期玩的怎么样？ 希望大家可以尽快从假期的状态中转变回来。今天给大家推荐一个我个人使用比较多的一个功能，就是`剪贴板历史`。

我在使用手机的时候（笔者使用的是安卓机），会经常复制一些文字或者图片，然后进行粘贴，有时候会需要粘贴之前复制的一个东西，因此剪贴板历史就显得很重要，手机上我用的就是`搜索输入法自带的剪贴板历史功能`。

而在电脑上我使用的是Alfred自带的`剪贴板历史`功能，只不过默认不开启，你需要去配置一下才行。

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7pqb232pxj30w50fvdgy.jpg)

然后你就可以查看你的剪贴板历史了：

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7pqbppfxrj30hg0cn0tt.jpg)

![](https://tva1.sinaimg.cn/large/006y8mN6ly1g7pqc0f7tbj30g40bv75d.jpg)

## 历史汇总

- [2019-09](./backup/2019-09/)

## 关注我

我重新整理了下自己的公众号，并且我还给它换了一个名字`脑洞前端`，它是一个帮助你打开大前端新世界大门的钥匙 🔑，在这里你可以听到新奇的观点，看到一些技术尝新，还会收到系统性总结和思考。

在这里我会尽量通过图的形式来阐述一些概念和逻辑，帮助大家快速理解，图解是我的目标。

之后我的文章会同步到微信公众号 `脑洞前端` ，你可以关注获取最新的文章，并和我进行交流。

另外你可以回复大前端进大前端微信交流群， 回复 leetcode 拉你进 leetcode 微信群，如果想加入 qq 群，请回复 qq。

<img width="300" src="https://tva1.sinaimg.cn/large/006y8mN6ly1g7he9xdtmyj30by0byaac.jpg">

## 贡献

- 如果有想法和创意，请提[issue](https://github.com/azl397985856/daily-featured/issues)或者进群提
- 如果想贡献代码，请提[PR](https://github.com/azl397985856/daily-featured/pulls)
- 如果需要修改项目中图片，[这里](./assets/)存放了项目中绘制图的源代码， 大家可以用[draw.io](https://www.draw.io/)打开进行编辑。

## License

[Apache-2.0](./LICENSE)
