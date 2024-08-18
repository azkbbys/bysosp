# JS概述

脚本可以为游戏添加自定义的动态行为，为你的用户提供更吸引人的交互体验。 [javascript](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ogs36u8gn7oz00zt)是神奇代码岛支持脚本语言，你可以用它来构建你得游戏功能。

神奇代码岛（Box3）是一个基于网页的多人联机3D创作平台，支持JavaScript编程。
在神奇代码岛，模型、建筑构成了丰富多彩了视觉世界，而JavaScript代码则为这个世界注入了交互玩法的灵魂；无论是对战还是冒险，模拟经营还是角色扮演，都离不开JavaScript的神奇魔力。
现在，就跟着我一起了解JavaScript的神奇魔法吧～

## 什么是JavaScript

JavaScript（简称“JS”）是当前最流行、应用最广泛的客户端脚本语言，在 Web 开发领域有着举足轻重的地位，是成为一名优秀前端工程师的必备技能之一。
JS 是一种具有函数优先的轻量级，解释型或即时编译型的编程语言。既能用在浏览器中控制页面交互，也能用在服务器端作为网站后台（借助 Node.js），还能在各种操作系统下运行，因此 JavaScript 也是一种全栈式的编程语言。

## JS 可以做什么

JavaScript 的应用场合极其广泛，简单到幻灯片、照片库、浮动布局和响应按钮点击，复杂到游戏、2D/3D 动画、大型数据库驱动程序等等。
JavaScript 可以用于 Web 开发的各个领域，例如：
Web 应用开发：日常生活中我们所浏览的网页都是由 HTML、CSS、JavaScript 构成的，通过 JavaScript 可以实时更新网页中元素的样式，并可以实现人与网页之间的交互（例如监听用户是否点击了鼠标或按下了某个按键等），还可以在网页中添加一些炫酷的动画；
移动应用开发：除了可以进行 Web 应用开发外，JavaScript 还可以用来开发手机或平板电脑上的应用程序，而且我们还可以借助一些优秀的框架（例如 React Native），让开发更加轻松；
Web 游戏：在网页中的小游戏，都可以使用 JavaScript 来实现；
后端 Web 应用开发：以前我们都是使用 JavaScript 来进行 Web 应用程序前端部分的开发，但随着 Node.JS（一个 JavaScript 运行环境）的出现，使得 JavaScript 也可以用来开发 Web 应用程序的后端部分。

## 如何学习

学习JavaScript，需先掌握[Javascript基础](https://docs.box3.codemao.cn/js-tutorial.html)，你可以依次掌握：
●变量、字符串、数字、数组等关键功能
●基础的运算符与逻辑
●条件语句、循环、函数等代码块
●对象与属性的学习和了解
●神奇代码岛相关的API的使用
●上手操作一些实例教程
学习过程，可以打开[地图编辑器(opens new window)](https://box3.codemao.cn/me/content?type=map)边操作变学习哦～当然，学习的方式方法不唯一
除了可以在神奇代码岛的API文档里阅读相关的资料，也可以在下面的外部学习资料里学习相关的内容

## 外部学习资料

●[MDN Web Docs(opens new window)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference)
●[RUNOOB.COM(opens new window)](https://www.runoob.com/js/js-tutorial.html)
●[语言中文网(opens new window)](http://c.biancheng.net/js/)
●还有，B站等视频网站也可以搜索相关的视频教学哦～

# 全局对象

在脚本中可全局访问的对象。
类、接口类型以及枚举值不在此列出，请查看对应目录下的内容。

全局变量

storage
• Conststorage: [GameStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/game_storage)
代表存储服务的全局对象。

voxels
• Constvoxels: [GameVoxels](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gkz7g1wazf5izpfy)
控制所有方块。

world
• Constworld: [GameWorld](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s)
代表游戏世界的全局对象。

## 🌍世界

概述
[GameWorld 世界](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s)

是整个游戏世界的主要接口，可以通过全局对象world 来使用它。
它对应涵盖了控制环境天气、物理重力、画面滤镜等全局场景属性，还可以在世界中创建、搜索实体，或监听世界中实体和玩家的碰撞、伤害、互动等事件。
在世界之下，还可以创造[GameZone 区域](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8)

对地图世界进行指定范围的定制。

类
●[GameWorld 世界](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s)

●[GameZone 区域](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8)

类型
●[GameSelectorString 选择器参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9)

●[GameWorldKeyframe 世界动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gz8i9v7feiuz8cm6)

●[GameZoneConfig 区域配置](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yiaupxo6r5es9wcw)

事件
几乎所有事件都能在world上进行监听。
●[GameChatEvent 聊天事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2)

●[GameDamageEvent 实体伤害事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)

●[GameDieEvent 实体死亡事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)

●[GameEntityContactEvent 实体碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)

●[GameEntityEvent 实体创建销毁事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d)

●[GameFluidContactEvent 液体碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)

●[GameInputEvent 玩家输入事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)

●[GameInteractEvent 实体互动事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/go3it5p7im5tonnk)

●[GamePurchaseSuccessEvent 购买成功事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oue67nqv8mfga7av)

●[GameRespawnEvent 实体复活事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)

●[GameTickEvent 时钟事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl)

●[GameTriggerEvent 区域触发事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)

●[GameVoxelContactEvent 方块碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)

## 🧱方块

概述
[GameVoxels 方块](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gkz7g1wazf5izpfy)

 是控制所有方块的接口，可通过全局对象voxels使用。
它负责控制地形变化，利用循环语法批量生成/销毁方块，获取某个方块的类型、名称、旋转角度等。

类
●[GameFluidContact 液体碰撞数据](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/pdmg33m4vgx4t6bu)

●[GameVoxelContact 方块碰撞数据](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/le6z78ge7yokyxal)

●[GameVoxels 方块](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gkz7g1wazf5izpfy)

事件
●[GameFluidContactEvent 液体碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)

●[GameVoxelContactEvent 方块碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)

## 🏠实体

概述
实体是地图内的游戏对象，用于对物体、玩家等的控制。
实体对象类为[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)，可以通过[world.createEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#XvlaO)进行创建，或通过[world.querySelector](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#LzPJ7)等方法获取地图内已存在的实体对象。

类
●[GameEntity 实体](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)

●[GameEntityContact 实体碰撞参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tdvolpzhshdwfxri)

●[GameRaycastResult 射线检测结果](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)

类型
●[GameEntityConfig 实体配置参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vim7evgezkmnvhxk)

●[GameEntityKeyframe 实体动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/re5g6gz99r48fzi9)

●[GameHurtOptions 实体伤害参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dvgk7szaqicsyb4q)

事件
●[GameClickEvent 点击事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4)

●[GameDamageEvent 实体伤害事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)

●[GameDieEvent 实体死亡事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)

●[GameEntityEvent 实体创建销毁事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d)

●[GameEntityContactEvent 实体碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)

●[GameFluidContactEvent 液体碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)

●[GameInteractEvent 实体互动事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/go3it5p7im5tonnk)

●[GameVoxelContactEvent 方块碰撞事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)

## 👤玩家

玩家指的是进入地图游玩的用户，由 [GamePlayer 玩家](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)

 控制，此接口可用定义游戏中的玩家属性、操作等等。玩家属于一种特殊的[实体](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cxlovd92efvpx3ny)，可以在 [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)

 的player属性上读取到玩家对象。

类
●[GamePlayer 玩家](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)

●[GameWearable 穿戴配件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)

类型
●[GameDialogCall 显示对话框](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/extmobyyfsaec26x)

●[GamePlayerKeyframe 玩家动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/hgcguag2m8l09v1g)

●[GameSkinInvisible 隐藏身体部位参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/agf4z03gzqipg9mv)

枚举
●[GameBodyPart 身体部位](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fqfcrsh8mid6ook3)

●[GameDialogType 对话框类型](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)

●[GamePlayerMoveState 玩家运动状态](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zeoheeamz6dfaf60)

●[GamePlayerWalkState 玩家行走状态](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nfty4bko9nn3kyiv)

●[SocialType 玩家社交关系](https://box3.yuque.com/staff-khn556/wupvz3/bxykxeicwinbyle1)

事件
●[GameInputEvent 玩家输入事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)

●[GameRespawnEvent 实体复活事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)

## 🎯事件

概述
控制、处理事件流程的公共模块。有关具体事件的信息，请查阅对应功能模块。

类
●[GameEventHandlerToken 事件管理凭据](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/su72pndir0p5c7hh)

类型
●[GameEventChannel 事件频道监听](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)

●[GameEventFuture 事件单次监听](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)

## 🕺动作

动作模块负责控制由 Voxa 导入的模型所带有的动作。包括加载特定动作，暂停动作，重播动作和设置默认动作等，主要通过[GameMotionController 动作控制器](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dikrnsd8s0c3zuoc)

进行控制。
动作作为实体的一部分，可以通过[entity.motion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#ZNwcj)获取该实体的动作控制器。

类
●[GameMotionController 动作控制器](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dikrnsd8s0c3zuoc)

●[GameMotionHandler 动作处理器](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/czupdql58ligote4)

类型
●[MotionClipConfig 动作序列配置](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mglxkfvi4hga2g97)

●[MotionConfig 动作配置](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/grhrvh4gh1s1t7ni)

事件
●[GameMotionEvent 动作事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eplk4m6wyt4gymk6)

## 💃动画

概述
通过动画模块，可以对[GameWorld](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s)、[GameEntity-bean](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)、[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)

 对象添加关键帧动画。动画将在本地播放运行，获得更好的性能，播放更流畅、平滑。
通过对应对象上的animate方法可以创建动画对象 [GameAnimation-bean](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ritpgy64d053qg64)，从而控制动画的播放。

类
●[GameAnimation 动画](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ritpgy64d053qg64)

类型
●[GameAnimationPlaybackConfig 动画播放配置参数](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk)

●[GameEntityKeyframe 实体动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/re5g6gz99r48fzi9)

●[GamePlayerKeyframe 玩家动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/hgcguag2m8l09v1g)

●[GameWorldKeyframe 世界动画关键帧](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gz8i9v7feiuz8cm6)

枚举
●[GameAnimationDirection - 动画播放方向](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cgylgydyg35npvup)

●[GameAnimationPlaybackState 动画播放状态](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wmi50cpmg29sg5up)

●[GameEasing 缓动效果](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)

事件
●[GameAnimationEvent 动画事件](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)

## 📈数据存储

概述
数据存储模块，管理游戏中的数据。

类
●[GameDataStorage 数据存储空间](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)

●[GameStorage 数据存储模块](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/game_storage)

●[QueryList 数据查询列表](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181)

类型
●[JSONValue 类JSON格式](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tgkiwinql39mrrc7)

●[ListPageOption 列表翻页配置](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ugyg698kg8940k4d)

●[ReturnValue 数据查询返回](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)

# Classes-类

## GameAnimation 动画

类 - GameAnimation
Animation 动画，可对World世界、Entity实体及Player玩家等对象添加动画。动画将在本地播放运行，获得更好的性能，播放更流畅、平滑。

currentTime
•currentTime:number= 0
动画的当前播放时间（多少动画帧）

playState
•playState:[GameAnimationPlaybackState](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wmi50cpmg29sg5up)= GameAnimationPlaybackState.PENDING
当前动画播放状态

playbackRate
•playbackRate:number= 1
每tick动画播放速度

startTime
•startTime:number= 0
动画开始的时间tick

target
•target:TargetType
动画作用的对象（可为world、player或entity）

控制动画播放

play
•play:function
播放或者恢复动画的播放

函数声明:
▸ (playback?: Partial‹[GameAnimationPlaybackConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk)›):void
参数:

| 名称      | 类型                                                                                                       |
| --------- | ---------------------------------------------------------------------------------------------------------- |
| playback? | Partial‹[GameAnimationPlaybackConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk)› |

cancel
•cancel: *function
取消当前播放的动画

和动画有关的事件

onFinish
•onFinish:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)‹KeyframeType, TargetType››
•nextFinish:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)‹KeyframeType, TargetType››
当动画结束播放时触发

onReady
•onReady:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)‹KeyframeType, TargetType››
• nextReady: [GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)‹KeyframeType, TargetType››
当动画开始播放时触发

方法

keyframes
•keyframes:function
返回所有的动画关键帧

函数声明：
▸ ():Partial‹KeyframeType›[]

then
▸then‹T›(resolve: function,reject?: undefined | function):any
类型参数
▪T
参数:
▪resolve:function
▸ (event:[GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg)‹KeyframeType, TargetType›):T
参数:

| 名称  | 类型                                                                                                                |  |
| ----- | ------------------------------------------------------------------------------------------------------------------- | - |
| event | [GameAnimationEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oeb04fye24vyeicg) ‹KeyframeType, TargetType› |  |

▪可选reject:undefined | function
返回值:any

## GameBounds3 3维空间

类 - GameBounds3
GameBounds用于指定世界中一个立方体空间区域。

构造函数
+new GameBounds3(lo:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc),hi:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)):[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)
新建一个区域
参数:

| 名称 | 类型                                                                            | 说明           |  |
| ---- | ------------------------------------------------------------------------------- | -------------- | - |
| lo   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 区域的低处顶点 |  |
| hi   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 区域的高处顶点 |  |

返回值:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)

属性

hi
区域的高处顶点
•hi:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)

lo
区域的低处顶点
•lo:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)

方法

copy
▸copy(b:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)):[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)
参数:

| 名称 | 类型                                                                            |  |
| ---- | ------------------------------------------------------------------------------- | - |
| b    | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb) |  |

返回值:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)

set
▸set(lox: number,loy: number,loz: number,hix: number,hiy: number,hiz: number):void
参数:

| 名称 | 类型   |  |
| ---- | ------ | - |
| lox  | number |  |
| loy  | number |  |
| loz  | number |  |
| hix  | number |  |
| hiy  | number |  |
| hiz  | number |  |

返回值:void

intersect
▸intersect(b:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)):[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)
参数:

| 名称 | 类型                                                                            | 说明                     |  |
| ---- | ------------------------------------------------------------------------------- | ------------------------ | - |
| b    | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb) | 计算与此包围盒相交的部分 |  |

intersects
▸intersects(b:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)):boolean
参数:

| 名称 | 类型                                                                            | 说明                   |  |
| ---- | ------------------------------------------------------------------------------- | ---------------------- | - |
| b    | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb) | 检测是否与此包围盒相交 |  |

返回值:boolean

contains
▸contains(b:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)):boolean
参数:

| 名称 | 类型                                                                            | 说明                   |  |
| ---- | ------------------------------------------------------------------------------- | ---------------------- | - |
| b    | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 检测是否包围了这个3d点 |  |

返回值:boolean

containsBounds
▸containsBounds(b:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)):boolean
参数:

| 名称 | 类型                                                                            | 说明                   |  |
| ---- | ------------------------------------------------------------------------------- | ---------------------- | - |
| b    | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb) | 检测是否完全包围了此盒 |  |

返回值:boolean

toString
▸toString():string
返回值:string

StaticfromPoints
▸fromPoints(...points: [[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)](%5BGameVector3%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc))):[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)
参数:

| 名称      | 类型                                                                                                                                                                      | 说明                               |  |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- | - |
| ...points | [[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)](%5BGameVector3%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)) | 任意数量的3d坐标点, 用来形成包围盒 |  |

返回值:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)

## GameChatEvent 聊天事件

类 - GameChatEvent
由聊天触发的事件 通过[GameWorld.onChat](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#PRROA)和[GamePlayer.onChat](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#lDN5j)触发

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
发起聊天的实体

message
•message:string
聊天事件中说话的内容

tick
•tick:number
聊天事件发生时间

## GameClickEvent 点击事件

类 - GameClickEvent
当玩家用鼠标点击实体时触发的事件

button
•button:[ACTION0](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)|[ACTION1](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)
被点击的按钮，ACTION0 = 左键，ACTION1 = 右键

clicker
•clicker:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)& object
发起点击事件的玩家

clickerPosition
•clickerPosition:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
点击鼠标的瞬间玩家所在位置

distance
•distance:number
玩家到被点击实体的距离

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
被点击的实体

raycast
•raycast:[GameRaycastResult](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)
玩家 -> 被点击实体的射线检测结果

tick
•tick:number
鼠标点击事件发生的时间

## GameDamageEvent 实体伤害事件

类 - GameDamageEvent
当实体收到伤害时触发的事件，由[GameWorld](https://docs.box3.codemao.cn/box3world.html).[onTakeDamage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#MSnaO)和[GameEntity](https://docs.box3.codemao.cn/box3entity.html).[onTakeDamage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#TLS2e)触发

tick
•tick:number
事件发生的时间

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
受到伤害的实体

damage
•damage:number
伤害值的大小

attacker
•attacker:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)|null
攻击者

damageType
•damageType:string
伤害的类型

## GameDataStorage 数据存储空间

Class: GameDataStorage
    代表数据存储空间的类，能通过 {GameStorage.getDataStorage} 或 {GameStorage.getGroupStorage} 创建。能够以键值对的形式存储数据，提供方法处理空间内键值对相关的操作。

 存储空间隔离
当游戏服务器尝试连接指定名称的空间时：

- 不同地图的服务器，连接到的空间不同
- 同一地图不同服务器，连接到的空间相同
- 编辑模式与游戏服务器连接的空间不同

属性与方法

key
• key: string
空间名称 （只读）

示例代码

set
• set : function
传入指定键与值，无论该键是否存在，均将值设置到此键上。

函数声明:
▸ (key:string, value:[JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tgkiwinql39mrrc7)): Promise `<void>`

参数:

| 名称  | 类型                                                                          |              |
| ----- | ----------------------------------------------------------------------------- | ------------ |
| key   | string                                                                        | 需要设置的键 |
| value | [JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tgkiwinql39mrrc7) | 需要设置的值 |

返回值:Promise `<void>`
当设置完成时 resolve，否则 reject

get
• get : function
获取指定键对应的值

函数声明:
▸ (key:string): Promise[[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)](%5BReturnValue%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))

参数:

| 名称 | 类型   |          |
| ---- | ------ | -------- |
| key  | string | 指定的键 |

返回值:Promise[[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)](%5BReturnValue%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))
返回 Promise 对象，当获取完成时 resolve，否则 reject，resolve 时返回对应{ ReturnValue | 键值对内容}。

update
• update : function
使用传入的方法更新键值对

函数声明:
▸ (key:string, handler:(prevValue: [ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))=>[JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tgkiwinql39mrrc7)): Promise `<void>`

参数:

| 名称    | 类型                                                                                                                                                                       |                                                                |
| ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| key     | string                                                                                                                                                                     | 需要更新的键                                                   |
| handler | (prevValue:[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))=>[JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tgkiwinql39mrrc7) | 处理更新的方法，接受一个参数，为当前键的值，返回一个更新后的值 |

返回值:Promise `<void>`
返回 Promise 对象，当更新完成时 resolve，否则 reject。

remove
• remove : function
删除指定键值对

函数声明:
▸ (key:string): Promise[[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)](%5BReturnValue%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))

参数:

| 名称 | 类型   |          |
| ---- | ------ | -------- |
| key  | string | 指定的键 |

返回值:Promise[[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)](%5BReturnValue%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7))
返回 Promise 对象，resolve 时返回被删除的 { [ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7) | 键值对内容}。

list
• list : function
批量获取键值对

函数声明:
▸ (options:[ListPageOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ugyg698kg8940k4d)): Promise[[QueryList](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181)](%5BQueryList%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181))

参数:

| 名称    | 类型                                                                                |                        |
| ------- | ----------------------------------------------------------------------------------- | ---------------------- |
| options | [ListPageOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ugyg698kg8940k4d) | 批量获取键值对的配置项 |

返回值:Promise[[QueryList](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181)](%5BQueryList%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181))
返回 Promise 对象，resolve 时返回{ [QueryList](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dw93mzb6q0d5d181) | 键值对查询表}。

操作频率限制

服务器维度
对每一个游戏服务器独立生效，与服务器在线玩家数正相关，同一队列中的所有API共享限制。

| 队列 | API              | 限制                               |
| ---- | ---------------- | ---------------------------------- |
| 写入 | set updateremove | （60 + 玩家数 * 10 ）次操作 / 分钟 |
| 读取 | get update       | （120 + 玩家数*20）次操作/分钟     |

注；当前版本下，此处玩家数取固定值70。

吞吐量维度
对每一个 Key 的任意操作有吞吐量的限制。

| 队列 | API              | 限制    |
| ---- | ---------------- | ------- |
| 写入 | set updateremove | 4M/min  |
| 读取 | get update       | 25M/min |

错误码

| Code | Status             | Error Message              | 描述                               |
| ---- | ------------------ | -------------------------- | ---------------------------------- |
| 400  | DB_NAME_INVALID    | Invalid data storage name. | 存储空间名为空，或不满足限制要求。 |
| 400  | KEY_INVALID        | Invalid data key.          | 数据键为空。                       |
| 400  | VALUE_INVALID      | Invalid data value.        | 数据值为空。                       |
| 400  | PARAMS_INVALID     | Invalid parameters.        | 参数不合法。                       |
| 429  | REQUEST_THROTTLED  | Too Many Requests          | 超出操作频率限制                   |
| 500  | SERVER_FETCH_ERROR | Server network error.      | 服务由于网络原因请求失败。         |
| 500  | UNKNOWN            | Unknown server error.      | 未知的服务器错误。                 |

示例代码

```javascript
console.clear()

const testStorage = storage.getDataStorage('test')

async function storageExample() {

    await testStorage.set('keyNumber', 1)

    await testStorage.set('keyStr', '字符串')

    await testStorage.set('keyBoolean', false)

    await testStorage.set('keyJson', { describe: 'json内容' })

    let numberValue = await testStorage.get('keyNumber')

    let strValue = await testStorage.get('keyStr')

    let boolValue = await testStorage.get('keyBoolean')

    let jsonValue = await testStorage.get('keyJson')

    console.log(`keyNumber 的 value： ${numberValue.value}`)

    console.log(`keyStr 的 value： ${strValue.value}`)

    console.log(`keyBoolean 的 value： ${boolValue.value}`)

    console.log(`keyJson 的 value： ${JSON.stringify(jsonValue.value)}`)

    await sleep(1000)

    numberValue = await testStorage.remove('keyNumber')

    strValue = await testStorage.remove('keyStr')

    boolValue = await testStorage.remove('keyBoolean')

    jsonValue = await testStorage.remove('keyJson')

    console.log('\n==========================\n\n')

    console.log(`keyNumber 的 value： ${numberValue}`)

    console.log(`keyStr 的 value： ${strValue}`)

    console.log(`keyBoolean 的 value： ${boolValue}`)

    console.log(`keyJson 的 value： ${JSON.stringify(jsonValue)}`)

    await sleep(1000)

    await testStorage.update('keyNumber', (preData) => { return 2 })

    await testStorage.update('keyStr', (preData) => { return '被更改的字符串' })

    await testStorage.update('keyBoolean', (preData) => { return true })

    await testStorage.update('keyJson', (preData) => { return { describe: 'json内容被更改' } })

    numberValue = await testStorage.get('keyNumber')

    strValue = await testStorage.get('keyStr')

    boolValue = await testStorage.get('keyBoolean')

    jsonValue = await testStorage.get('keyJson')

    console.log('\n==========================\n\n')

    console.log(`keyNumber 的 value： ${numberValue.value}`)

    console.log(`keyStr 的 value： ${strValue.value}`)

    console.log(`keyBoolean 的 value： ${boolValue.value}`)

    console.log(`keyJson 的 value： ${JSON.stringify(jsonValue.value)}`)

    await sleep(1000)

    console.log('\n==========================\n\n')

    const queryList = await testStorage.list({

    // 分页指针，用于指定本次获取的分页起点。

    cursor: 0,

    // 分页大小，一页内的数据量，默认100。

    pageSize: 100

    })

    while (true) {

    for (let value of queryList.getCurrentPage()) {

    console.log(`${value.key} 的 value：${JSON.stringify(value.value)}`)

    }

    // 假如为最后一页，退出循环

    if (queryList.isLastPage) break

    // 翻到下一页

    await queryList.nextPage()

    }

}

storageExample()
```

## GameDieEvent 实体死亡事件

类 - GameDieEvent
当实体死亡时触发的事件，由[GameWorld.onDie](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#fO5zM)和[GameEntity.onDie](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#A8ka7)触发

tick
•tick:number
事件发生的时间

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
死亡的实体

attacker
•attacker:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)|null
击杀者

damageType
•damageType:string
伤害的类型

## GameEntity 实体

类 - GameEntity
Entity实体是Box3中的游戏对象，用于对物体、玩家等的控制。

属性与方法

控制实体的外观
由[GameEntityConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vim7evgezkmnvhxk)实现

entity.mesh
•mesh:string= ""

实体形状数据(mesh)的hash。如果设为空字符串/''，则实体无mesh。 除非实体为玩家，否则设定实体的mesh之后，mesh就会用来计算实体的边界。
只有提前在场景中放置模型，才能获得模型的Mesh属性。
模型被放置后，会自动保存在文件列表中。模型文件对应的*'mesh/.vb'名称便是 mesh属性。
示例代码

entity.position
• position: [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<> = new GameVector3(0, 0, 0)
实体的位置。
示例代码

entity.meshOrientation
• meshOrientation: [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)<> = new GameQuaternion(0, 0, 0, 1)
实体的旋转角度

entity.lookAt
(targetPosition:[GameVector3](https://box3.yuque.com/staff-khn556/wupvz3/lqqc61nd3gud9omc), meshFacing?:"X"|"Y"|"Z", up?:[GameVector3](https://box3.yuque.com/staff-khn556/wupvz3/lqqc61nd3gud9omc)) : void
将实体旋转至面向指定位置的方向，与图形学中定义的 LookAt 矩阵不是一个东西哦。
通过此方法进行的旋转会瞬时发生，仅影响实体的朝向，不会影响实体的运动状态。
●position:[GameVector3](https://box3.yuque.com/staff-khn556/wupvz3/lqqc61nd3gud9omc) - 世界坐标，希望让实体朝向的位置
●meshFacing:"X"|"Y"|"Z" - 定义模型在未旋转状态下的参考方向，处理模型设计时未朝向Z轴时的情况：
○当取X、Z时，定义模型的正方向分别为X、Z轴正方向，上方向为 Y 轴正方向
○当取Y时，定义模型的正方向为Y轴正方向，上方向为Z轴正方向
○默认值为Z，即模型设计时朝向Z轴正方向
●up:[GameVector3](https://box3.yuque.com/staff-khn556/wupvz3/lqqc61nd3gud9omc) - 上向量，默认取 Y 轴正方向

entity.meshScale
• meshScale: [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<> = new GameVector3(1 / 64, 1 / 64, 1 / 64)
实体的缩放比例

entity.meshColor
• meshColor: [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)<> = new GameRGBAColor(1, 1, 1, 1)
实体的颜色

entity.meshInvisible
•meshInvisible:boolean= false
可控制实体隐形，当值设为true时，则实体隐形。

entity.meshEmissive
• meshEmissive: number = 0
实体的发光度

entity.meshMetalness
• meshMetalness: number = 0
实体的金属感

entity.meshShininess
• meshShininess: number = 0
实体的反光度，设为1则为非常光滑

entity.meshOffset
•meshOffset:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(0, 0, 0)
实体的位移

控制实体的物理属性
由[GameEntityConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vim7evgezkmnvhxk)实现

entity.bounds
•bounds:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(1, 1, 1)
实体边界框的半径，沿着x/y/z方向，这是一个只读属性，每帧都会重新计算

entity.collides
• collides: boolean = true
如果为假(false)，则实体不会碰撞

entity.fixed
• fixed: boolean = false
如果为真(true)，则实体不会移动

entity.friction
• friction: number = 0
控制实体的粘性(0 = 滑，1 = 粘)

entity.gravity
• gravity: boolean = true
如果为假(false)，则实体不会下落
示例代码

entity.mass
• mass: number = 1
实体物理质量

entity.restitution
• restitution: number = 0
控制实体的弹性(0 = 软, 1 = 弹)

entity.velocity
• velocity: [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<> = new GameVector3(0, 0, 0)
实体的速度
示例代码

entity.contactForce
•contactForce:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(0, 0, 0)
实体受到的碰撞力

entity.entityContacts
•entityContacts:[GameEntityContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/tdvolpzhshdwfxri)[] = []
返回正在和玩家/实体发生碰撞的全部实体列表

entity.voxelContacts
•voxelContacts:[GameVoxelContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/le6z78ge7yokyxal)[] = []
返回正在和玩家/实体发生碰撞的全部方块列表

entity.fluidContacts
•fluidContacts:[GameFluidContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/pdmg33m4vgx4t6bu)[] = []
返回正在被玩家/实体触碰的全部液体方块列表

聊天

entity.say
•say(message: string):void
让实体说话。
示例代码

互动
允许实体进行互动

entity.enableInteract
•enableInteract:boolean= false
是否允许实体进行互动。如果允许互动，走进互动范围之内，实体身上将会出现互动提示。

实体互动范围

entity.interactRadius
•interactRadius:number= 16
实体互动范围。数值越小，则需要靠近实体才会出现互动提示。
范围有多个可互动实体，按下键盘[或]键，切换互动目标。

互动提示文本

entity.interactHint
•interactHint:string= ""
进入实体互动范围时，实体身上出现的提示文本。

互动提示文本颜色

entity.interactColor
•interactColor:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(1, 1, 1)
进入实体互动范围时，提示文本的颜色。
示例代码
与实体互动之前，在场景中必须先有一个实体。
在模型列表中，挑选一个你喜欢的模型，将它放置在场景中，并记住模型的名字。

和实体有关的事件

entity.onClick
•onClick:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameClickEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4)](%5BGameClickEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4))
•nextClick:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameClickEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4)](%5BGameClickEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4))
当玩家用鼠标点击实体时触发的事件

entity.onEntityContact
•onEntityContact:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
•nextEntityContact:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
当实体触碰另一个实体时触发

entity.onEntitySeparate
•onEntitySeparate:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
•nextEntitySeparate:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
当实体停止触碰另一个实体时触发

entity.onFluidEnter
•onFluidEnter:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
•nextFluidEnter:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
当实体进入液体时触发

entity.onFluidLeave
•onFluidLeave:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
•nextFluidLeave:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
当实体离开液体时触发

entity.onInteract
•onInteract:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameInteractEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/go3it5p7im5tonnk)›
•nextInteract:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameInteractEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/go3it5p7im5tonnk)›
当实体进行互动时触发
示例代码

entity.onVoxelContact
•onVoxelContact:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
•nextVoxelContact:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
当实体触碰方块时触发

entity.onVoxelSeparate
•onVoxelSeparate:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
•nextVoxelSeparate:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
当实体停止触碰方块时触发

控制玩家

entity.isPlayer
•isPlayer:boolean= false
如果为真，则实体为玩家

Optionalplayer
•player? :[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)
索引与玩家相关的全部状态和方法

快速查找实体

entity.addTag
为实体添加一个新标签
函数声明:
▸addTag(tag: string):void
参数

| 名称 | 类型   | 说明           |
| ---- | ------ | -------------- |
| tag  | string | 要添加的标签名 |

entity.hasTag
判断实体是否带有某个标签
函数声明:
▸hasTag(tag: string):boolean
参数

| 名称 | 类型   | 说明   |
| ---- | ------ | ------ |
| tag  | string | 标签名 |

示例代码

entity.id
•id:string= ""
已在编辑器中添加的实体名称

entity.removeTag
从实体移除标签
函数声明:
▸removeTag(tag: string):void
参数

| 名称 | 类型   | 说明           |
| ---- | ------ | -------------- |
| tag  | string | 要移除的标签名 |

entity.tags
在编辑器中给实体添加的全部标签

函数声明:
▸tags():string[]

实体的销毁

entity.destroy
•destroy:function
销毁实体
函数声明:
▸destroy():void

entity.destroyed
•destroyed:boolean= false
如果为真(true)，实体就被销毁。

entity.onDestroy
•onDestroy:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameEntityEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d)](%5BGameEntityEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d))
•nextDestroy:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameEntityEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d)](%5BGameEntityEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d))
当实体被销毁时触发

控制实体的生命值

entity.enableDamage
•enableDamage:boolean= false
如果为真true，则可对实体进行伤害

entity.showHealthBar
•showHealthBar:boolean= true
如果为真true，则显示实体的生命值HP

entity.hp
•hp:number= 100
实体的当前生命值hp

entity.maxHp
•maxHp:number= 100
实体的最大生命值hp

entity.onTakeDamage
实体受到伤害时触发的事件
•onTakeDamage:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameDamageEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)](%5BGameDamageEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm))
•nextTakeDamage:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameDamageEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)](%5BGameDamageEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm))

entity.onDie
实体死亡时触发的事件
•onDie:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameDieEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)](%5BGameDieEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y))
•nextDie:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameDieEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)](%5BGameDieEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y))

entity.hurt
可用这个函数来定义对实体的伤害。输入对实体的伤害值。
函数声明:
▸hurt(amount: number,options?:Partial[[GameHurtOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dvgk7szaqicsyb4q)](%5BGameHurtOptions%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dvgk7szaqicsyb4q))):void
参数

| 名称     | 类型                                                                                                                                                                                                  | 说明                 |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------- |
| amount   | number                                                                                                                                                                                                | 伤害值               |
| options? | Partial[[GameHurtOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dvgk7szaqicsyb4q)<br />>](%5BGameHurtOptions%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dvgk7szaqicsyb4q)%3Cbr/) | 伤害的相关配置，选填 |

代码示例

控制实体产生粒子的属性

entity.particleRate
•particleRate:number= 0
实体平均每秒产生粒子的数量。如果希望实体停止释放粒子，可以将该属性改为0
示例代码

entity.particleRateSpread
•particleRateSpread:number= 0
如果设定了该属性的值，实体每一秒产生粒子的数量将不再是个固定值，而是从区间 [particleRate,particleRate+particleRateSpread) 里随机选取的一个整数。例如，假设particleRate=0，particleRateSpread=3，每秒产生的粒子数量是[0, 0+3) ，即[0, 3)区间里的一个随机整数，也就是可能为0，1，或2
示例代码

entity.particleLimit
•particleLimit:number= 100
实体可产生的粒子总数的上限

entity.particleLifetime
•particleLifetime:number= 10
粒子的存活时间，以秒为单位
示例代码

entity.particleLifetimeSpread
•particleLifetimeSpread:number= 0
如果设定了该属性的值，粒子的存活时间将不再是固定值，而是区间 [particleLifetime,particleLifetime+particleLifetimeSpread) 里的一个随机数，可能为小数
示例代码

entity.particleSize
•particleSize:number[]= [1, 1, 1, 1, 1]
该属性的值可以是一个长度为0至5的数组。每个粒子的存活时间被平均分为五个阶段，对于长度为5的数组，数组里的每个值分别指定粒子在各个阶段的大小，其中，第一个值为粒子刚产生是的大小，第五个值为粒子消失时的大小。举几个例子，假设粒子的存活时间被设定为5秒，如果particleSize的值为
●[25, 25, 25, 25, 25]，在粒子存活的5秒内大小不会发生变化，产生时是25，消失时也是25
●[0, 25, 0, 25, 15]，粒子产生时大小为0，然后逐渐变为25，之后又逐渐变为0，再逐渐变为25，最后变为15，可以让该实体所产生的粒子具有逐渐放大缩小的效果
●[15， 25], 粒子产生时大小为15，1秒后逐渐变大至25，之后又逐渐缩小至最小值
示例代码

entity.particleSizeSpread
•particleSizeSpread:number= 0
●如果设定了该属性，但没设定particleSize的值，每产生一个粒子，会从区间[0，particleSizeSpread)里选取的一个随机数作为它的大小
●如果同时设定了particleSize和particleSizeSpread两个属性，每产生一个粒子，从区间[0，particleSizeSpread)里选取一个随机数x，这个粒子第i个阶段的大小将为particleSize[i]+x

entity.particleColor
•particleColor:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)[]= [ new GameRGBColor(1,1,1), new GameRGBColor(1,1,1), new GameRGBColor(1,1,1), new GameRGBColor(1,1,1), new GameRGBColor(1,1,1) ]
类似particleSize，该属性的值可以是一个长度为0至5的数组，数组里的每个值分别指定了粒子在各个阶段的颜色。类似地，可以通过该属性使粒子具有颜色渐变的效果
示例代码

entity.particleVelocity
•particleVelocity:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)= new GameVector3(0, 0, 0)
该实体产生的所有粒子的初始速度，如果将该属性设为new GameVector3(x, y, z)，x，y，z三个值分别指定粒子在对应三个方向上的速率
示例代码

entity.particleVelocitySpread
•particleVelocitySpread:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)= new GameVector3(0, 0, 0)
增加该实体产生的所有粒子初始速度的不确定性，如果将该属性设为new GameVector3(sx, sy, sz)，每产生一个粒子，会基于这三个值分别产生一个随机值加到 x/y/z 三个方向所对应的速率上。通过设定这个属性，可以使粒子具有向随机方向运动的效果
示例代码

entity.particleDamping
•particleDamping:number= 0
●如果该属性的值为正数，会短暂减少该实体所产生粒子的初始速度，数值越大，减少初始速度的效果持续得越久
●如果为负值，会短暂增加粒子的初始速度，数值越小，增加初始速度的效果越明显
示例代码

entity.particleAcceleration
•particleAcceleration:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)= new GameVector3(0, 0, 0)
该实体所产生粒子的加速度

entity.particleNoise
•particleNoise:number= 0
指定粒子相对于之前运动方向的最大偏离值，数值越大，各个粒子的运动相对原有方向的偏离越明显

entity.particleNoiseFrequency
•particleNoiseFrequency:number= 1
指定粒子改变运动方向的频率，数值越大，各个粒子的运动方向越没有规律
示例代码

控制音效
上传音效
编辑器目前内置了34款音效，可以在菜单-[文件管理]的搜索.mp3查看。点击文件后，会弹出声音文件的详情属性。点击位置即可复制文件路径，在脚本中使用对应的方法播放。
如需上传自定义声音，可以在[文件管理]窗口，点击右下角浮动的加号按钮-[上传音频]。
属性

entity.chatSound
•chatSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当实体说话时，播放聊天音效。默认为'audio/chat.mp3'。通过entity.say()触发。

entity.hurtSound
•hurtSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当实体触发受伤事件时，播放受伤音效。默认为'audio/hurt.mp3'。通过entity.onTakeDamage()触发

entity.dieSound
•dieSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当实体触发死亡事件时，播放死亡音效。默认为'audio/die.mp3'。通过entity.onDie()触发

entity.interactSound
•interactSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当实体进行互动时，播放互动音效。此音效仅互动的玩家可听见。通过entity.onInteract()触发。

方法

entity.sound
•sound:function
在实体的位置播放声音。
参数
spec:{sample, radius, gain, pitch} | string
●sample:string 必填，声音文件路径。可在文件管理器中上传自定义声音。如'audio/chat.mp3'
●radius?:number 可选，声音范围。默认为32。距离实体越近，声音听的越清晰。超出范围的玩家则听不到声音。
●gain?:number 可选，音量增益。正常为1，数值越大，声音越响。
●pitch?:number 可选，音高增益。正常为1，大于1，声音播放越快，小于1，声音播放越慢。
示例1

示例2

示例3

动画

entity.animate
可用这个函数来设定实体的动画轨迹
函数声明:
▸animate(keyframes:[GameEntityKeyframe](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/re5g6gz99r48fzi9)[],playbackInfo:Partial[[GameAnimationPlaybackConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk)](%5BGameAnimationPlaybackConfig%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk))):[GameAnimation](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ritpgy64d053qg64)
代码示例

```javascript
//需要提前在编辑器中添加'单元方块'的模型。

const vox = world.querySelector('#单元方块-1') //获取实体

vox.meshScale = vox.meshScale.scale(4) //让实体变大4倍

const ani = vox.animate([

  { position: [0, 12, 0], meshColor: [1, 1, 0, 1] },

  { position: [0, 12, 127], meshColor: [1, 0, 0, 1] },

  { position: [127, 12, 127], meshColor: [0, 1, 0, 1] },

  { position: [127, 12, 0], meshColor: [0, 0, 1, 1] },

], {

  iterations: 3,//兜3圈

  direction: GameAnimationDirection.WRAP,//从终点回到起点

  duration: 16 * 5, //兜一圈5秒(每秒16帧)

})

ani.onReady(() => {//当动画开始播放时

  world.say('开始兜圈')

})

ani.onFinish(() => {//当动画结束播放时

  world.say('兜圈结束')

})
```

动作

entity.motion
• motion: [GameMotionController](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dikrnsd8s0c3zuoc)<> = new [GameMotionController](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dikrnsd8s0c3zuoc)()
实体动作控制器
代码示例

```javascript
const entity = world.querySelector('#npc')

const entityMotionControl = entity.motion; // MotionController

const motion = entityMotionControl.loadByName('hello'); // MotionHandler 'hello'指代'npc'实体上的其中一个motion动作名称

motion.onFinish(() => {

  console.log('Motion End');

});

motion.play()
```

## GameEntityContact 实体碰撞参数

类 - GameEntityContact
正在发生碰撞的实体

other
•other:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
与此实体碰撞的另一个实体

axis
•axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
碰撞的分离轴，也就是碰撞后物体弹飞的方向

force
•force:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
碰撞所产生的力

## GameEntityContactEvent 实体碰撞事件

类 - GameEntityContactEvent
当两个实体碰撞时触发的事件。
由[GameWorld.onEntityContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#pI6Y2),[GameWorld.onEntitySeparate](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#gPBFQ),[GameEntity.onEntityContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#EM0Fn),[GameEntity.onEntitySeparate](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#VbAUD)触发

axis
•axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
碰撞的分离轴，也就是碰撞后物体弹飞的方向

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
碰撞中的第一个实体

force
•force:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
碰撞所产生的力

other
•other:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
碰撞中的第二个实体

tick
•tick:number
两个实体碰撞的时间

## GameEntityEvent 实体创建销毁事件

类 - GameEntityEvent
当创建或销毁实体时触发的事件。
由 [GameWorld.onPlayerJoin](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#P6gUg), [GameWorld.onPlayerLeave](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#mUHUB), [GameWorld.onEntityCreate](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#VHyc3), [GameWorld.onEntityDestroy](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#NIBv8) 和 [GameEntity.onDestroy](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#gRhnq) 触发

```javascript
world.onPlayerJoin((entityEvent) => {

    // entityEvent.entity

    // entityEvent.tick

});
```

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
创建/销毁的实体

tick
•tick:number
事件发生时间

## GameEventHandlerToken 事件处理器

类 - GameEventHandlerToken
当事件监听被触发时，由 [GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)

 返回的token，可用于取消事件监听。

cancel
取消事件监听

函数声明:
▸cancel():void

resume
恢复事件监听

函数声明:
▸ resume(): void

事件列表:
●[GameTickEvent 时钟](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl)
●[GameClickEvent 点击](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/mtb7dirtqv6g83o4)
●[GameInputEvent 输入](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)
●[GameChatEvent 聊天](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2)
●[GameInteractEvent 互动](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/go3it5p7im5tonnk)
●[GameEntityEvent 实体创建/销毁](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/dcqt2gzgkxnxqt2d)
●[GameEntityContactEvent 实体触碰](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)
●[GameVoxelContactEvent 触碰方块](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)
●[GameFluidContactEvent 触碰液体](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)
●[GameDamageEvent 实体伤害](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)
●[GameDieEvent 实体死亡](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)
●[GameTriggerEvent 区域触碰](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)

## GameFluidContact 液体碰撞数据

类 - GameFluidContact
被实体/玩家触碰的液体方块。

voxel
•voxel:number
液体方块id

volume
•volume:number
液体方块中，被玩家或实体进入的体积比例，大小为(0,1]

## GameFluidContactEvent 液体碰撞事件

 当实体进入或离开液体时触发的事件。
由 [GameWorld.onFluidEnter](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#ZxpSh), [GameWorld.onFluidLeave](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#mPt0K), [GameEntity.onFluidEnter](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#xFbGB), [GameEntity.onFluidLeave](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#qkPb7) 触发

```javascript
world.onFluidEnter(({entity, tick, voxel}) => {

})
```

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
触碰液体的实体

tick
•tick:number
实体进入或离开液体的时间

voxel
•voxel:number
液体方块id

## GameInputEvent 玩家输入事件

类 - GameInputEvent
输入事件，在玩家按下或松开按钮时触发。
事件发生的时刻，即为玩家按下/松开按钮的同一刻。
由[GameWorld.onPress](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#icj8F),[GameWorld.onRelease](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#dRB7i),[GamePlayer.onPress](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#O5SsB),[GamePlayer.onRelease](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#CenKW)触发。
示例代码

点击左键，将鼠标指针位置的方块替换为石头。点击右键，销毁方块。

button
•button:[GameButtonType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)
玩家输入的按钮

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)& object
指向按下/松开按钮的玩家

position
•position:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
玩家按下/松开按钮的瞬间所在位置

pressed
•pressed:boolean
如果为真，则事件为按下按钮，否则，为松开按钮。

raycast
•raycast:[GameRaycastResult](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)
按下/松开按钮的瞬间，从玩家视角投射的射线检测结果。

tick
•tick:number
按下/松开按钮的时间

## GameInteractEvent 实体互动事件

类 - GameInteractEvent

参数
●entity
●targetEntity
●tick

参数

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
发起互动的实体

targetEntity
•targetEntity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
收到互动请求的实体

tick
•tick:number
事件发生时间

## GameMotionController 动作控制器

类 - GameMotionController
Motion 动作，可对Entity实体带有的动作进行操作，包括加载特定动作，暂停动作，重播动作和设置默认动作等。

示例代码
 播放动作

加载特定动作

loadByName
•  loadByName : function
加载特定动作或动作序列，并返回对应的动作对象

函数声明:
▸ ( configs : "string" | [MotionConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/docs/pqaedvg6kom5g2g7)[] | [MotionClipConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/docs/rsefcstdog725s5p)): [GameMotionHandler](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/czupdql58ligote4)
参数:

| 名称    | 类型   |
| ------- | ------ |
| configs | string |

返回值:[GameMotionHandler ](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/czupdql58ligote4)

控制动作播放

pause
• pause  : function
暂停实体上的动作播放

函数声明：
▸ (): void

resume
• resume   : function
恢复实体上的动作播放

函数声明：
▸ (): void

设置默认动作

setDefaultMotionByName
• setDefaultMotionByName : function
 设置默认动作
●没有其他动作在播放的情况下，默认动作会在游戏运行时自动循环播放
●调用此函数时，如当前处于默认动作执行状态，则将打断旧默认动作，播放新的默认动作
●动作名不存在时，此方法不产生任何效果，并抛出包含实体、模型与动作信息的错误

函数声明：
▸ ( motionName : undefined | string):  void
参数:

| 名称       | 类型      |
| ---------- | --------- |
| motionName | undefined |

返回值: void

示例代码

```javascript
const entity = world.querySelector('#npc')

entity.motion.setDefaultMotionByName('FirstMotion');

entity.motion.setDefaultMotionByName(''); // 报错，不存在对应动作

entity.motion.setDefaultMotionByName(); // 设置默认动作为空，即不播放默认动作
```

## GameMotionEvent 动作事件

类 - GameMotionEvent
动作事件，通过GameMotionHandler.onFinish触发

cancelled
•cancelled: bool
动画是否被取消

## GameMotionHandler 动作处理器

类 - GameMotionHandler
 动作播放的 Handler，用于处理动作中断等行为

示例代码
 播放动作

基本

target
• target : GameEntity
当前motion的entity对象

控制动作播放

play
• play  : function
 播放当前实体动作
●会打断当前动作，开始对应动作/序列动作的播放
●当配置中包含的动作播放结束时，触发 MotionPlayHandler 的 Finish 事件。

函数声明：
▸ (): void

返回值: void

示例代码

```javascript
const entity = world.querySelector('#npc')

const motion = entity.motion.loadByName('FirstMotion');

motion.play()
```

cancel
• cancel  : function
中断此动作播放，并触发 end 事件

函数声明：
▸ (): void

播放结束事件

onFinish
• onFinish : [GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameMotionEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eplk4m6wyt4gymk6)›
• nextFinish: [GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameMotionEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eplk4m6wyt4gymk6)›
 响应结束状态的监听函数

## GamePlayer 玩家

类 - GamePlayer
Player 玩家指的是进入游戏的用户，此接口可用定义游戏中的玩家属性、操作等等。玩家属于一种特殊的[实体](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)。

基本

name
•name:string= "player"
玩家的昵称。无法控制更改。

boxId
•boxId:string= ""
玩家的Box ID(3-15字符)。无法控制更改。 游客的boxID值为空""。

userKey
•userKey:string= ""
玩家的唯一识别码(16字符)，可以用于存储玩家信息到数据库，无法控制更改。 游客的userKey值为空""。

avatar
string
玩家头像信息。

spawnPoint
•spawnPoint:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(64, 140, 64)
玩家的出生点。默认出生点设置在new GameVector3(64, 140, 64)

movementBounds
•movementBounds:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)<>= new[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)(new[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)(-50, -50, -50), new[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)(178, 178, 178));
玩家的活动范围限制，如超出此范围，则传回出生点

向玩家发送消息

directMessage
▸directMessage(message: string):void
向玩家直接发送私信

onChat
•onChat:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameChatEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2)](%5BGameChatEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2))
•nextChat:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameChatEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2)](%5BGameChatEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aft5xl7q0dh6puh2))
当发起聊天时调用

dialog
•dialog:[GameDialogCall](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/extmobyyfsaec26x)
在游戏中显示一个对话框。
示例代码 1

示例代码 2

cancelDialogs
•cancelDialogs:function
关闭该玩家的所有打开的对话框。

share
(content:string) : void;
为该玩家显示分享弹窗，并能够自定义分享内容。
●content - 分享弹窗的内容，限制长度为40个字以内，超出后截断，并在末尾添加省略号……。
自动标签
通过此 API 调用弹出的分享弹框的内容末尾，会自动新起一行添加#神奇代码岛 #地图标签，自动添加的内容不计入限制长度内。
编辑模式
编辑模式下，此API弹出的分享弹窗分享的地址是编辑模式的地址。

控制玩家的外观

color
•color:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)<>= new GameRGBColor(1, 1, 1)
玩家的颜色

emissive
•emissive:number= 0
玩家的发光度
示例代码

invisible
•invisible:boolean= false
玩家是否隐身
示例代码

skin
[SkinDescription](https://box3.yuque.com/staff-khn556/wupvz3/gwfba5hzun9bhseg)
此玩家的皮肤配置，用于管理当前玩家皮肤的展示。通过此处修改皮肤不会影响皮肤的隐藏状态，设置前是隐藏的，设置后也还是隐藏着。

皮肤不存在&非法参数
当皮肤名称不存在于项目皮肤库或不符合类型定义时，无事发生，并会在控制台打印警告。

示例

setSkinByName
(skinName:string) : void
将指定皮肤套装应用到此玩家上。此方法不会影响皮肤的隐藏状态，设置前是隐藏的，设置后也还是隐藏着。

参数
●skinName:string - 指定要设置的皮肤名称，将玩家皮肤整体替换为对应的皮肤。
皮肤不存在&非法参数
当皮肤名称不存在于项目皮肤库或不为字符串时，无事发生，并在控制台打印警告。

resetToDefaultSkin
() : void
重置此玩家的皮肤配置为默认皮肤配置，效果同 setSkinByName传入了默认皮肤套装名称。

clearSkin
() : void
清除地图对此玩家应用的皮肤配置，将此玩家的皮肤配置为仅展示玩家自己的皮肤。

skinInvisible
•skinInvisible:[GameSkinInvisible](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/agf4z03gzqipg9mv)
隐藏玩家模型部件接口
示例代码

showName
•showName:boolean= true
玩家名字是否显示

showIndicator
• showIndicator: boolean = false
玩家标记否显示

scale
•scale:number= 1
玩家的缩放比例
示例代码1

metalness
•metalness:number= 0
玩家的金属感

shininess
•shininess:number= 0
玩家的反光度

addWearable
•addWearable:function
在玩家某身体部位附上穿戴配件物体
函数声明:
▸ (spec: Partial‹[GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)›):[GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)
参数:

| 名称 | 类型                                                                                        |
| ---- | ------------------------------------------------------------------------------------------- |
| spec | Partial‹[GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)› |

示例代码

removeWearable
•removeWearable:function
把玩家身体部位已附上的穿戴配件物体删除
wearableis the wearable to remove
函数声明:
▸ (wearable:[GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)):void
参数:

| 名称     | 类型                                                                             |
| -------- | -------------------------------------------------------------------------------- |
| wearable | [GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x) |

示例代码

wearables
•wearables:function
列举在玩家上所有的穿戴配件物体
函数声明:
• (bodyPart?:[GameBodyPart](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fqfcrsh8mid6ook3)):[GameWearable](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/smdhl0l2qxg5we0x)[]
参数:

| 名称      | 类型                                                                             | 说明                 |
| --------- | -------------------------------------------------------------------------------- | -------------------- |
| bodyPart? | [GameBodyPart](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fqfcrsh8mid6ook3) | 某玩家身体部位，选填 |

示例代码

Web相关

link
•link:function
在玩家弹出一个“传送门”窗口，可以跳转到其他地图或任意链接。（目前支持神奇代码岛、编程猫、微信文章、Bilibili视频等链接）
函数声明:
▸ (href: string):void
参数:

| 名称 | 类型   | 说明     |
| ---- | ------ | -------- |
| href | string | 链接 URL |

示例代码

url
•url:[URL](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vvy0hopvp0bmgb1b)
获取该玩家进入地图时所用的URL链接地址, 主要用于获取URL参数, 以便区别对待进来的玩家
示例代码

玩家的复活和死亡

forceRespawn:()
让玩家强制重生，立即返回出生点
•forceRespawn(): void

onRespawn
玩家复活时调用的事件
•onRespawn:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameRespawnEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)](%5BGameRespawnEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr))
•nextRespawn:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameRespawnEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)](%5BGameRespawnEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr))

dead
玩家是否已死亡，生命值hp低于0。若玩家死亡，则会倒在地上。
•dead: boolean = false
此属性为只读，不可修改。

控制玩家视角

cameraEntity
•cameraEntity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)| null= null
在第一人称视角(FPS)或第三人称跟随视角(FOLLOW)下，玩家视角所跟随的实体

cameraMode
•cameraMode:[GameCameraMode](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kg0ggd71y96dlu0w)
视角模式
●GameCameraMode.FPS -"fps"- 第一人称视角
●GameCameraMode.FOLLOW -"follow"- 第三人称跟随视角(默认)
●GameCameraMode.FIXED -"fixed"- 第三人称固定视角
示例代码

cameraPosition
•cameraPosition:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(0, 0, 0)
固定视角(FIXED)下，镜头的眼睛位置

cameraTarget
•cameraTarget:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(0, 0, 0)
固定视角(FIXED)下镜头所朝向的目标点

cameraUp
•cameraUp:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(0, 1, 0)
固定视角(FIXED)下，镜头向上的矢量

cameraFovY
• cameraFovY: number  = 0.25
垂直方向的视场角

setCameraPitch
• setCameraPitch: function
设置玩家视角准心绕水平方向的旋转弧度
函数声明:
▸ (v: number): void
参数:

| 名称 | 类型   | 说明     |
| ---- | ------ | -------- |
| v    | number | 设置弧度 |

示例代码

setCameraYaw
• setCameraYaw: function
设置玩家视角准心绕垂直方向的旋转弧度
函数声明:
▸ (v: number): void
参数:

| 名称 | 类型   | 说明     |
| ---- | ------ | -------- |
| v    | number | 设置弧度 |

示例代码

enable3DCursor
•enable3DCursor:boolean= false
启动玩家的3D光标
示例代码

玩家的输入信息

enableAction0
●enableAction0:boolean= true
如果为false， 关闭Action0键。PC端为鼠标左键，手机端不会显示A按钮。
示例代码

启动鼠标左键/移动端虚拟按钮A键

enableAction1
●enableAction1:boolean= true
如果为false， 关闭ActionB键。PC端为鼠标右键，手机端不会显示B按钮。
启动鼠标右键/移动端虚拟按钮B键

action0Button
•action0Button:boolean= false
鼠标左键/移动端虚拟按钮A键

action1Button
•action1Button:boolean= false
鼠标右键/移动端虚拟按钮B键

crouchButton
•crouchButton:boolean= false
下蹲按钮

facingDirection
•facingDirection:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)<>= new GameVector3(1, 0, 0)
玩家朝向

cameraPitch
• cameraPitch: number= 0
玩家视角准心绕水平方向的旋转弧度 只读

cameraYaw
• cameraYaw: number= 0
玩家视角准心绕垂直方向的旋转弧度 只读
PITCHAXIS

ROLLAXIS

YAWAXIS

![image.png](https://cdn.nlark.com/yuque/0/2023/png/12895980/1694596903548-ac680c23-0a4d-4ed4-a2a6-7218836c44f3.png?x-oss-process=image%2Fformat%2Cwebp)

jumpButton
•jumpButton:boolean= false
跳跃按钮

onPress
•onPress:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameInputEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)](%5BGameInputEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx))
•nextPress:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameInputEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)](%5BGameInputEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx))
当玩家按下按钮时调用

onRelease
•onRelease:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameInputEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)](%5BGameInputEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx))
•nextRelease:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameInputEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx)](%5BGameInputEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yazeh0kkzogc71tx))
当玩家松开按钮时调用

walkButton
•walkButton:boolean= false
步行按钮

控制玩家的行动

canFly
•canFly:boolean= false
如果为真(true)，则允许玩家飞行
示例代码

spectator
•spectator:boolean= false
如果为真(true)，则玩家是一个幽灵，可以穿墙

enableJump
•enableJump:boolean= true
如果为假(false)，则不允许玩家跳跃
示例代码

enableDoubleJump
•enableDoubleJump:boolean= true
如果为假(false)，则不允许玩家二段跳跃
示例代码

walkSpeed
•walkSpeed:number= 0.22
最大步行速度

runSpeed
•runSpeed:number= 0.4
最大奔跑速度

runAcceleration
•runAcceleration:number= 0.35
奔跑加速度

jumpPower
•jumpPower:number= 0.96
跳跃力度

jumpSpeedFactor
•jumpSpeedFactor:number= 0.85
跳跃速度

jumpAccelerationFactor
•jumpAccelerationFactor:number= 0.55
跳跃加速率

doubleJumpPower
•doubleJumpPower:number= 0.9
二段跳力度

crouchSpeed
•crouchSpeed:number= 0.1
蹲着走路的速度

crouchAcceleration
•crouchAcceleration:number= 0.09
蹲着走路的加速度

flySpeed
•flySpeed:number= 2
最大飞行速度

flyAcceleration
•flyAcceleration:number= 2
飞行加速度

swimAcceleration
•swimAcceleration:number= 0.1
游泳加速度

swimSpeed
•swimSpeed:number= 0.4
最大游泳速度

walkAcceleration
•walkAcceleration:number= 0.19
步行加速度

disableInputDirection
[GameInputDirection](https://box3.yuque.com/staff-khn556/wupvz3/glhsleip3t0eqduh)
禁用指定方向的摇杆输入偏移量，当横纵两个方向均被禁用时，将不显示此玩家的触屏虚拟摇杆。

查看玩家的状态

moveState
•moveState=[GamePlayerMoveState](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zeoheeamz6dfaf60).FALL
玩家的运动状态，初始值为下落

walkState
•walkState=[GamePlayerWalkState](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nfty4bko9nn3kyiv).NONE
玩家的步行状态，初始值为非步行中

控制音效

预设音效

action0Sound
•action0Sound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家按下'action0'按键（鼠标左键 / 虚拟按钮A）时，播放的音效。

action1Sound
•action1Sound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家按下'action1'按键（鼠标右键 / 虚拟按钮B）时，播放的音效。

crouchSound
•crouchSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家按下'crouchButton '按键进行蹲下时，播放的音效。

jumpSound
•jumpSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家按下'jumpButton '按键进行跳跃时，播放的音效。默认为'audio/jump.mp3'

doubleJumpSound
•doubleJumpSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家触发二段跳时，播放的音效。默认为'audio/double_jump.mp3'

landSound
•landSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
玩家落地时，播放的音效。默认为'audio/land.mp3'

enterWaterSound
•enterWaterSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家进入液体时，播放的音效。默认为'audio/dive.mp3'

leaveWaterSound
•leaveWaterSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家离开液体时，播放的音效。默认为'audio/splash.mp3'

swimSound
•swimSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家正在游泳时，播放的音效。默认为'audio/swim.mp3'
注：游泳的音效在前进时才会循环播放。如果在水中静止不动，不会播放音效。

spawnSound
•spawnSound:[GameSoundEffect](https://docs.box3.codemao.cn/box3soundeffect.html)‹›= new GameSoundEffect()
当玩家重生时，播放的音效。默认为'audio/spawn.mp3'。通过player.onRespawn()触发

stepSound
•stepSound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
当玩家行走时，每迈出一步，播放的音效。默认为'audio/step.mp3'

startFlySound
•startFlySound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
玩家开始飞行时的音效。

stopFlySound
•stopFlySound:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
玩家结束飞行时播放的音效。

播放音效

sound
•sound:function
为指定的玩家播放声音，此声音仅该玩家能听见，其他玩家无法听到。
参数:
spec:{sample, gain, pitch} | string
●sample:string 必填，声音文件路径。可在文件管理器中上传自定义声音。如'audio/chat.mp3'
●gain?:number 可选，音量增益。正常为1，数值越大，声音越响。
●pitch?:number 可选，音高增益。正常为1，大于1，声音播放越快，小于1，声音播放越慢。
示例代码1

示例代码2

music
•music:[GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2)‹›= new GameSoundEffect()
为指定的玩家播放背景音乐（循环播放），此声音仅该玩家能听见，其他玩家无法听到。 背景音乐的音量会根据用户在[设置-声音]更改。

画面滤镜

colorLUT
•colorLUT:string= ""
用于渲染玩家所见游戏世界的色调
示例代码

动画

player.animate
可用这个函数来设定玩家的动画，变化颜色

社交

querySocial
(socialType: [SocialType](https://box3.yuque.com/staff-khn556/wupvz3/bxykxeicwinbyle1)) => Promise<number[]>
· 查询当前玩家的社交关系，支持查询：
· 关注
· 粉丝
· 好友
· 返回玩家 ID 列表

openUserProfileDialog
(userId: number) => void
 对当前玩家，调起指定ID玩家的个人主页。

商城

openMarketplace
●openMarketplace：function
打开游戏商店对话框，根据玩家传入的“商品ID”显示相应的产品。

函数声明：
▸ (productIds: number[]): void
参数：

| 名称       | 类型     | 说明       |
| ---------- | -------- | ---------- |
| productIds | number[] | 商品ID数组 |

示例代码

```javascript
world.onPlayerJoin(({ entity }) => {

  // product ID1: 160000000000001  ID2: 160000000000002

  entity.player.openMarketplace([160000000000001, 160000000000002])

});
```

投喂记录

getMiaoShells
●getMiaoShells：function
获取此用户在当前地图下累计打赏的喵贝壳

函数声明：
▸ (): Promise `<number>`
示例代码

```javascript
world.onPlayerJoin(async ({ entity }) => {

  // 获取用户在当前地图下累计打赏的喵贝壳

  const count = await entity.player.getMiaoShells()

  entity.player.directMessage(`我累计打赏的喵贝壳：${count}`)

})
```

## GamePurchaseSuccessEvent 购买成功事件

类 - GamePurchaseSuccessEvent
当玩家成功购买物品时触发的事件

tick
• tick: number
购买成功事件发生的时间

userId
• userId: string
触发购买事件的玩家userId

productId
• productId: number
购买商品的ID

orderId
• orderId: number
购买成功的订单号

## GameQuaternion 四元数

类 - GameQuaternion

构造函数
+new GameQuaternion(w: number,x: number,y: number,z: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型   |
| ---- | ------ |
| w    | number |
| x    | number |
| y    | number |
| z    | number |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

属性

| 名称 | 类型   |  |
| ---- | ------ | - |
| w    | number |  |
| x    | number |  |
| y    | number |  |
| z    | number |  |

方法

add
▸add(v:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                               |  |
| ---- | ---------------------------------------------------------------------------------- | - |
| v    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |  |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

angle
▸angle(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):number
参数:

| 名称 | 类型                                                                               |  |
| ---- | ---------------------------------------------------------------------------------- | - |
| q    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |  |

返回值:number

clone
▸clone():[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

copy
▸copy(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                               |  |
| ---- | ---------------------------------------------------------------------------------- | - |
| q`   | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |  |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

div
▸div(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)‹›
参数:

| 名称 | 类型                                                                               |  |
| ---- | ---------------------------------------------------------------------------------- | - |
| q    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |  |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)‹›

dot
▸dot(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):number
参数:

| 名称 | 类型                                                                               |  |
| ---- | ---------------------------------------------------------------------------------- | - |
| q    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |  |

返回值:number

equals
▸equals(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2),tolerance: number):boolean
参数:

| 名称      | 类型                                                                               | Default |  |
| --------- | ---------------------------------------------------------------------------------- | ------- | - |
| q         | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) | -       |  |
| tolerance | number                                                                             | 0.0001  |  |

返回值:boolean

getAxisAngle
▸getAxisAngle(q: any):object
参数:

| 名称 | 类型 |
| ---- | ---- |
| q    | any  |

返回值:object
●angle:number
●axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)

inv
▸inv():[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

mag
▸mag():number
返回值:number

mul
▸mul(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                               |
| ---- | ---------------------------------------------------------------------------------- |
| q    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

normalize
▸normalize():[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

rotateX
▸rotateX(_rad: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 |
| ---- |
| _rad |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

rotateY
▸rotateY(_rad: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型   |
| ---- | ------ |
| _rad | number |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

rotateZ
▸rotateZ(_rad: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型   |
| ---- | ------ |
| _rad | number |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

set
▸set(w: number,x: number,y: number,z: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型   |
| ---- | ------ |
| w    | number |
| x    | number |
| y    | number |
| z    | number |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

slerp
▸slerp(q:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2),n: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                               |
| ---- | ---------------------------------------------------------------------------------- |
| q    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |
| n    | number                                                                             |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

sqrMag
▸sqrMag():number
返回值:number

sub
▸sub(v:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                               |
| ---- | ---------------------------------------------------------------------------------- |
| v    | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2) |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

toString
▸toString():string
返回值:string

StaticfromAxisAngle
▸fromAxisAngle(axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc),rad: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                            |
| ---- | ------------------------------------------------------------------------------- |
| axis | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) |
| rad  | number                                                                          |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

StaticfromEuler
▸fromEuler(x: number,y: number,z: number):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型   |
| ---- | ------ |
| x    | number |
| y    | number |
| z    | number |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

StaticrotationBetween
▸rotationBetween(a:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc),b:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)):[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)
参数:

| 名称 | 类型                                                                            |
| ---- | ------------------------------------------------------------------------------- |
| a    | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) |
| b    | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) |

返回值:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)

## GameRaycastResult 射线检测结果

类 - GameRaycastResult
射线检测(raycast)的结果，包含射线和所击中目标的信息。

direction
•direction:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
射线的方向

distance
•distance:number
射线穿越的距离

hit
•hit:boolean
如果为真，则射线击中目标

hitEntity
•hitEntity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)| null
射线所击中的实体

hitPosition
•hitPosition:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
射线击中的位置

hitVoxel
•hitVoxel:number
射线所击中的方块id (如未击中方块，则为0)

normal
•normal:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
射线所击中平面的法向量

origin
•origin:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
射线的起点

voxelIndex
•voxelIndex:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
如果射线击中的是方块，则返回所击中方块的网格坐标。

## GameRespawnEvent 实体复活事件

类 - GameRespawnEvent
当实体复活时触发的事件

tick
• tick: number
事件发生的时间

entity
• entity: [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
复活的实体

## GameRGBColor 色彩

类 - GameRGBColor

GameRGBColor
+new GameRGBColor(r: number,g: number,b: number):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型   |
| ---- | ------ |
| r    | number |
| g    | number |
| b    | number |

示例代码

注意，此处输入的颜色值范围在(0-1) 之间。
如果需要使用 RGB 255，可以将颜色值除于255，即可得到0-1的数值。

方法

add
▸add(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| rgb  | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

clone
▸clone():[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

copy
▸ copy(c: [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)): [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| c    | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

div
▸div(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| rgb  | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

equals
▸equals(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg),tolerance: number):boolean
参数:

| 名称      | 类型                                                                             | Default |
| --------- | -------------------------------------------------------------------------------- | ------- |
| rgb       | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) | -       |
| tolerance | number                                                                           | 0.0001  |

返回值:boolean

lerp
▸lerp(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg),n: number):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| rgb  | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |
| n    | number                                                                           |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

mul
▸mul(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| rgb  | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

set
▸set(r: number,g: number,b: number,a: number):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型   |
| ---- | ------ |
| r    | number |
| g    | number |
| b    | number |
| a    | number |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

sub
▸sub(rgb:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)):[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
参数:

| 名称 | 类型                                                                             |
| ---- | -------------------------------------------------------------------------------- |
| rgb  | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg) |

返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

toRGBA
▸toRGBA():[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

toString
▸toString():string
返回值:string

Staticrandom
▸random():[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)
返回值:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)

## GameRGBAColor 透明色彩

类 - GameRGBAColor

GameRGBAColor
new GameRGBAColor(r: number,g: number,b: number,a: number):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型         |
| ---- | ------------ |
| r    | number (0-1) |
| g    | number (0-1) |
| b    | number (0-1) |
| a    | number (0-1) |

示例代码

注意，此处输入的颜色值范围在(0-1) 之间。
如果需要使用 RGB 255，可以将颜色值除于255，即可得到0-1的数值。

方法

add
▸add(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| rgba | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

clone
▸clone():[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

copy
▸copy(c:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| c    | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

div
▸div(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| rgba | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

equals
▸equals(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376),tolerance: number):boolean
参数:

| 名称      | 类型                                                                              | Default |
| --------- | --------------------------------------------------------------------------------- | ------- |
| rgba      | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) | -       |
| tolerance | number                                                                            | 0.0001  |

返回值:boolean

lerp
▸lerp(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376),n: number):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| rgba | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |
| n    | number                                                                            |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

mul
▸mul(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| rgba | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

set
▸set(r: number,g: number,b: number,a: number):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型   |
| ---- | ------ |
| r    | number |
| g    | number |
| b    | number |
| a    | number |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

sub
▸sub(rgba:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)):[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
参数:

| 名称 | 类型                                                                              |
| ---- | --------------------------------------------------------------------------------- |
| rgba | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) |

返回值:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)

toString
▸toString():string
返回值:string

## GameStorage 数据存储模块

类 - GameStorage
数据存储模块，管理游戏中的数据。

storage  对象是整个 Data Storage API的入口

getDataStorage
• getDataStorage : function
连接指定数据存储空间，如果不存在则创建一个新的空间。

函数声明
▸ (key: string): [GameDataStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)

参数:

| 名称 | 类型   |                                    |
| ---- | ------ | ---------------------------------- |
| key  | string | 指定空间的名称，长度不超过50个字符 |

返回值:[GameDataStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)

示例代码

getGroupStorage
• getGroupStorage : function
连接地图组内指定数据存储空间，如果不存在则创建一个新的空间。此方法拿到的[GameDataStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)为主图和副图共同维护的数据存储空间。

函数声明
▸ (key: string): [GameDataStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)

参数:

| 名称 | 类型   |                                    |
| ---- | ------ | ---------------------------------- |
| key  | string | 指定空间的名称，长度不超过50个字符 |

返回值:[GameDataStorage](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yifnc28uw0e9d8hl)

示例代码

主图获取玩家数据

```javascript
// 在拓展地图中，如果希望主图和副图共用玩家数据，则都用getGroupStorage获取

const userStorage = storage.getGroupStorage('users')
```

副图获取玩家数据

```javascript
const userStorage = storage.getGroupStorage('users')
```

## GameTickEvent 时钟事件

类 - GameTickEvent
每一刻(tick)触发一次的事件，由[GameWorld.onTick](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#mIgHE)触发。
示例代码

```javascript
world.onTick((tickEvent)
console.log(tickEvent.elapsedTimeMS);

    console.log(tickEvent.prevTick);

    console.log(tickEvent.skip);

    console.log(tickEvent.tick);

})
```

elapsedTimeMS
•elapsedTimeMS:number
Wall clock time between ticks 两个时刻之间的时间间隔

prevTick
•prevTick:number
Last tick which was handled 上一个已处理的时刻

skip
•skip:boolean
是否因为代码延迟而跳过了某些时刻

tick
•tick:number
事件触发时间

## GameTriggerEvent 区域触发事件

类 - GameTriggerEvent
当实体/玩家触发区域的事件。
由 [GameZone.onEnter](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8#rwvcl), [GameZone.onLeave](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8#kUa9I), [GameZone.nextEnter](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8#AWgrJ), [GameZone.nextLeave](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8#pIt6d) 触发

参数
●entity
●tick

参数

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
触发事件的实体

tick
•tick:number
触发事件的时间

## GameVector3 三维向量

类 - GameVector3

构造函数
new GameVector3(x: number, y: number, z: number): GameVector3
参数:

| 名称 | 类型   |
| ---- | ------ |
| x    | number |
| y    | number |
| z    | number |

返回值:GameVector3

属性

| 名称 | 类型   |
| ---- | ------ |
| x    | number |
| y    | number |
| z    | number |

方法

add
▸ add(v: GameVector3): GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

angle
▸angle(v:GameVector3):number
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:number

clone
▸clone():GameVector3
返回值:GameVector3

copy
▸copy(v:GameVector3):void
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:void

cross
▸cross(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

distance
▸distance(v:GameVector3):number
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:number

div
▸div(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

dot
▸dot(v:GameVector3):number
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:number

equals
▸equals(v:GameVector3,tolerance: number):boolean
参数:

| 名称      | 类型        | Default |
| --------- | ----------- | ------- |
| v         | GameVector3 | -       |
| tolerance | number      | 0.0001  |

返回值:boolean

exactEquals
▸exactEquals(v:GameVector3):boolean
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:boolean

lerp
▸lerp(v:GameVector3,n: number):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |
| n    | number      |

返回值:GameVector3

mag
▸mag():number
返回值:number

max
▸max(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

min
▸min(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

mul
▸mul(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v`   | GameVector3 |

返回值:GameVector3

normalize
▸normalize():GameVector3
返回值:GameVector3

scale
▸scale(n: number):GameVector3
参数:

| 名称 | 类型   |
| ---- | ------ |
| n    | number |

返回值:GameVector3

set
▸set(x: number,y: number,z: number):void
参数:

| 名称 | 类型   |
| ---- | ------ |
| x    | number |
| y    | number |
| z    | number |

返回值:void

sqrMag
▸sqrMag():number
返回值:number

sub
▸sub(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

toString
▸toString():string
返回值:string

towards
▸towards(v:GameVector3):GameVector3
参数:

| 名称 | 类型        |
| ---- | ----------- |
| v    | GameVector3 |

返回值:GameVector3

## GameVoxelContact 方块碰撞数据

VoxelContact方块碰撞参数
被实体触碰的方块属性

x
•x:number
被触碰方块的x坐标

y
•y:number
被触碰方块的y坐标

z
•z:number
被触碰方块的z坐标

voxel
•voxel:number
被触碰的方块id

force
•force:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
触碰的力

axis
•axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
触碰的分离轴，也就是触碰后物体弹飞的方向

## GameVoxelContactEvent 方块碰撞事件

当实体触碰方块时触发的事件。
由 [GameWorld.onVoxelContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#JZHtR), [GameWorld.onVoxelSeparate](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#qtJQI), [GameEntity.onVoxelContact](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#Lr61W), [GameEntity.onVoxelSeparate](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#zfEFq) 触发

axis
•axis:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
触碰的分离轴，也就是触碰后物体弹飞的方向

entity
•entity:[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
触碰到方块的实体

force
•force:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
碰撞力

tick
•tick:number
实体触碰方块的时间

voxel
•voxel:number
被触碰的方块id

x
•x:number
被触碰方块的x坐标

y
•y:number
被触碰方块的y坐标

z
•z:number
被触碰方块的z坐标

## GameVoxels 方块模块

类 - GameVoxels
GameVoxels是控制Box3所有方块的接口，你可以使用 voxels 对象控制地形变化，利用循环语法批量生成/销毁方块，获取某个方块的类型、名称、旋转角度等。

Basic 基础

voxels.shape
属性     属性值类型：GameVector3     默认值：{x: 128, y: 128, z: 128}
世界地形最大尺寸。
目前，Box3地形最大可支持128x128x128，未来将开放更大的地形，敬请期待。

Voxel Name 方块名称

voxels.id()
方法
将方块名称转换为方块id
参数 name

| 名称 | 类型   | 说明     |
| ---- | ------ | -------- |
| name | string | 方块名称 |

返回值 id

| 名称 | 类型   | 说明    |
| ---- | ------ | ------- |
| id   | number | 方块 id |

voxels.name()
方法
将方块id转换为方块名称
参数 id

| 名称 | 类型   | 说明   |
| ---- | ------ | ------ |
| id   | number | 方块id |

返回值 name

| 名称 | 类型   | 说明     |
| ---- | ------ | -------- |
| name | string | 方块名称 |

setVoxel 放置方块
如果你想要地图在非运行状态，通过脚本在场景中快速建造，可以尝试以下操作：
1开启编辑器右上角的调试模式(小虫子图标)
2使用窗口底部的控制台，输入对应的代码。
即使游戏没有运行，也能使部分代码直接生效。
💡提示
使用控制台执行脚本前，请务必要小心，提前做好项目备份工作。一旦代码生效后，有可能造成无法恢复的情况。
要操作方块时，建议先使用空白地图对代码进行充分测试，效果满意后，再操作正式的地图。

voxels.setVoxel()
方法
在指定的坐标位置放置一个方块。
参数 x, y, z, voxel, rotation

| 名称     | 类型   | 说明                  |
| -------- | ------ | --------------------- |
| x        | number | 必填，放置位置的x坐标 |
| y        | number | 必填，放置位置的y坐标 |
| z        | number | 必填，放置位置的z坐标 |
| voxel    | number | string                |
| rotation | number | string                |

返回值 id

| 名称 | 类型   | 说明       |
| ---- | ------ | ---------- |
| id   | number | 新的方块id |

💡提示
若方块名称为'air' 或者方块id为0，则会打破
 简单示例

 将脚下的方块全部变成雪地

 删除地面至上空的所有方块

 方块自动往上增长

利用方块显示字母

 利用方块显示文章

 创建一个棋盘

voxels.setVoxelId()
方法
使用方块ID，直接在指定的坐标位置放置方块。执行效率比[voxels.setVoxel()](https://box3.yuque.com/staff-khn556/wupvz3/gkz7g1wazf5izpfy#kuAQe)更快。
参数 x, y, z, voxel

| 名称  | 类型   | 说明                    |
| ----- | ------ | ----------------------- |
| x     | number | 必填，放置的方块 x 坐标 |
| y     | number | 必填，放置的方块 y 坐标 |
| z     | number | 必填，放置的方块 z 坐标 |
| voxel | number | 必填，放置的方块 id     |

返回值 id

| 名称 | 类型   | 说明                 |
| ---- | ------ | -------------------- |
| id   | number | 返回指定位置的方块id |

getVoxel 获取方块

voxels.getVoxel()
方法
获取某个坐标位置的方块id
参数 x, y, z

| 名称 | 类型   | 说明                    |
| ---- | ------ | ----------------------- |
| x    | number | 必填，获取的方块 x 坐标 |
| y    | number | 必填，获取的方块 y 坐标 |
| z    | number | 必填，获取的方块 z 坐标 |

返回值 id

| 名称 | 类型   | 说明                 |
| ---- | ------ | -------------------- |
| id   | number | 返回指定位置的方块id |

voxels.getVoxelId()
方法
直接获取指定位置的方块ID。执行效率比[voxels.getVoxel()](https://box3.yuque.com/staff-khn556/wupvz3/gkz7g1wazf5izpfy#JvOpR)更快。
参数 x, y, z

| 名称 | 类型   | 说明                    |
| ---- | ------ | ----------------------- |
| x    | number | 必填，获取的方块 x 坐标 |
| y    | number | 必填，获取的方块 y 坐标 |
| z    | number | 必填，获取的方块 z 坐标 |

返回值 id

| 名称 | 类型   | 说明                 |
| ---- | ------ | -------------------- |
| id   | number | 返回指定位置的方块id |

voxels.getVoxelRotation()
方法
获取某个坐标位置的方块旋转码
参数 x, y, z

| 名称 | 类型   | 说明                    |
| ---- | ------ | ----------------------- |
| x    | number | 必填，获取的方块 x 坐标 |
| y    | number | 必填，获取的方块 y 坐标 |
| z    | number | 必填，获取的方块 z 坐标 |

返回值 id

| 名称 | 类型   | 说明                 |
| ---- | ------ | -------------------- |
| id   | number | 返回指定位置的方块id |

Voxels Type 方块类型

voxels.VoxelTypes
属性     属性值类型：Array     默认值：String[]
返回包含所有方块名称的数组。

Build 快速建造
此处提供一些快速建造特定几何造型的代码片段，可供参考。
 实心矩形

 空心矩形

 实心球体

 圆柱体

 生成楼梯(+x)

 生成楼梯(-x)

💡提示
方块id和名称对照表

| 方块id | 名称                   |
| ------ | ---------------------- |
| 0      | air                    |
| 3      | add                    |
| 5      | subtract               |
| 7      | multiply               |
| 9      | divide                 |
| 11     | equal                  |
| 13     | exclamation_mark       |
| 15     | question_mark          |
| 17     | zero                   |
| 19     | one                    |
| 21     | two                    |
| 23     | three                  |
| 25     | four                   |
| 27     | five                   |
| 29     | six                    |
| 31     | seven                  |
| 33     | eight                  |
| 35     | nine                   |
| 37     | A                      |
| 39     | B                      |
| 41     | C                      |
| 43     | D                      |
| 45     | E                      |
| 47     | F                      |
| 49     | G                      |
| 51     | H                      |
| 53     | I                      |
| 55     | J                      |
| 57     | K                      |
| 59     | L                      |
| 61     | M                      |
| 63     | N                      |
| 65     | O                      |
| 67     | P                      |
| 69     | Q                      |
| 71     | R                      |
| 73     | S                      |
| 75     | T                      |
| 77     | U                      |
| 79     | V                      |
| 81     | W                      |
| 83     | X                      |
| 85     | Y                      |
| 87     | Z                      |
| 89     | cadet_blue             |
| 91     | sky_blue               |
| 93     | powder_blue            |
| 95     | dark_gray              |
| 97     | light_gray             |
| 99     | olive_green            |
| 101    | yellow_green           |
| 103    | pale_green             |
| 105    | red                    |
| 107    | dark_red               |
| 109    | brick_red              |
| 111    | medium_gray            |
| 113    | dark_slate_blue        |
| 115    | pink                   |
| 117    | sakura_pink            |
| 119    | orange                 |
| 121    | lemon                  |
| 123    | stained_glass          |
| 125    | dirt                   |
| 127    | grass                  |
| 129    | stone                  |
| 131    | green_leaf             |
| 133    | acacia                 |
| 135    | sand                   |
| 137    | plank_01               |
| 139    | plank_02               |
| 141    | plank_03               |
| 143    | plank_04               |
| 145    | ice_brick              |
| 147    | light_grey_stone_brick |
| 149    | grey_stone_brick       |
| 151    | gold_trim_brick        |
| 153    | red_brick              |
| 155    | quartz_brick           |
| 157    | lantern_01             |
| 159    | lantern_02             |
| 160    | window                 |
| 162    | cross_window           |
| 164    | geometric_window_01    |
| 166    | geometric_window_02    |
| 169    | snow                   |
| 170    | glass                  |
| 172    | color_glass            |
| 175    | black                  |
| 177    | white                  |
| 179    | wooden_box             |
| 181    | board_01               |
| 183    | board_02               |
| 185    | stripe_01              |
| 187    | stripe_02              |
| 189    | stripe_03              |
| 191    | stripe_04              |
| 193    | stripe_05              |
| 195    | carpet_01              |
| 197    | carpet_02              |
| 199    | carpet_03              |
| 201    | carpet_04              |
| 203    | carpet_05              |
| 205    | carpet_06              |
| 207    | carpet_07              |
| 209    | palace_eaves_01        |
| 211    | palace_eaves_02        |
| 213    | palace_eaves_03        |
| 215    | palace_eaves_04        |
| 217    | palace_eaves_05        |
| 219    | palace_eaves_06        |
| 221    | palace_eaves_07        |
| 223    | palace_eaves_08        |
| 225    | roof_red               |
| 227    | roof_purple            |
| 229    | roof_green             |
| 231    | roof_blue_04           |
| 233    | roof_yellow            |
| 235    | carpet_08              |
| 237    | carpet_09              |
| 239    | carpet_10              |
| 241    | carpet_11              |
| 243    | carpet_12              |
| 245    | carpet_13              |
| 247    | stainless_steel        |
| 249    | ice_wall               |
| 251    | leaf_01                |
| 253    | leaf_02                |
| 255    | palace_roof            |
| 257    | wood                   |
| 259    | red_brick_floor        |
| 261    | red_brick_wall         |
| 263    | palace_floor           |
| 264    | palace_carving         |
| 267    | stone_pillar_03        |
| 269    | stone_pillar_04        |
| 271    | stone_pillar_05        |
| 273    | stone_pillar_06        |
| 275    | stone_wall             |
| 276    | blue_glass             |
| 278    | green_glass            |
| 281    | red_light              |
| 283    | orange_light           |
| 285    | yellow_light           |
| 287    | green_light            |
| 289    | indigo_light           |
| 291    | blue_light             |
| 293    | purple                 |
| 295    | pink_light             |
| 297    | mint_green_light       |
| 299    | white_light            |
| 301    | warm_yellow_light      |
| 302    | black_glass            |
| 304    | red_glass              |
| 307    | palace_lamp            |
| 309    | board_03               |
| 311    | board_04               |
| 313    | board_05               |
| 315    | board_06               |
| 317    | dark_grass             |
| 319    | greenbelt_L            |
| 321    | greenbelt_L1           |
| 323    | stone_brick_01         |
| 325    | stone_brick_02         |
| 327    | dark_stone             |
| 329    | dark_brick_00          |
| 331    | dark_brick_01          |
| 333    | dark_brick_02          |
| 335    | stone_wall_01          |
| 337    | pink_cake              |
| 339    | macaroon               |
| 341    | biscuit                |
| 343    | snowland               |
| 345    | polar_region           |
| 347    | polar_ice              |
| 349    | blue_surface_01        |
| 351    | blue_surface_02        |
| 353    | purple_surface_01      |
| 355    | purple_surface_02      |
| 357    | dark_surface           |
| 359    | rock                   |
| 361    | palace_cloud           |
| 363    | blue                   |
| 364    | water                  |
| 367    | turquoise              |
| 369    | dark_orchid            |
| 371    | medium_orchid          |
| 373    | medium_purple          |
| 375    | medium_violet_red      |
| 377    | maroon                 |
| 379    | coffee_gray            |
| 381    | peru                   |
| 383    | dark_salmon            |
| 385    | navajo_white           |
| 387    | orange_red             |
| 389    | medium_yellow          |
| 391    | medium_green           |
| 393    | sienna                 |
| 395    | mint_green             |
| 397    | medium_spring_green    |
| 398    | ice                    |
| 401    | crane_roof_01          |
| 403    | crane_roof_02          |
| 405    | crane_lantern          |
| 407    | roof_grey              |
| 408    | palace_window          |
| 411    | woodstone_12           |
| 412    | strawberry_juice       |
| 414    | lime_juice             |
| 416    | blueberry_juice        |
| 418    | lemon_juice            |
| 420    | grape_juice            |
| 422    | orange_juice           |
| 424    | milk                   |
| 426    | soy_sauce              |
| 428    | coffee                 |
| 430    | peach_juice            |
| 433    | board0                 |
| 435    | board1                 |
| 437    | board2                 |
| 439    | board3                 |
| 441    | board4                 |
| 443    | board5                 |
| 445    | board6                 |
| 447    | board7                 |
| 449    | board8                 |
| 451    | board9                 |
| 453    | board10                |
| 455    | board11                |
| 457    | board12                |
| 459    | board13                |
| 461    | board14                |
| 463    | board15                |
| 465    | lava01                 |
| 467    | lava02                 |
| 469    | windygrass             |
| 471    | conveyor               |
| 473    | ledfloor01             |
| 475    | ledfloor02             |
| 477    | yellow_grass           |
| 479    | express_box            |
| 481    | television             |
| 483    | bookshelf              |
| 485    | ampersand              |
| 487    | asterisk               |
| 489    | at                     |
| 491    | backslash              |
| 493    | bracket_close          |
| 495    | bracket_open           |
| 497    | caret                  |
| 499    | colon                  |
| 501    | comma                  |
| 503    | dollar                 |
| 505    | greater_than           |
| 507    | less_than              |
| 509    | paren_open             |
| 511    | paren_close            |
| 513    | percent                |
| 515    | period                 |
| 517    | pound                  |
| 519    | quotation_mark         |
| 521    | semicolon              |
| 523    | slash                  |
| 525    | tilde                  |
| 527    | winter_leaf            |
| 529    | leaf_03                |
| 531    | leaf_04                |
| 533    | leaf_05                |
| 535    | honeycomb_01           |
| 537    | honeycomb_02           |
| 539    | white_grass            |
| 541    | palm                   |

## GameWearable 穿戴配件

类 - GameWearable
用于在玩家身体部位可穿戴配件物体的参数与函数

参数
●bodyPart
●color
●emissive
●mesh
●metalness
●offset
●orientation
●player
●scale
●shininess

函数
●remove

控制穿戴配件的参数

bodyPart
•bodyPart:[GameBodyPart](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fqfcrsh8mid6ook3)= GameBodyPart.HEAD
穿戴配件在玩家上的部位

color
•color:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(1, 1, 1)
穿戴配件的颜色

emissive
•emissive:number= 0
穿戴配件的发光度

mesh
•mesh:string= ""
穿戴配件的形状数据
e.g.mesh = 'mesh/my-mesh.vb'
注意:'mesh/my-mesh.vb'必须在文件列表中（Tips: 先将模型加到地图上，再删掉即可。）

metalness
•metalness:number= 0
穿戴配件的金属感

offset
•offset:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)‹›= new GameVector3(0, 0, 0)
穿戴配件的位移

orientation
•orientation:[GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)‹›= new GameQuaternion(0, 1, 0, 0)
穿戴配件的旋转角度

player
•player:[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)| null= null
穿戴配件的玩家

scale
•scale:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)‹›= new GameVector3(1, 1, 1)
穿戴配件的缩放比例

shininess
•shininess:number= 0
穿戴配件的反光度

函数

remove
▸remove():void
Returns:void
示例代码

```javascript
// 在玩家离开液体时把在玩家身上所有的穿戴配件删除

world.onFluidLeave(({ entity }) => {

  if (entity.isPlayer) {

    const allWearables = entity.player.wearables();

    allWearables.forEach((item) => {

    item.remove();

    });

  }

});
```

## GameWorld 世界模块

类 - GameWorld
GameWorld这个类在当前地图是有全局唯一的实例 world，你可以使用world对象控制环境天气、物理重力、画面滤镜等全局场景属性，还可以在世界中创建、搜索实体，或监听世界中实体和玩家的碰撞、伤害、互动等事件。

Basics 基础

world.projectName
 属性      属性值类型：string     默认值：无
本张地图名称，对应项目设置中的名称。
该属性是只读的，如需修改地图名称，请在编辑器菜单底部 [项目-编辑资料-地图名称] 进行修改。

world.onTick()
事件
这是世界的计时事件，每64毫秒触发一次，Tick计数加1。
监听此事件可以让世界以64毫秒为间隔循环执行代码。
在理想情况下，每Tick为64毫秒。若网络发生延迟，可能会有变化。
●onTick: [GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameTickEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl)](%5BGameTickEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl))
●nextTick: [GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameTickEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl)](%5BGameTickEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/iewkxcpddoqrt1vl))
返回值 GameTickEvent:{ tick, prevTick, elapsedTimeMS, skip }

| 名称          | 类型    | 说明                          |
| ------------- | ------- | ----------------------------- |
| tick          | number  | 事件发生时间                  |
| prevTick      | number  | 上一个已处理的时刻            |
| elapsedTimeMS | number  | 两个时刻之间的时间间隔(毫秒)  |
| skip          | boolean | 是否因为延迟而跳过了某些 Tick |

 示例代码1

 示例代码2

world.currentTick
属性     属性值类型：number     默认值：0
世界当前的Tick计数。

Chat 聊天频道

world.say()
方法
向所有玩家广播一条消息。
参数 message

| 名称    | 类型   | 说明         |
| ------- | ------ | ------------ |
| message | string | 要广播的消息 |

 简单示例

 循环喊话

 高级计时器

world.onChat()
事件
当玩家在聊天窗口说话时触发

| 名称    | 类型                                                                           | 说明                 |
| ------- | ------------------------------------------------------------------------------ | -------------------- |
| entity  | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 发起聊天的实体       |
| message | string                                                                         | 聊天事件中说话的内容 |
| tick    | number                                                                         | 聊天事件发生时间     |

Player 玩家：加入/离开

world.onPlayerJoin()事件：当玩家加入地图时触发

返回值 GameEntityEvent:{ entity, tick }

| 名称   | 类型                                                                           | 说明         |
| ------ | ------------------------------------------------------------------------------ | ------------ |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 创建的实体   |
| tick   | number                                                                         | 事件发生时间 |

 简单示例

 所有玩家飞行

 特定玩家进入地图提醒

world.onPlayerLeave()事件：
当玩家离开地图时触发
返回值 GameEntityEvent:{ entity, tick }

| 名称   | 类型                                                                           | 说明           |
| ------ | ------------------------------------------------------------------------------ | -------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 离开地图的实体 |
| tick   | number                                                                         | 事件发生时间   |

Input 点击/互动

world.onInteract()事件：
若实体开启了互动功能[enableInteract = true](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)，则玩家与实体进行互动时触发。
当玩家走进实体的互动范围，实体身上就会出现按键提示，玩家按下互动按钮(默认为键盘E按键)与该实体进行互动。
触发onInteract事件同时还会触发实体默认的互动音效
返回值 GameInteractEvent{ entity, targetEntity, tick }

| 名称         | 类型                                                                           | 说明               |
| ------------ | ------------------------------------------------------------------------------ | ------------------ |
| entity       | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 发起互动的实体     |
| targetEntity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 收到互动请求的实体 |
| tick         | number                                                                         | 事件发生时间       |

💡提示
想要和实体进行互动，需要先在编辑器中放置一个模型，并给他取一个名字。
这里的示范，将名字改为了'NPC'。

💡提示
通过通过监听onInteract事件，可以自定义互动时发生的行为。
比如，让[实体说话](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#hurzg)，或让玩家[显示一个对话框](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#soRHv)

world.onClick()事件：
当玩家用鼠标点击实体时触发
返回值 GameInputEvent:{ entity, clicker, button, distance, clickerPosition, raycast, tick}

| 名称            | 类型                                                                                                                                                                                  | 说明                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| entity          | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)                                                                                                        | 被点击的实体                               |
| clicker         | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)& {isPlayer:true,player:[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)} | 发起点击事件的玩家                         |
| button          | [GameButtonType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)                                                                                                    | 点击的按钮，ACTION0 = 左键，ACTION1 = 右键 |
| distance        | number                                                                                                                                                                                | 玩家到被点击实体的距离                     |
| clickerPosition | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)                                                                                                       | 点击鼠标的瞬间玩家所在位置                 |
| raycast         | [GameRaycastResult](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)                                                                                                 | 按下按钮瞬间，从玩家视角投射的射线检测结果 |
| tick            | number                                                                                                                                                                                | 事件发生时间                               |

world.onPress()事件：
当玩家按下按钮时触发
返回值 GameInputEvent:{ button, entity, position, pressed, raycast, tick }

| 名称     | 类型                                                                                                                                                                                   | 说明                                        |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| button   | [GameButtonType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)                                                                                                     | 玩家输入的按钮                              |
| entity   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)& {isPlayer:true, player:[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)} | 按下按钮的玩家                              |
| position | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)                                                                                                        | 按下按钮瞬间，玩家的位置                    |
| pressed  | boolean                                                                                                                                                                                | 是否按下了按钮。若为 true，则为按下了按钮。 |
| raycast  | [GameRaycastResult](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)                                                                                                  | 按下按钮瞬间，从玩家视角投射的射线检测结果  |
| tick     | number                                                                                                                                                                                 | 事件发生时间                                |

world.onRelease()事件：
当玩家松开按钮时触发
返回值 GameInputEvent:{ button, entity, position, pressed, raycast, tick }

| 名称     | 类型                                                                                                                                                                                   | 说明                                           |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| button   | [GameButtonType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/xlg3k99cmtgyc37d)                                                                                                     | 玩家输入的按钮                                 |
| entity   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)& {isPlayer:true, player:[GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)} | 按下按钮的玩家                                 |
| position | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)                                                                                                        | 按下按钮瞬间，玩家的位置                       |
| pressed  | boolean                                                                                                                                                                                | 是否按下了按钮。若为 false，则为松开按钮。     |
| raycast  | [GameRaycastResult](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/eoawgqo7sl2cuz6a)                                                                                                  | 按下按钮瞬间，从玩家视角向前投射的射线检测结果 |
| tick     | number                                                                                                                                                                                 | 事件发生时间                                   |

💡提示
提示：GameWorld 和 GamePlayer 都有触发点击/按下按钮的事件。他们的区别就是：
●GameWorld会监听世界所有实体的事件
●GamePlayer 只监听玩家本身的事件
通常 GamePlayer.onPress() 会放在 GameWorld.onPlayerJoin() 事件中使用。
详情请阅读 [GamePlayer](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)

Entity 实体：创建/销毁

world.createEntity()
方法
创建一个新实体[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)或复制一个现有的实体，若实体数量([entityQuota](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#V3nLM))达到上限，则返回 null。
参数 GameEntityConfig

| 名称   | 类型                                                                                                                                                                                       | 说明                 |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------- |
| config | Partial[[GameEntityConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vim7evgezkmnvhxk)](%5BGameEntityConfig%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vim7evgezkmnvhxk)) | 指定实体的一组初始值 |

返回值 GameEntity

| 名称   | 类型                                                                           | 说明                         |
| ------ | ------------------------------------------------------------------------------ | ---------------------------- |
| Entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 根据指定参数创建的一个新实体 |

💡提示
需要提前在编辑器中添加'花'的模型。
添加后可以在地图中删除 (只需确保 设置-文件 页面中已加载 花.vb 模型文件)。

world.entityQuota()
方法
返回脚本当前仍可创建的实体数量
返回值 number

| 类型   | 说明                   |
| ------ | ---------------------- |
| number | 当前仍可创建的实体数量 |

world.onEntityCreate()事件：当实体被创建时触发

返回值 GameEntityEvent:{ entity, tick }

| 名称   | 类型                                                                           | 说明         |
| ------ | ------------------------------------------------------------------------------ | ------------ |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 被创建的实体 |
| tick   | number                                                                         | 事件发生时间 |

world.onEntityDestroy()事件：当实体被销毁时触发

返回值 GameEntityEvent:{ entity, tick }

| 名称   | 类型                                                                           | 说明         |
| ------ | ------------------------------------------------------------------------------ | ------------ |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 销毁的实体   |
| tick   | number                                                                         | 事件发生时间 |

Battle & Health 战斗及生命值
若实体开启了允许伤害的属性[(enableDamage = true)](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)，可以通过[hurt()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#mECcB)方法对该实体造成生命值伤害。
伤害: 实体受到伤害，会触发[onTakeDamage()](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#MSnaO)事件。
死亡: 实体生命值[HP](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#vqUwj)降为0以下时，实体将触发死亡事件[onDie()](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#fO5zM), 倒地不起。
复活: 实体死亡后，可通过增加生命值[HP](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#vqUwj)，让实体进行复活，同时触发[onRespawn()](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#EdpQj)事件。
强制重生: 如果实体类型为玩家，还可以通过[forceRespawn()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#B4nEF)方法，使玩家强制重生，返回[出生点](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#pvk3M)。

world.onTakeDamage()
事件
当实体受到伤害时触发。
●onTakeDamage:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameDamageEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)](%5BGameDamageEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm))
●nextTakeDamage:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameDamageEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm)](%5BGameDamageEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/aivo4orkcmc9m0gm))
返回值 GameDamageEvent:{ entity, attacker, damage, damageType, tick }

| 名称       | 类型                                                                           | 说明           |
| ---------- | ------------------------------------------------------------------------------ | -------------- |
| attacker   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | null           |
| damage     | number                                                                         | 伤害值         |
| damageType | string                                                                         | 伤害类型       |
| entity     | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 受到伤害的实体 |
| tick       | number                                                                         | 事件发生时间   |

world.onDie()
事件
当实体死亡时触发。
●onDie:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameDieEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)](%5BGameDieEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y))
●nextDie:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameDieEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y)](%5BGameDieEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/fsnsdr8uvuspan6y))
返回值 GameDieEvent:{ entity, attacker, damageType, tick }

| 名称       | 类型                                                                           | 说明         |
| ---------- | ------------------------------------------------------------------------------ | ------------ |
| attacker   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | null         |
| damageType | string                                                                         | 伤害类型     |
| entity     | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 死亡的实体   |
| tick       | number                                                                         | 事件发生时间 |

 简单示例

 死亡5秒后重生

world.onRespawn()
事件
当实体复活时触发。
onRespawn:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameRespawnEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)](%5BGameRespawnEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr))
nextRespawn:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameRespawnEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr)](%5BGameRespawnEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cshui17169guugxr))
返回值 GameRespawnEvent:{ entity, tick }

| 名称   | 类型                                                                           | 说明         |
| ------ | ------------------------------------------------------------------------------ | ------------ |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 死亡的实体   |
| tick   | number                                                                         | 事件发生时间 |

提示
GameWorld 和 GameEntity 拥有相同的触发事件。 他们的区别是
●GameWorld会触发世界所有的实体事件。
●GameEntity 只触发实体本身的事件。

Zones 区域

world.addZone()
方法
创建一个区域，用于检测实体进入或离开某个区域。 也可以用来设置环境参数，如雾、雨、天、雪、风、重力等定义区域内的环境参数。
参数 GameZoneConfig

| 名称   | 类型                                                                                          | 说明                     |
| ------ | --------------------------------------------------------------------------------------------- | ------------------------ |
| config | Partial‹[GameZoneConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yiaupxo6r5es9wcw)› | 指定区域的一组初始参数值 |

返回值 GameZone

| 名称     | 类型                                                                         | 说明 |
| -------- | ---------------------------------------------------------------------------- | ---- |
| GameZone | [GameZone](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8) | 区域 |

world.removeZone()
方法
删除区域
参数 zone

| 名称 | 类型                                                                         | 说明         |
| ---- | ---------------------------------------------------------------------------- | ------------ |
| zone | [GameZone](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8) | 要删除的区域 |

world.zones()
方法
返回所有的区域列表
返回值 GameZone[]

| 名称       | 类型                                                                         | 说明       |
| ---------- | ---------------------------------------------------------------------------- | ---------- |
| GameZone[] | [GameZone](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8) | 所有的区域 |

Search 搜索
Game可以用类似jQuery选择器的语法来搜索某些实体。
●搜索全部:'*'
●搜索名称:'#id'
●搜索标签:'.tag'
●搜索同时包含多个标签:'.tag1 .tag2'
●搜索玩家:'player'

world.querySelector()
方法
搜索满足条件的第一个实体。
参数 selector

| 名称     | 类型                                                                                   | 说明                 |
| -------- | -------------------------------------------------------------------------------------- | -------------------- |
| selector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 一个选择器搜索模式。 |

返回值 GameEntity | null

| 名称   | 类型                                                                           | 说明                 |
| ------ | ------------------------------------------------------------------------------ | -------------------- |
| Entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 符合选择器的首个实体 |

 简单示例

 示例代码2

world.querySelectorAll()
方法
搜索满足条件的所有实体，返回一个列表。
参数 selector

| 名称     | 类型                                                                                   | 说明               |
| -------- | -------------------------------------------------------------------------------------- | ------------------ |
| selector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 一个选择器搜索模式 |

返回值 GameEntity[]

| 名称     | 类型                                                                           | 说明                 |
| -------- | ------------------------------------------------------------------------------ | -------------------- |
| Entity[] | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 符合选择器的全部实体 |

 简单示例

搜索所有玩家

💡提示
querySelector 和 querySelectorAll 两者区别是
querySelector 搜索满足条件的第一个实体，如果没有搜索到，则返回 null
querySelectorAll 搜索满足条件的所有实体，返回是一个数组，如果没有搜索到实体，则返回空的数组。

world.searchBox()
方法
搜索指定范围中的全部实体
参数 bounds

| 名称   | 类型                                                                            | 说明             |
| ------ | ------------------------------------------------------------------------------- | ---------------- |
| bounds | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb) | 要搜索的范围边界 |

返回值 GameEntity[]

| 名称     | 类型                                                                           | 说明             |
| -------- | ------------------------------------------------------------------------------ | ---------------- |
| Entity[] | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 范围内的全部实体 |

world.raycast()
方法
射线检测，从origin原点位置向direction方向投射一条隐形的射线，返回碰到的实体或方块。
参数 origin, direction, options

| 名称      | 类型                                                                                   | 说明               |
| --------- | -------------------------------------------------------------------------------------- | ------------------ |
| origin    | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)        | 必填，射线的起点   |
| direction | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)        | 必填，射线的方向   |
| options   | [GameRaycastOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zi57zw8to9oze8u3) | 可选，选项配置参数 |

返回值 GameRaycastResult

| 名称        | 类型                                                                            | 说明                                               |
| ----------- | ------------------------------------------------------------------------------- | -------------------------------------------------- |
| origin      | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 射线的起点                                         |
| direction   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 射线的方向                                         |
| distance    | number                                                                          | 射线穿越的距离                                     |
| hit         | boolean                                                                         | 如果为真，则射线击中了目标                         |
| hitEntity   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | null                                               |
| hitPosition | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 射线击中的位置                                     |
| hitVoxel    | number                                                                          | 射线所击中的方块 id (如未击中方块，则为 0)         |
| voxelIndex  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 如果射线击中的是方块，则返回所击中方块的网格坐标。 |
| normal      | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 射线所击中平面的法向量                             |

Physics 物理相关 📌

world.gravity
属性     属性值类型：number     默认值：-0.1
世界重力。对应编辑器菜单 [场景-物理-地心引力] 控件属性。
数值越小，行动越笨重。受重力影响最明显的属性是跳跃高度及下落速度。如果重力数值大于0，可以实现反重力。

world.airFriction
属性     属性值类型：number     默认值：0.001
空气阻力。对应编辑器菜单[场景-速度阻尼]控件属性。
数值在0-1之间。数值越大，行走加速度越小。可以用来模拟大风的环境。

world.onEntityContact()
事件
当实体与实体发生碰撞时触发。
●onEntityContact:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
●nextEntityContact:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
返回值 GameEntityContactEvent:{ entity, other, force, axis, tick }

| 名称   | 类型                                                                            | 说明                 |
| ------ | ------------------------------------------------------------------------------- | -------------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 碰撞中的第一个实体   |
| other  | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 碰撞中的第二个实体   |
| force  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞所产生的力       |
| axis   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞后物体弹飞的方向 |
| tick   | number                                                                          | 事件发生时间         |

 简单示例

 碰到指定实体加血

 碰到实体变身

💡提示
两个实体刚接触的第一下，触发onEntityContact 直到两个实体分开，触发onEntitySeparate

world.onEntitySeparate()
事件
实体与实体结束碰撞时触发。
●onEntitySeparate:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
●nextEntitySeparate:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameEntityContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng)](%5BGameEntityContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cx43ln010fi1npng))
返回值 GameEntityContactEvent:{entity, other, force, axis, tick}

| 名称   | 类型                                                                            | 说明                 |
| ------ | ------------------------------------------------------------------------------- | -------------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 碰撞中的第一个实体   |
| other  | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 碰撞中的第二个实体   |
| force  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞所产生的力       |
| axis   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞后物体弹飞的方向 |
| tick   | number                                                                          | 事件发生时间         |

world.onVoxelContact()
事件
当实体与方块发生碰撞时触发。
●onVoxelContact:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
●nextVoxelContact:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
返回值 GameVoxelContactEvent:{ entity, voxel, x, y, z, force, axis, tick }

| 名称   | 类型                                                                            | 说明                 |
| ------ | ------------------------------------------------------------------------------- | -------------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 触碰方块的实体       |
| voxel  | number                                                                          | 被触碰的方块 id      |
| x      | number                                                                          | 被触碰方块的 x 坐标  |
| y      | number                                                                          | 被触碰方块的 y 坐标  |
| z      | number                                                                          | 被触碰方块的 z 坐标  |
| force  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞所产生的力       |
| axis   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞后物体弹飞的方向 |
| tick   | number                                                                          | 事件发生时间         |

 破坏碰到的冰块

 检测脚下的方块

world.onVoxelSeparate()
事件
当实体与方块结束碰撞时触发。
●onVoxelSeparate:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
●nextVoxelSeparate:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameVoxelContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w)](%5BGameVoxelContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yq8us26l3irc2m0w))
返回值 GameVoxelContactEvent:{ entity, voxel, x, y, z, force, axis, tick }

| 名称   | 类型                                                                            | 说明                 |
| ------ | ------------------------------------------------------------------------------- | -------------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)  | 触碰方块的实体       |
| voxel  | number                                                                          | 被触碰的方块 id      |
| x      | number                                                                          | 被触碰方块的 x 坐标  |
| y      | number                                                                          | 被触碰方块的 y 坐标  |
| z      | number                                                                          | 被触碰方块的 z 坐标  |
| force  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞所产生的力       |
| axis   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 碰撞后物体弹飞的方向 |
| tick   | number                                                                          | 事件发生时间         |

world.onFluidEnter()
事件
当实体进入水里/液体时触发。
●onFluidEnter:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
●nextFluidEnter:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
返回值 GameFluidContactEvent:{ entity, voxel, tick }

| 名称   | 类型                                                                           | 说明           |
| ------ | ------------------------------------------------------------------------------ | -------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 触碰液体的实体 |
| voxel  | number                                                                         | 触碰的液体方块 |
| tick   | number                                                                         | 事件发生时间   |

world.onFluidLeave()
事件
当实体离开水里/液体时触发。
●onFluidLeave:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)[[GameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
●nextFluidLeave:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)[ameFluidContactEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10)](%5BGameFluidContactEvent%5D(https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yqghak2c6vyayb10))
返回值 GameFluidContactEvent:{ entity, voxel, tick }

| 名称   | 类型                                                                           | 说明           |
| ------ | ------------------------------------------------------------------------------ | -------------- |
| entity | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 触碰液体的实体 |
| voxel  | number                                                                         | 触碰的液体方块 |
| tick   | number                                                                         | 事件发生时间   |

world.addCollisionFilter()
方法
添加碰撞过滤器，关闭两个实体组之间的碰撞。其中两个实体组分别用[选择器](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9)aSelector、bSelector来定义，可按实体名称、标签、以及是否玩家等条件来筛选。
参数

| 名称      | 类型                                                                                   | 说明                       |
| --------- | -------------------------------------------------------------------------------------- | -------------------------- |
| aSelector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 用于定义第一组实体的选择器 |
| bSelector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 用于定义第二组实体的选择器 |

返回值 void

world.removeCollisionFilter()
方法
移除碰撞过滤器，不再关闭两个实体组aSelector、bSelector之间的碰撞。
参数

| 名称      | 类型                                                                                   | 说明                       |
| --------- | -------------------------------------------------------------------------------------- | -------------------------- |
| aSelector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 用于定义第一组实体的选择器 |
| bSelector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 用于定义第二组实体的选择器 |

返回值 void

world.clearCollisionFilters()
方法
清除全部碰撞过滤器。
返回值 void

world.collisionFilters()
方法
返回当前有效的全部碰撞过滤器。 Returns a list of all currently active collision filters
返回值 string[][]

| 类型       | 说明                     |
| ---------- | ------------------------ |
| string[][] | 当前有效的全部碰撞过滤器 |

world.testSelector()
方法
测试实体是否符合某个[选择器(Selector)](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9)的条件。 Test a selector on an entity.
参数

| 名称     | 类型                                                                                   | 说明           |
| -------- | -------------------------------------------------------------------------------------- | -------------- |
| selector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 要测试的选择器 |
| entity   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)         | 要测试的实体   |

返回值 boolean

| 类型    | 说明                                                     |
| ------- | -------------------------------------------------------- |
| boolean | true: 实体符合选择器的条件;false: 实体不符合选择器的条件 |

 简单示例

示例代码2

Sound 音乐音效

world.sound()
方法
播放一段声音，所有玩家都能听到。在[文件管理]窗口右下角[上传音频]，通过.sound()方法传入声音文件的路径。
参数 spec | string

| 名称     | 类型                                                                            | 说明                                                                     |
| -------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| sample   | string                                                                          | 必填，声音文件路径。可在文件管理器中上传自定义声音。如'audio/chat.mp3'   |
| gain     | number                                                                          | 可选，音量增益。正常为 1，数值越大，声音越响。                           |
| position | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc) | 可选，声音播放的位置。可以指定在某个实体身上发出声音。                   |
| radius   | number                                                                          | 可选，声音范围。默认为 32，即 2 格方块距离。超出范围的玩家则听不到声音。 |
| pitch    | number                                                                          | 可选，音高增益。正常为 1，大于 1，声音播放越快，小于 1，声音播放越慢。   |

 简单示例

示例代码2

💡提示
除了world.sound()，[Entity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)和[Player](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0)也拥有类似播放声音的功能。
使用 [entity.sound()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#V6C4l) 可以在实体的位置播放声音，设置radius范围后，周围的玩家都可以听见声音。
使用 [player.sound()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#YFchP) 仅某个玩家自己可以听到声音，其他玩家都听不到。
Game世界预设了一些声音属性，在对应的事件触发时播放音效： 当地图开始运行时循环播放的[背景音乐](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#Yn7CB)，
当任意[玩家进入/离开地图时](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#PojOY)时播放的音效，
当任意[方块被放置/破坏](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#EBTEk)时播放的音效。

world.ambientSound
属性     属性值类型：new GameSoundEffect()     默认值：''
改变地图背景音乐，从地图运行开始循环播放。
背景音乐的音量会根据用户在[设置-声音]更改。

world.playerJoinSound

属性    属性值类型：new GameSoundEffect()    默认值：''
当玩家进入地图时，播放的音效。通过[world.onPlayerJoin()](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#P6gUg)触发。

world.playerLeaveSound

属性    属性值类型：new GameSoundEffect()    默认值：''
当玩家离开地图时，播放的音效。通过[world.onPlayerLeave()](https://box3.yuque.com/staff-khn556/wupvz3/gqdnaany8xlb0q0s#mUHUB)触发。

world.placeVoxelSound

属性    属性值类型：new GameSoundEffect()    默认值：'audio/place_block.mp3'
方块被放置时，播放的音效。通过[GameVoxels.setVoxel()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gkz7g1wazf5izpfy#kuAQe)触发。默认音效为'audio/place_block.mp3'

world.breakVoxelSound

属性    属性值类型：new GameSoundEffect()    默认值：'audio/break_block.mp3'
方块被销毁时，播放的音效。通过[GameVoxels.setVoxel()](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gkz7g1wazf5izpfy#kuAQe)触发。默认音效为'audio/break_block.mp3'

Weather 天气：雾

world.maxFog
属性     属性值类型：number     默认值：1
最大雾量。对应编辑器菜单[场景-全局特效-雾气-最大雾量]控件属性。

world.fogColor
属性     属性值类型：number     默认值：new GameRGBColor(1, 1, 1)
雾的颜色。对应编辑器菜单[场景-全局特效-雾气-颜色]控件属性。

world.fogStartDistance
属性     属性值类型：number     默认值：0
●fogStartDistance: number = 0
雾起始距离。对应编辑器菜单[场景-全局特效-雾气-起始距离]控件属性。

world.fogHeightOffset
属性     属性值类型：number     默认值：0
雾起始高度。对应编辑器菜单[场景-全局特效-雾气-高度]控件属性。

world.fogUniformDensity
属性     属性值类型：number     默认值：0
雾均匀密度，对应编辑器菜单[场景-全局特效-雾气-均匀雾量]控件属性。
若值大于0，越难看到天空。

world.fogHeightFalloff
属性     属性值类型：number     默认值：0.8
雾衰减的速率。对应编辑器菜单 [场景-全局特效-雾气-高度衰减系数] 控件属性。
数值在0-1之间。值越小，雾越浓。

Weather 天气：雨

world.rainSpeed
属性     属性值类型：number     默认值：1
雨的速度。对应编辑器菜单[场景-全局特效-雨-速度]控件属性。

world.rainColor
属性     属性值类型：GameRGBAColor     默认值：new GameRGBAColor(1, 1, 1, 1)
雨的颜色。对应编辑器菜单[场景-全局特效-雨-颜色]控件属性。

world.rainDirection
属性     属性值类型：GameVector3     默认值：new GameVector3(0, 1, 0)
雨的方向。对应编辑器菜单[场景-全局特效-雨-方向]控件属性。

world.rainDensity
属性     属性值类型：number     默认值：0
雨的密度。对应编辑器菜单[场景-全局特效-雨-密度]控件属性。
密度越大，雨滴越多。

world.rainInterference
属性     属性值类型：number     默认值：0
雨的扰动幅度。对应编辑器菜单[场景-全局特效-雨-不规则性]控件属性。

world.rainSizeLo
属性     属性值类型：number     默认值：0
雨滴的最小直径。

world.rainSizeHi
属性     属性值类型：number     默认值：1
雨滴的最大直径。

Weather 天气：雪

world.snowColor
属性     属性值类型：GameRGBAColor     默认值：new GameRGBAColor(1, 1, 1, 1)
雪花颜色。

world.snowTexture
属性     属性值类型：string     默认值：''
雪花纹理。此处填写文件管理器中的纹理资源名称。如 'snow/heart.part'

world.snowDensity
属性     属性值类型：number     默认值：0
雪的密度。密度越大，雪花越多。

world.snowFallSpeed
属性     属性值类型：number     默认值：1
雪花下落速度。如果小于0，则反向运动。

world.snowSpinSpeed
属性     属性值类型：GameVector3     默认值：new GameVector3(0, 0, 0)
雪花自旋速度。

world.snowSizeLo
属性     属性值类型：number     默认值：0
雪花最小直径。

world.snowSizeHi
属性     属性值类型：number     默认值：1
雪花最大半径。

Weather 天气: 光照

world.lightMode
属性     属性值类型：string     默认值：'natural'
作用于天空和环境光的照明类型。对应编辑器设置 [场景-日光-日光规律] 控件属性。
目前有提供2种光照模式，'manual'(自定义)或'natural'(动态)。默认为 'natural'。

world.sunFrequency
属性     属性值类型：number     默认值：0
太阳运动的频率，数值越大，昼夜交替越快。
昼夜时间计算公式:timeOfDay = (sunPhase + sunFrequency * tick) % 1

world.sunPhase
属性     属性值类型：number     默认值：0     范围：0-1
太阳从升起至落下，在天空的初始位置。对应编辑器菜单 [场景-日光] 控件属性。
数值在0-1之间。大于0.5时，世界进入黑夜。 仅在日光规律为 natural 状态时生效。
💡提示
关于太阳位置和世界时间的关系：
太阳位置 sunPhase = 0 世界时间为 06:00
太阳位置 sunPhase = 0.25 世界时间为 12:00
太阳位置 sunPhase = 0.5 世界时间为 18:00
太阳位置 sunPhase = 0.75 世界时间为第二天 00:00
太阳位置 sunPhase = 1 世界时间为第二天 06:00

world.sunDirection
属性     属性值类型：GameVector3     默认值：new GameVector3(0, -1, 0)
太阳光照明方向。仅在光照模式为manual自定义模式时生效。

world.sunLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(1000, 1000, 1000)
太阳光颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyLeftLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在-X轴方向的亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyRightLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在+X轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyBottomLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在-Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyTopLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在+Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyFrontLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在-Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

world.skyBackLight
属性     属性值类型：GameRGBColor     默认值：new GameRGBColor(0, 0, 0)
环境光在+Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。
颜色值大于0时，颜色越亮。

动画

world.animate()
方法
创建一个关键帧动画[GameAnimation](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ritpgy64d053qg64)。
参数

| 名称         | 类型                                                                                            | 说明         |
| ------------ | ----------------------------------------------------------------------------------------------- | ------------ |
| keyframes    | [GameWorldKeyframe](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gz8i9v7feiuz8cm6)[]         | 关键帧的数据 |
| playbackInfo | [GameAnimationPlaybackConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/yccnow4dplv1lldk) | 动画播放参数 |

返回值

| 名称      | 类型                                                                              | 说明               |
| --------- | --------------------------------------------------------------------------------- | ------------------ |
| Animation | [GameAnimation](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ritpgy64d053qg64) | 创建出来的动画对象 |

Web相关

world.url
属性     属性值类型：[URL](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/vvy0hopvp0bmgb1b)
获取当前地图所在的URL链接地址。

商城

world.onPlayerPurchaseSuccess()
事件
当玩家成功购买物品时触发
●onPlayerPurchaseSuccess : [GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)< [GamePurchaseSuccessEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oue67nqv8mfga7av) >
●nextPlayerPurchaseSuccess : [GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1) < [GamePurchaseSuccessEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/oue67nqv8mfga7av) >

返回值 GamePurchaseSuccessEvent:{ tick, userId, ProductId, orderId }

| 名称      | 类型   | 说明                     |
| --------- | ------ | ------------------------ |
| tick      | number | 购买成功事件发生的时间   |
| userId    | string | 触发购买事件的玩家userId |
| productId | number | 购买商品的ID             |
| orderId   | number | 购买成功的订单号         |

Teleport 传送

world.teleport()
方法
地图组内传送能力，能够令 Player 被传送到其他地图中。此能力受权限影响，无权限用户可见，但调用后直接报错。
参数 mapId, players

| 名称    | 类型                                                                             | 说明                         |
| ------- | -------------------------------------------------------------------------------- | ---------------------------- |
| mapId   | string                                                                           | 必填，目标地图id             |
| players | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)[] | 必填，被传送的玩家entity数组 |

需注意：
●传送进入的地图为独立服务器，因此同一张目标地图，分批次传送不同的人，所进入的是不同服务器。
●只能在已发布地图中生效
●players的长度不能超过50
●players中不能存在游客（没有UserID）

简单示例

1

2

3

4

5

6

7

8

9

10

11

12

while (true) {

    try {

    let players = world.querySelectorAll('player').slice(0, 50)

    players = players.filter(e => e.player.userId !== '' && e.player.userId !== '0' && e.player.userId !== 0)

    world.teleport('100001157', players)

    break

    } catch (e) {

    world.say('传送失败：' + e.stack)

    }

    await sleep(1000)

}

world.say('传送成功 ')

## GameZone 区域

类 - GameZone
区域可用于检测实体进入某个区域或离开。 也可以用来设置环境参数，如雾、雨、天、雪、风、重力等定义区域内的环境参数。

参数
●bounds
●entities
●selector
●nextEnter
●nextLeave
●onEnter
●onLeave
●remove
●force
●massScale
●fogColor
●fogDensity
●fogEnabled
●fogHeightFalloff
●fogHeightOffset
●fogMax
●fogStartDistance
●rainColor
●rainDensity
●rainDirection
●rainEnabled
●rainInterference
●rainSizeHi
●rainSizeLo
●rainSpeed
●skyBackLight
●skyBottomLight
●skyEnabled
●skyFrontLight
●skyLeftLight
●skyLunarPhase
●skyMode
●skyRightLight
●skySunDirection
●skySunFrequency
●skySunLight
●skySunPhase
●skyTopLight
●snowColor
●snowDensity
●snowEnabled
●snowFallSpeed
●snowSizeHi
●snowSizeLo
●snowSpinSpeed
●snowTexture

bounds
•bounds:[GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)‹›= new GameBounds3( new GameVector3(0, 0, 0), new GameVector3(0, 0, 0))
该区域的所指定的检测区域

entities
•entities:function
在区域内的全部实体[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)

函数声明:
▸ ():[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)[]

fogColor
•fogColor:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(1, 1, 1)
区域内雾的颜色

fogDensity
•fogDensity:number= 0
区域内雾均匀密度

fogEnabled
•fogEnabled:boolean= false
区域内雾是否开启
示例代码

fogHeightFalloff
•fogHeightFalloff:number= 0.8
区域内雾衰减的速率

fogHeightOffset
•fogHeightOffset:number= -8
区域内雾起始高度

fogMax
•fogMax:number= 1
区域内最大雾量

fogStartDistance
•fogStartDistance:number= 0
区域内雾起始距离

force
•force:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)‹›= new GameVector3(0, 0, 0)
对物体施加的力的大小
示例代码

massScale
•massScale:number= 0
控制物体的质量对力的影响程度。 0 = 像重力一样 1 = 像风一样

onEnter

nextEnter
•onEnter:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameTriggerEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)›
•nextEnter:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameTriggerEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)›
有实体进入指定区域时，触发事件

onLeave

NextLeave
•onLeave:[GameEventChannel](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)‹[GameTriggerEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)›
•nextLeave:[GameEventFuture](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/azxgcc43ibscl5z1)‹[GameTriggerEvent](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/onor4cnp3rhr4060)›
有实体离开区域时触发事件
示例代码

rainColor
•rainColor:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)‹›= new GameRGBAColor(1, 1, 1, 1)
区域内雨的颜色

rainDensity
•rainDensity:number= 0
区域内雨的密度 密度越大，雨滴越多。

rainDirection
•rainDirection:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)‹›= new GameVector3(0, 1, 0)
区域内雨的方向

rainEnabled
•rainEnabled:boolean= false
区域内雨是否开启
示例代码

rainInterference
•rainInterference:number= 0
区域内雨的扰动幅度

rainSizeHi
•rainSizeHi:number= 1
区域内雨滴的最大直径

rainSizeLo
•rainSizeLo:number= 0
区域内雨滴的最小直径

rainSpeed
•rainSpeed:number= 1
区域内雨的速度

remove
•remove:function
把该区域删除

函数声明:
▸ ():void

selector
•selector:[GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9)= ""
触发区域事件的物体搜索条件

skyBackLight
•skyBackLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内环境光在+Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skyBottomLight
•skyBottomLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内境光在-Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skyEnabled
•skyEnabled:boolean= false
区域内环境参数是否有效
示例代码

skyFrontLight
•skyFrontLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内环境光在-Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skyLeftLight
•skyLeftLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内环境光在-X轴方向的亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skyLunarPhase
•skyLunarPhase:number= 0
区域内月亮的相位，数值在0和1之间。若大于0.5时，为上弦月。

skyMode
•skyMode:"natural" | "manual"= "natural"
区域内作用于天空和环境光的照明类型。目前有提供2种光照模式，'manual'(自定义)或'natural'(动态)。默认为 'natural'。示例代码

skyRightLight
•skyRightLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内环境光在+X轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skySunDirection
•skySunDirection:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)‹›= new GameVector3(0, -1, 0)
区域内太阳光照明方向。仅在光照模式为manual自定义模式时生效。

skySunFrequency
•skySunFrequency:number= 0
区域内太阳运动的频率，数值越大，昼夜交替越快。

skySunLight
•skySunLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(1000, 1000, 1000)
区域内太阳光颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

skySunPhase
•skySunPhase:number= 0
区域内太阳从升起至落下，在天空的位置。

skyTopLight
•skyTopLight:[GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)‹›= new GameRGBColor(0, 0, 0)
区域内环境光在+Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。

snowColor
•snowColor:[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)‹›= new GameRGBAColor(1, 1, 1, 1)
区域内雪花颜色

snowDensity
•snowDensity:number= 0
区域内雪的密度。密度越大，雪花越多。

snowEnabled
•snowEnabled:boolean= false
区域内雪是否开启
示例代码

snowFallSpeed
•snowFallSpeed:number= 1
区域内雪花下落速度。如果小于0，则反向运动。

snowSizeHi
•snowSizeHi:number= 1
区域内雪花最大半径

snowSizeLo
•snowSizeLo:number= 0
区域内雪花最小直径

snowSpinSpeed
•snowSpinSpeed:number= 0
区域内雪花自旋速度

snowTexture
•snowTexture:string= ""
区域内雪花纹理

更多代码示例

```javascript
// 一半酸雨, 一半樱花飘落的场景效果, 跳起来场景效果消失

world.addZone({

  selector: 'player',

  bounds: {

    lo: [0, 0, 64],

    hi: [128, 10, 128],

  },

  rainEnabled: true,

  rainDensity: 0.5,

  rainSpeed: 0.5,

  snowEnabled: true,

  snowDensity: 0.5,

  snowTexture: 'snow/bubble.part',

  snowFallSpeed: -0.1,

  fogEnabled: true,

  fogColor: new GameRGBColor(0.5, 1, 0),

  fogDensity: 0.02,

})

world.addZone({

  selector: 'player',

  bounds: {

    lo: [0, 0, 0],

    hi: [128, 10, 64],

  },

  rainEnabled: true,

  rainDensity: 0.5,

  rainSpeed: -0.5,

  snowEnabled: true,

  snowDensity: 0.5,

  snowTexture: 'snow/sakura.part',

  snowFallSpeed: 0.1,

  fogEnabled: true,

  fogColor: new GameRGBColor(1, 0, 0.5),

  fogDensity: 0.02,

})
```

## ServerEvent

类 - ServerEvent
从客户端发往服务器的自定义事件。

属性

tick
number
事件产生时的客户端 Tick。

entity
[GamePlayerEntity](https://box3.yuque.com/staff-khn556/wupvz3/kgrabhf749axn65y)
事件产生的来源用户。

args
any
客户端通过该事件发送的数据。

## ServerRemoteChannel

类 - ServerRemoteChannel
管理客户端与服务端通信的系统， 与客户端脚本中的 [ClientRemoteChannel](https://box3.yuque.com/staff-khn556/wupvz3/te1en17qs6c5cont)

 配合使用。

方法

sendClientEvent
(entities:[GamePlayerEntity](https://box3.yuque.com/staff-khn556/wupvz3/kgrabhf749axn65y)|[GamePlayerEntity](https://box3.yuque.com/staff-khn556/wupvz3/kgrabhf749axn65y)[], clientEvent:any) : void
向指定玩家发送客户端事件。

参数
●entities:[GamePlayerEntity](https://box3.yuque.com/staff-khn556/wupvz3/kgrabhf749axn65y)|[GamePlayerEntity](https://box3.yuque.com/staff-khn556/wupvz3/kgrabhf749axn65y)[] - 玩家实体列表，代表发送对象，传入空数组时不会产生任何效果
●clientEvent:any - 自定义事件，在客户端接收到时，传入监听器的参数，仅允许可序列化的值

broadcastClientEvent
(clientEvent:any) : void
向所有玩家广播客户端事件。

参数
●clientEvent:any - 自定义事件对象，在客户端接收到时，传入监听器的参数，仅允许可序列化的值

onServerEvent
[GameEventChannel](https://box3.yuque.com/staff-khn556/wupvz3/wkgxqor9a2i34oet)[[ServerEvent](https://box3.yuque.com/staff-khn556/wupvz3/du8np88uv0scn51v)](%5BServerEvent%5D(https://box3.yuque.com/staff-khn556/wupvz3/du8np88uv0scn51v))
监听客户端发来的服务端事件。

## QueryList 数据查询列表

Class: QueryList
键值对查询列表，用于批量获取键值对，通过 {GameDataStorage.list} 方法返回。
列表根据配置项被划分为一个或多个分页，每个分页最多包含 { [ListPageOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ugyg698kg8940k4d) | pageSize} 个键值对。

基本

isLastPage
• isLastPage: boolean
是否为最后一页，如果翻过头了，也会为 true

getCurrentPage
• getCurrentPage: function
按 {[ListPageOptions](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ugyg698kg8940k4d) | pageSize} 获取当前页的键值对

函数声明:
▸ (): [ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)[]

返回值:[ReturnValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ofrqlqsh7eq81xw7)[]
返回当前页的键值对内容

nextPage
• nextPage : function
翻到下一页，执行后 {getCurrentPage} 将返回下一页的键值对内容

函数声明:
▸ (): Promise `<void>`

返回值:Promise `<void>`
返回 Promise 对象，resolve表示翻页成功，reject 后表示翻页失败

# Types-类型

## JSONValue 类JSON格式

类型别名 - JSONValue
允许存储的值，类型可以是如下类型之一：

| 类型                                                                                                   | 描述                                                                                        |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------- |
| string                                                                                                 | 字符串                                                                                      |
| number                                                                                                 | 数字                                                                                        |
| boolean                                                                                                | 布尔值                                                                                      |
| { [x: string]:[JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zz3qof7bfzaxst46#JSONValue)} | 键值对                                                                                      |
| [JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zz3qof7bfzaxst46#JSONValue)[]              | [JSONValue](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zz3qof7bfzaxst46#JSONValue)数组 |

定义

```javascript
export type JSONValue =

  string

  | number

  | boolean

  |{ [x: string]: JSONValue }

  | JSONValue[];
```

## ListPageOption 列表翻页配置

类型别名 - ListPageOptions
批量获取键值对的配置项。

定义

●cursor:number
○分页指针，用于指定本次获取的分页起点页码。
●pageSize?:number
○可选项，分页大小，一页内的数据量，默认100。
●constraintTarget?:string
○约束目标值的路径，当值是JSON格式时，指定用作排序的值的路径。例如传入 score时，会取值上score属性的值作为排序、最大最小值的限制目标；
○可以级联最多5级，例如a.b.c.d.e，超出视作非法参数，按下一条方式处理；
○当路径不存在或传入非法参数时，以值本身作为目标进行排序，并打印一条警告；
●ascending?:boolean - 是否升序，设置为 true 时为升序，false为降序，不传或传入undefined时不排序；
●max?:number - 最大值，过滤返回对应值的最大值，超出或非数字则不返回该Key，默认不过滤；
●min?:number - 最小值，同max类似。

## GameAnimationPlaybackConfig 动画播放配置参数

接口 - GameAnimationPlaybackConfig
用于动画播放配置的参数组

| 参数           | 类型                                                                                       | 说明             |
| -------------- | ------------------------------------------------------------------------------------------ | ---------------- |
| delay          | number                                                                                     | 播放延迟         |
| direction      | [GameAnimationDirection](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/cgylgydyg35npvup) | 播放方向         |
| duration       | number                                                                                     | 播放时长         |
| endDelay       | number                                                                                     | 结束延迟         |
| iterationStart | number                                                                                     | 反复播放开始时间 |
| iterations     | number                                                                                     | 反复播放次数     |
| startTick      | number                                                                                     | 开始时间         |

## GameDialogCall 显示对话框

类型别名 - GameDialogCall
GameDialogCall:function
在游戏中显示一个对话框。
目前支持3种对话框样式：[文本框 Text](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wc7bX)/[选项框 Select](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#c8eCh)/[输入框 Input](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Rj3dZ)
GameDialogCall =
((params:[GameTextDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wc7bX)) => Promise<[GameDialogResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#ZhwoF)| null> &[GameDialogCancelOption](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wy4Sc)) |
((params:[GameSelectDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#c8eCh)) => Promise<[DialogSelectResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#BxeyE)| null> &[GameDialogCancelOption](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wy4Sc)) |
((params:[GameInputDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Rj3dZ)) => Promise<[GameDialogResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#ZhwoF)| null> &[GameDialogCancelOption](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wy4Sc)) |

[GameDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#i6mSU)
对话框类型
●文本对话框[GameTextDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Wc7bX)
●选项对话框[GameSelectDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#c8eCh)
●输入对话框[GameInputDialogParams](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#Rj3dZ)

[GameDialogResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#ok30Y)
对话框输入响应
●[DialogSelectResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#BxeyE)

GameDialogParams
对话框属性列表
GameDialogParams:object

类型声明:
●type:[GameDialogType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)
对话框的类型。目前有三种对话框类型，具体可查看[GameDialogType](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)
●content: string
对话框显示的正文内容。支持使用'\n' 换行。
●contentBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
对话框正文窗口的背景颜色。
●contentTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
对话框正文字体的颜色。
●title:string
对话框显示的标题名称。
●titleBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
对话框显示的标题窗口背景颜色。
●titleTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
对话框显示的标题字体颜色。
●hasArrow? :undefined | false | true
可选: 如果接下来还有新的对话，在当前对话框中是否显示箭头提示。
仅在文本对话框[GameDialogType.TEXT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)中使用。
●confirmText? :undefined | string
可选: 仅在输入对话框[GameDialogType.INPUT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)使用。
确认按钮显示的文本。如果为空，按钮文本默认显示为 '确认 | Confirm'.
●options? :string[]
可选: 仅在选项对话框[GameDialogType.SELECT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)中使用。
在对话框中提供一些可供玩家选择的对话选项。
●placeholder? :undefined | string
可选: 仅在输入对话框[GameDialogType.INPUT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)中使用。
在输入框背景显示的提示文字。
●lookTarget?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
可选: 使相机镜头朝向指定实体或坐标的位置。
●lookTargetOffset?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
可选: 如果相机指定了注视目标，可以设置基于目标位置的偏移。
●lookUp?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
可选: 调整相机抬头向量。使画面上下左右颠倒。
●lookEye?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
可选: 调整相机的位置。
●lookEyeOffset?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
可选: 如果相机位置指定了实体，可以设置基于目标位置的偏移。

GameTextDialogParams
文本对话框参数
GameTextDialogParams:object

类型声明:
●type:[GameDialogType.TEXT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)
对话框类型。文本对话框的类型是GameDialogType.TEXT
●hasArrow? :undefined | false | true
是否显示箭头提示
●content: string
对话框显示的正文内容。支持使用'\n' 换行。
●contentBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文背景颜色
●contentTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文字体颜色
●title:string
对话框标题
●titleBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题背景颜色
●titleTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题正文颜色
●lookTarget? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机注视的实体
●lookTargetOffset? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机注视的位置偏移
●lookUp? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
相机抬头向量
●lookEye?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机镜头的位置
●lookEyeOffset ?: [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机位置的偏移

GameSelectDialogParams
选项对话框参数
GameSelectDialogParams:object

类型声明:
●type:[GameDialogType.SELECT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)
对话框类型。选项对话框的类型是GameDialogType.SELECT
●options? :string[]
选项列表
●content: string
对话框显示的正文内容。支持使用'\n' 换行。
●contentBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文背景颜色
●contentTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文字体颜色
●title:string
对话框标题
●titleBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题背景颜色
●titleTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题正文颜色
●lookTarget? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机注视的实体
●lookTargetOffset? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机注视的位置偏移
●lookUp? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
相机抬头向量
●lookEye?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机镜头的位置
●lookEyeOffset?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机位置的偏移

GameInputDialogParams
输入对话框参数
GameInputDialogParams:object

类型声明:
●type:[GameDialogType.INPUT](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/nordqvgc2xoeq28p)
对话框类型。输入对话框的类型是GameDialogType.INPUT
●confirmText? :undefined | string
确认按钮文字
●placeholder? :undefined | string
输入框提示文字
●content: string
对话框显示的正文内容。支持使用'\n' 换行。
●contentBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文背景颜色
●contentTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
正文字体颜色
●title:string
对话框标题
●titleBackgroundColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题背景颜色
●titleTextColor? :[GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)
标题正文颜色
●lookTarget? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机注视的实体
●lookTargetOffset? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机注视的位置偏移
●lookUp? :[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
相机抬头向量
●lookEye?:[GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)|[GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)
相机镜头的位置
●lookEyeOffset ?: [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)
基于相机位置的偏移

GameDialogResponse
对话框回应
如果没有完成对话而点击了其他地方，使对话框被取消，则返回null
如果是文本对话框，回应'success'
如果是选项对话框，回应输入框填写的内容字符串
如果是选项对话框，回应[DialogSelectResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#BxeyE)
GameDialogResponse:[DialogSelectResponse](https://box3.yuque.com/staff-khn556/wupvz3/extmobyyfsaec26x#BxeyE)| string = 'success' | null

DialogSelectResponse
选项对话框回应
在选项对话框中，玩家点击了按钮，会得到对话框的回应事件。返回被玩家按下的选项信息。
DialogSelectResponse:object

类型声明:
●选项编号index:number（zero-based 从0开始计数）
●选项内容value:string

GameDialogCancelOption
GameDialogCancelOption:object

函数声明:
●cancel():function
关闭对话框。

综合示例 1

```javascript
world.onPlayerJoin(async ({ entity }) => {

  // 玩家进入游戏时，弹出一个欢迎对话框

  const dialog = entity.player.dialog({

    type: GameDialogType.TEXT,

    title: "吉吉喵",

    content:`你好，${entity.player.name}，很高兴认识你。`,

  });

  // 等待任何一个 [玩家点击或关闭对话框， 3秒后自动把对话框关闭]

  Promise.race([

    dialog,

    (async() => {

    await sleep(3000);

    dialog.cancel();

    })()

  ]).then( /* 任何一个函数返回 */ );

})
```

综合示例 2

```javascript
world.onPlayerJoin(async ({ entity }) => {

  // 玩家进入游戏时，弹出一个欢迎对话框

  const dialog = entity.player.dialog({

    type: GameDialogType.TEXT,

    title: "吉吉喵",

    content: `你好，${entity.player.name}，很高兴认识你。`,

  });

  // 3秒后自动关闭

  setTimeout(()=>{

    dialog.cancel();

  },3000);

})
```

## GameEntityConfig 实体配置参数

接口 - GameEntityConfig
用于控制实体的参数组

| 参数                   | 类型                                                                                | 说明                                       |
| ---------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------ |
| position               | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 实体的位置                                 |
| velocity               | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 实体朝向某个方向运动的作用力               |
| collides               | boolean                                                                             | 实体是否可碰撞                             |
| mesh                   | string                                                                              | mesh决定了实体的外形。'mesh/*.vb'          |
| meshColor              | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)   | 实体的颜色                                 |
| meshScale              | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 实体的缩放比例                             |
| meshOrientation        | [GameQuaternion](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ci4biyw0qruafkf2)  | 实体的旋转角度                             |
| meshMetalness          | number                                                                              | 实体的金属感                               |
| meshEmissive           | number                                                                              | 实体的发光度                               |
| meshShininess          | number                                                                              | 实体的反光度                               |
| gravity                | boolean                                                                             | 实体是否会下落                             |
| fixed                  | boolean                                                                             | 实体的位置是否固定不动                     |
| mass                   | number                                                                              | 实体质量                                   |
| friction               | number                                                                              | 实体的粘性(0 = 滑，1 = 粘)                 |
| restitution            | number                                                                              | 实体的弹性(0 = 软, 1 = 弹)                 |
| enableInteract         | boolean                                                                             | 允许实体进行互动                           |
| interactRadius         | number                                                                              | 进入实体互动的范围。范围越小，需更靠近。   |
| interactHint           | string                                                                              | 进入实体互动范围时，实体身上出现的提示文本 |
| interactColor          | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)   | 进入实体互动范围时，提示文本的字体颜色     |
| particleRate           | number                                                                              | 实体每秒产生粒子的数量                     |
| particleRateSpread     | number                                                                              | 增加实体每秒产生粒子数量的随机性           |
| particleLimit          | number                                                                              | 实体可产生粒子总数的上限                   |
| particleLifetime       | number                                                                              | 实体所产生粒子能存活的秒数                 |
| particleLifetimeSpread | number                                                                              | 增加实体所产生粒子存活时间的随机性         |
| particleSize           | number[]                                                                            | 实体所产生粒子的大小变化                   |
| particleSizeSpread     | number                                                                              | 增加实体所产生粒子大小的随机性             |
| particleColor          | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)[]  | 实体所产生粒子的颜色变化                   |
| particleVelocity       | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 实体所产生粒子的初始速度                   |
| particleVelocitySpread | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 增加实体所产生粒子初始速度的随机性         |
| particleDamping        | number                                                                              | 实体所产生粒子的阻尼系数                   |
| particleAcceleration   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)     | 实体所产生粒子的加速度                     |
| particleNoise          | number                                                                              | 实体所产生粒子摆动的最大幅度               |
| particleNoiseFrequency | number                                                                              | 实体所产生粒子摆动的频率                   |
| chatSound              | [GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2) | 实体触发说话事件时播放的音效               |
| interactSound          | [GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2) | 实体触发互动事件时播放的音效               |
| hurtSound              | [GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2) | 实体触发受伤事件时播放的音效               |
| dieSound               | [GameSoundEffect](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ucndfavnw4hpxiu2) | 实体触发死亡事件时播放的音效               |

## GameEntityKeyframe 实体动画关键帧

接口 - GameEntityKeyframe
Entity实体动画关键帧参数，可对Entity除音效外的大部分属性做动画效果，例如位移、大小、模型、颜色等等

| 参数                   | 类型                                                                               | 说明                                       |
| ---------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------ |
| duration               | number                                                                             | 播放时长                                   |
| easeIn                 | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)     | 缓入效果                                   |
| easeOut                | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)     | 缓出效果                                   |
| velocity               | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 实体朝向某个方向运动的作用力               |
| collides               | boolean                                                                            | 实体是否可碰撞                             |
| mesh                   | string                                                                             | mesh决定了实体的外形。'mesh/*.vb'          |
| meshColor              | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)  | 实体的颜色                                 |
| meshScale              | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 实体的缩放比例                             |
| meshOrientation        | GameQuaternion                                                                     | 实体的旋转角度                             |
| meshMetalness          | number                                                                             | 实体的金属感                               |
| meshEmissive           | number                                                                             | 实体的发光度                               |
| meshShininess          | number                                                                             | 实体的反光度                               |
| gravity                | boolean                                                                            | 实体是否会下落                             |
| fixed                  | boolean                                                                            | 实体的位置是否固定不动                     |
| mass                   | number                                                                             | 实体质量                                   |
| friction               | number                                                                             | 实体的粘性(0 = 滑，1 = 粘)                 |
| restitution            | number                                                                             | 实体的弹性(0 = 软, 1 = 弹)                 |
| enableInteract         | boolean                                                                            | 允许实体进行互动                           |
| interactRadius         | number                                                                             | 进入实体互动的范围。范围越小，需更靠近。   |
| interactHint           | string                                                                             | 进入实体互动范围时，实体身上出现的提示文本 |
| interactColor          | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)  | 进入实体互动范围时，提示文本的字体颜色     |
| particleRate           | number                                                                             | 实体每秒产生粒子的数量                     |
| particleRateSpread     | number                                                                             | 增加实体每秒产生粒子数量的随机性           |
| particleLimit          | number                                                                             | 实体可产生粒子总数的上限                   |
| particleLifetime       | number                                                                             | 实体所产生粒子能存活的秒数                 |
| particleLifetimeSpread | number                                                                             | 增加实体所产生粒子存活时间的随机性         |
| particleSize           | number[]                                                                           | 实体所产生粒子的大小变化                   |
| particleSizeSpread     | number                                                                             | 增加实体所产生粒子大小的随机性             |
| particleColor          | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)[] | 实体所产生粒子的颜色变化                   |
| particleVelocity       | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 实体所产生粒子的初始速度                   |
| particleVelocitySpread | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 增加实体所产生粒子初始速度的随机性         |
| particleDamping        | number                                                                             | 实体所产生粒子的阻尼系数                   |
| particleAcceleration   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 实体所产生粒子的加速度                     |
| particleNoise          | number                                                                             | 实体所产生粒子摆动的最大幅度               |
| particleNoiseFrequency | number                                                                             | 实体所产生粒子摆动的频率                   |

## GameEventChannel 事件频道监听

类型别名 - GameEventChannel

描述
EventChannel 可用于监听指定对象的事件。输入事件处理器handler，即得取消此事件处理器的[GameEventHandlerToken](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/su72pndir0p5c7hh)

，各类用于监听事件的onXXX方法均为此类型的实现。

定义

GameEventChannel

```javascript
export type GameEventChannel `<EventType>` = (

  handler: (event: EventType) => void,

) => GameEventHandlerToken;
```

●EventType- 泛型参数，用于指定事件类型
●handler:(event: EventType) => void-  事件发生时调用的处理器

示例

1秒后停止监听onTick

```javascript
// 1000毫秒后停止报时

const token = world.onTick(() => console.log("tick !"));

setTimeout(() => {

  console.log('cancel tick handler');

  token.cancel();// 取消记录tick事件

}, 1000);
```

## GameEventFuture 事件单次监听

类型别名 - GameEventFuture

描述
此类型为[GameEventChannel 事件频道监听](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/wkgxqor9a2i34oet)

的单次、Promise版本。
Promise（承诺）提供了另一种处理事件的方式。您可以使用Promise来组织长序列的事件，从而实现结构化编程。
配合 async/await语法使用，可以以类似同步代码的方式组织异步代码。在某些情况下，这可以使代码更简单和更清晰，但必须谨慎使用。
尽管看起来与同步代码十分相似，但异步代码在等待时可以被中断，这意味着世界中的事物可能会在您的代码之外发生变化。
此外，异步代码生成的错误不会显示堆栈跟踪，这可能会加大调试的难度。
请考虑这些因素，并谨慎使用Promise、async/await。

定义

GameEventFuture

```javascript
export type GameEventFuture `<EventType>` = (

  filter?: (event: EventType) => boolean,

) => Promise `<EventType>`;
```

●EventType- 触发的事件对象的类型
●filter?:(event: EventType) => boolean - 一个可选的函数，用于检查事件的类型。触发事件前执行该函数并传入事件对象，如果返回false，则不会触发该事件

示例

以 async/await 方式使用

```javascript
// Wait for 2 players to enter the world

async function waitForPlayers (count) {

    while (world.querySelectorAll('player').length < 2) {

    const { entity } = await world.nextPlayerJoin();

    world.say(entity.player.name + ' joined');

    }

}

waitForPlayers.then(() => world.say('game ready'));
```

## GameHurtOptions 实体伤害参数

接口: GameHurtOptions
攻击/伤害的相关参数

| 参数       | 类型                                                                           | 说明                 |
| ---------- | ------------------------------------------------------------------------------ | -------------------- |
| attacker   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y) | 发出攻击的实体       |
| damageType | string                                                                         | 伤害类型，可自行定义 |

## GamePlayerKeyframe 玩家动画关键帧

接口 - GamePlayerKeyframe
Player玩家动画关键帧参数，可对Player的大部分属性做动画效果，例如尺寸、颜色、隐身等等

| 参数           | 类型                                                                               | 说明                                                                  |
| -------------- | ---------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| duration       | number                                                                             | 播放时长                                                              |
| easeIn         | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)     | 缓入效果                                                              |
| easeOut        | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)     | 缓出效果                                                              |
| cameraEntity   | [GameEntity](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y)     | 在第一人称视角(FPS)或第三人称跟随视角(FOLLOW)下，玩家视角所跟随的实体 |
| cameraMode     | [GameCameraMode](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kg0ggd71y96dlu0w) | 视角模式                                                              |
| cameraPosition | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 固定视角(FIXED)下，镜头的眼睛位置                                     |
| cameraTarget   | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 固定视角(FIXED)下镜头所朝向的目标点                                   |
| cameraUp       | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 固定视角(FIXED)下，镜头向上的矢量                                     |
| scale          | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)    | 玩家的缩放比例                                                        |
| color          | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)   | 玩家的颜色                                                            |
| colorLUT       | string                                                                             | 用于渲染玩家所见游戏世界的色调                                        |
| invisible      | boolean                                                                            | 玩家是否隐身                                                          |
| emissive       | number                                                                             | 玩家的发光度                                                          |
| metalness      | number                                                                             | 玩家的金属感                                                          |
| shininess      | number                                                                             | 玩家的反光度                                                          |
| showName       | boolean                                                                            | 玩家名字是否显示                                                      |

## GameRaycastOptions 射线检测配置

接口 - GameRaycastOptions
进行射线检测的参数配置

| 参数           | 类型                                                                                   | 说明                       |
| -------------- | -------------------------------------------------------------------------------------- | -------------------------- |
| maxDistance    | number                                                                                 | 允许射线穿越的最大距离     |
| ignoreFluid    | boolean                                                                                | 如果为真，则射线无视液体   |
| ignoreVoxel    | boolean                                                                                | 如果为真，则射线无视方块   |
| ignoreEntities | boolean                                                                                | 如果为真，则射线无视实体   |
| ignoreSelector | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 被射线检测忽略的实体选择器 |

## GameSelectorString 选择器参数

类型别名 - GameSelectorString
typeGameSelectorString= string;
选择器(Selectors)可以方便搜索游戏内的全部对象。Game的选择器接口是参照 DOM APIs 而设。

```javascript
const entities = world.querySelector('*'); // 世界中的全部实体

const theChair = world.querySelector('#chair'); // 模型名称为"chair"的首个实体

const players = world.querySelectorAll('player'); // 游戏中的全部玩家

const boxes = world.querySelectorAll('.box'); // 标签带有"box"的全部实体

const redBox = world.querySelector('.box .red');// 标签同时带有"box"和“red”的首个实体
```

## GameSkinInvisible 隐藏身体部位参数

类型别名 - GameSkinInvisible
玩家身体可隐藏的部位

| 参数          | 类型    | 说明   |
| ------------- | ------- | ------ |
| hips          | boolean | 臀部   |
| torso         | boolean | 躯干   |
| neck          | boolean | 颈部   |
| head          | boolean | 头     |
| leftShoulder  | boolean | 左肩   |
| leftUpperArm  | boolean | 左上臂 |
| leftLowerArm  | boolean | 左下臂 |
| leftHand      | boolean | 左手   |
| leftUpperLeg  | boolean | 左上腿 |
| leftLowerLeg  | boolean | 左下腿 |
| leftFoot      | boolean | 左脚   |
| rightShoulder | boolean | 右肩膀 |
| rightUpperArm | boolean | 右上臂 |
| rightLowerArm | boolean | 右下臂 |
| rightHand     | boolean | 右手   |
| rightUpperLeg | boolean | 右上腿 |
| rightLowerLeg | boolean | 右下腿 |
| rightFoot     | boolean | 右脚   |

## GameSoundEffect 音效

接口 - GameSoundEffect
使用Sound()方法播放声音时，传入的参数。
●sample
●gain
●gainRange
●pitch
●pitchRange
●radius

属性

sample
•sample:string= ""
声音文件路径。可在文件管理器中上传自定义声音。如'audio/chat.mp3'
在指定声音文件路径时，必须确保文件已经上传在文件管理器中。

radius
•radius:number= 32
声音范围。默认为32。距离实体越近，声音听的越清晰。

gain
•gain:number= 1
音量增益。正常为1，数值越大，声音越响。

gainRange
•gainRange:number= 0
音量增益方差。计算公式为：effect.gain + (Math.random() - 0.5) * effect.gainRange

pitch
•pitch:number= 1
音高增益。正常为1。大于1，声音播放越快。小于1，声音播放越慢。

pitchRange
•pitchRange:number= 0
音高增益方差。计算公式为：effect.pitch + (Math.random() - 0.5) * effect.pitchRange

音效列表

[World Sound 世界音效](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#IyalY)

| 声音                                                                                       | 默认音频文件            | 说明                                          |
| ------------------------------------------------------------------------------------------ | ----------------------- | --------------------------------------------- |
| [ambientSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#Yn7CB)     |                         | 循环播放的背景音乐。                          |
| [playerJoinSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#PojOY)  |                         | 有玩家进入游戏。通过world.onPlayerJoin()触发  |
| [playerLeaveSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/gqdnaany8xlb0q0s#Ugwy4) |                         | 有玩家离开游戏。通过world.onPlayerLeave()触发 |
| [placeVoxelSound](https://docs.box3.codemao.cn/box3world.html#placevoxelsound)                | 'audio/place_block.mp3' | 方块被放置。通过world.setVoxel()触发          |
| [breakVoxelSound](https://docs.box3.codemao.cn/box3world.html#breavoxelsound)                 | 'audio/break_block.mp3' | 方块被破坏。通过world.setVoxel()触发          |

[Entity Sound 实体音效](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#JoZIC)

| 声音                                                                                    | 默认音频文件 | 说明                                      |
| --------------------------------------------------------------------------------------- | ------------ | ----------------------------------------- |
| [chatSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#dmgxA)     |              | 实体说话时。通过entity.say()触发          |
| [hurtSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#Zqgk4)     |              | 实体受伤时。通过entity.onTakeDamage()触发 |
| [dieSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#okad9)      |              | 实体死亡时。通过entity.onDie()触发        |
| [interactSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kgrabhf749axn65y#VdXns) |              | 实体被互动时。通过entity.onInteract()触发 |

[Player Sound 玩家音效](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#gBHmE)

| 声音                                                                                      | 默认音频文件            | 说明                           |
| ----------------------------------------------------------------------------------------- | ----------------------- | ------------------------------ |
| [spawnSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#MjXRW)      | 'audio/spawn.mp3'       | 玩家复活时。                   |
| [jumpSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#GDLnL)       | 'audio/jump.mp3'        | 玩家跳跃时。                   |
| [doubleJumpSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#Mbd5R) | 'audio/double_jump.mp3' | 玩家二段跳时。                 |
| [landSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#Gb76c)       | 'audio/land.mp3'        | 玩家落地时。                   |
| [enterWaterSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#kkEKW) | 'audio/dive.mp3'        | 玩家进入液体时。               |
| [leaveWaterSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#BZOka) | 'audio/splash.mp3'      | 玩家离开液体时。               |
| [stepSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#shkLw)       | 'audio/step.mp3'        | 玩家正在行走，迈出一步时。     |
| [swimSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#sTVFS)       | 'audio/swim.mp3'        | 玩家正在游泳，向前划动时。     |
| [crouchSound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#SaRMV)     |                         | 玩家下蹲时。                   |
| [startFlySound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#U6bte)   |                         | 玩家开始飞行时。               |
| [stopFlySound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#Dbryq)    |                         | 玩家结束飞行时。               |
| [action0Sound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#XVfGj)    |                         | 玩家按下鼠标左键/虚拟按钮A时。 |
| [action1Sound](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ddctd6h29w3myth0#SMvH1)    |                         | 玩家按下鼠标右键/虚拟按钮B时。 |

上传音效
编辑器目前内置了34款音效，可以在菜单-[文件管理]的搜索.mp3查看。点击文件后，会弹出声音文件的详情属性。点击位置即可复制文件路径，在脚本中使用对应的方法播放。
如需上传自定义声音，可以在[文件管理]窗口，点击右下角浮动的加号按钮-[上传音频]。

在哪里下载优质的音效
在互联网中搜索音效时，希望能注重版权意识。使用了某个作者的作品，请务必在作品详情页注明来源。
这里推荐一些授权素材网站，只要遵守网站的使用协议，你便可以将它们免费用在你的作品中。大部分网站非中文站点，但可以借助浏览器翻译工具，进行阅读。
●[zapsplat](https://www.zapsplat.com/)
●[soundbible](http://soundbible.com/)
●[OpenGameArt](https://opengameart.org/art-search-advanced?keys=&field_art_type_tid%5B%5D=13&sort_by=count&sort_order=DESC)
●[小森平的免费音效](https://taira-komori.jpn.org/freesoundtw.html)
●[Free SFX](https://www.freesfx.co.uk/)
●[FreeSound](https://freesound.org/)
●[SoundJay](https://www.soundjay.com/)

## GameWorldKeyframe 世界动画关键帧

接口 - GameWorldKeyframe
World世界动画关键帧参数，可对World的大部分属性做动画效果，例如重力、雨、雾、雪、光照等等

| 参数              | 类型                                                                              | 说明                           |
| ----------------- | --------------------------------------------------------------------------------- | ------------------------------ |
| duration          | number                                                                            | 播放时长                       |
| easeIn            | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)    | 缓入效果                       |
| easeOut           | [GameEasing](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/ufkohwwiumbubphm)    | 缓出效果                       |
| gravity           | number                                                                            | 世界重力                       |
| airFriction       | number                                                                            | 空气阻力                       |
| maxFog            | number                                                                            | 最大雾量                       |
| fogColor          | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)  | 雾的颜色                       |
| fogHeightFalloff  | number                                                                            | 雾衰减的速率                   |
| fogHeightOffset   | number                                                                            | 雾起始高度                     |
| fogStartDistance  | number                                                                            | 雾起始距离                     |
| fogUniformDensity | number                                                                            | 雾均匀密度                     |
| rainColor         | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) | 雨的颜色                       |
| rainDensity       | number                                                                            | 雨的密度                       |
| rainDirection     | number                                                                            | 雨的方向                       |
| rainInterference  | number                                                                            | 雨的扰动幅度                   |
| rainSizeHi        | number                                                                            | 雨滴的最大直径                 |
| rainSizeLo        | number                                                                            | 雨滴的最小直径                 |
| rainSpeed         | number                                                                            | 雨的速度                       |
| snowColor         | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376) | 雪花颜色                       |
| snowDensity       | number                                                                            | 雪花密度                       |
| snowFallSpeed     | number                                                                            | 雪花速度                       |
| snowSizeHi        | number                                                                            | 雪花最大直径                   |
| snowSizeLo        | number                                                                            | 雪花最小直径                   |
| snowSpinSpeed     | number                                                                            | 雪花自旋速度                   |
| snowTexture       | string                                                                            | 雪花纹理                       |
| lightMode         | string                                                                            | 作用于天空和环境光的照明类型   |
| sunFrequency      | number                                                                            | 太阳运动的频率                 |
| sunDirection      | number                                                                            | 太阳光照明方向                 |
| sunLight          | number                                                                            | 太阳光颜色亮度                 |
| sunPhase          | number                                                                            | 太阳从升起至落下，在天空的位置 |
| lunarPhase        | number                                                                            | 月亮的相位                     |
| skyLeftLight      | number                                                                            | 环境光在-X轴方向的颜色亮度     |
| skyRightLight     | number                                                                            | 环境光在+X轴方向的颜色亮度     |
| skyBottomLight    | number                                                                            | 环境光在-Y轴方向的颜色亮度     |
| skyTopLight       | number                                                                            | 环境光在+Y轴方向的颜色亮度     |
| skyFrontLight     | number                                                                            | 环境光在+Z轴方向的颜色亮度     |
| skyBackLight      | number                                                                            | 环境光在-Z轴方向的颜色亮度     |

## GameZoneConfig 区域配置

接口 - GameZoneConfig
用于区域的参数

| 参数             | 类型                                                                                   | 说明                                                                                                       |
| ---------------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| bounds           | [GameBounds3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/zpmrz60ybosiiabb)        | 区域的所指定的检测区域                                                                                     |
| selector         | [GameSelectorString](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/twfeqqs5gfb8b6k9) | 触发区域事件的物体搜索条件                                                                                 |
| force            | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)        | 对物体施加的力的大小                                                                                       |
| massScale        | number                                                                                 | 控制物体的质量对力的影响程度。 0 = 像重力一样; 1 = 像风一样                                                |
| fogColor         | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 雾的颜色                                                                                                   |
| fogDensity       | number                                                                                 | 雾均匀密度                                                                                                 |
| fogEnabled       | boolean                                                                                | 雾是否开启                                                                                                 |
| fogHeightFalloff | number                                                                                 | 雾起始高度                                                                                                 |
| fogHeightOffset  | number                                                                                 | 雾衰减的速率                                                                                               |
| fogMax           | number                                                                                 | 最大雾量                                                                                                   |
| fogStartDistance | number                                                                                 | 雾起始距离                                                                                                 |
| rainColor        | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)      | 雨的颜色                                                                                                   |
| rainDensity      | number                                                                                 | 雨的密度。密度越大，雨滴越多。                                                                             |
| rainDirection    | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)        | 雨的方向                                                                                                   |
| rainEnabled      | boolean                                                                                | 雨是否开启                                                                                                 |
| rainInterference | number                                                                                 | 雨的扰动幅度                                                                                               |
| rainSizeHi       | number                                                                                 | 雨滴的最大直径                                                                                             |
| rainSizeLo       | number                                                                                 | 雨滴的最小直径                                                                                             |
| rainSpeed        | number                                                                                 | 雨的速度                                                                                                   |
| skyBackLight     | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在+Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                |
| skyBottomLight   | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在-Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                |
| skyEnabled       | boolean                                                                                | 环境参数是否有效                                                                                           |
| skyFrontLight    | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在-Z轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                |
| skyLeftLight     | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在-X轴方向的亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                    |
| skyLunarPhase    | number                                                                                 | 月亮的相位，数值在0和1之间。若大于0.5时，为上弦月。                                                        |
| skyMode          | "natural" or "manual"                                                                  | 作用于天空和环境光的照明类型。目前有提供2种光照模式，'manual'(自定义)或'natural'(动态)。默认为 'natural'。 |
| skyRightLight    | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在+X轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                |
| skySunDirection  | [GameVector3](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/lqqc61nd3gud9omc)        | 太阳光照明方向。仅在光照模式为manual自定义模式时生效。                                                     |
| skySunFrequency  | number                                                                                 | 太阳运动的频率，数值越大，昼夜交替越快。                                                                   |
| skySunLight      | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 太阳光颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                            |
| skySunPhase      | number                                                                                 | 太阳从升起至落下，在天空的位置。                                                                           |
| skyTopLight      | [GameRGBColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/kxqf3awgo7oc95eg)       | 环境光在+Y轴方向的颜色亮度。仅在光照模式为manual自定义模式时生效。颜色值大于0时，颜色越亮。                |
| snowColor        | [GameRGBAColor](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/he0l2ds1y29p5376)      | 雪花颜色                                                                                                   |
| snowDensity      | number                                                                                 | 雪的密度。密度越大，雪花越多。                                                                             |
| snowEnabled      | boolean                                                                                | 雪是否开启                                                                                                 |
| snowFallSpeed    | number                                                                                 | 雪花下落速度。如果小于0，则反向运动。                                                                      |
| snowSizeHi       | number                                                                                 | 雪花最大半径                                                                                               |
| snowSizeLo       | number                                                                                 | 雪花最小直径                                                                                               |
| snowSpinSpeed    | number                                                                                 | 雪花自旋速度                                                                                               |
| snowTexture      | string                                                                                 | 雪花纹理                                                                                                   |

默认值参考 [GameZone](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/puh5iyu2e8s1lar8)

```javascript
{

  selector: '',

    bounds: {

    lo: [0, 0, 0],

    hi: [0, 0, 0],

    },

  force: [0, 0, 0],

    massScale: 0,

    fogEnabled: false,

    fogColor: new GameRGBColor(1, 1, 1),

    fogDensity: 0,

    fogHeightFalloff: 0.8,

    fogHeightOffset: -8,

    fogMax: 1,

    fogStartDistance: 0,

    rainEnabled: false,

    rainColor: new GameRGBAColor(1, 1, 1, 1),

    rainDensity: 0,

    rainSpeed: 1,

    rainDirection: new GameVector3(0, 1, 0),

    rainInterference: 0,

    rainSizeHi: 1,

    rainSizeLo: 0,

    rainSpeed: 1,

    skyEnabled: false,

    skyMode: 'natural',

    skyBottomLight: new GameRGBColor(0, 0, 0),

    skyTopLight: new GameRGBColor(0, 0, 0),

    skyBackLight: new GameRGBColor(0, 0, 0),

    skyFrontLight: new GameRGBColor(0, 0, 0),

    skyLeftLight: new GameRGBColor(0, 0, 0),

    skyRightLight: new GameRGBColor(0, 0, 0),

    skySunDirection: new GameVector3(0, -1, 0),

    skyLunarPhase: 0,

    skySunFrequency: 0,

    skySunPhase: 0,

    skySunLight: new GameRGBColor(1000, 1000, 1000),

    snowEnabled: false,

    snowColor: new GameRGBAColor(1, 1, 1, 1),

    snowDensity: 0,

    snowTexture: '',

    snowFallSpeed: 1,

    snowSizeHi: 1,

    snowSizeLo: 0,

    snowSpinSpeed: 0,

    }
```

## MotionClipConfig 动作序列配置

类 - MotionClipConfig
动作序列配置

| 参数       | 类型    | 说明                                                                                         |
| ---------- | ------- | -------------------------------------------------------------------------------------------- |
| iterations | number  | 输入Infinity就是无限循环，此时会覆盖掉默认动作 能cancel或者播放新的动作覆盖可选项，默认 1 次 |
| motions    | (string | [MotionConfig](https://box3.yuque.com/org-wiki-box3-ev7rl4/wupvz3/grhrvh4gh1s1t7ni))[]          |

## MotionConfig 动作配置

接口 - MotionConfig

动作配置

| 参数       | 类型   | 说明                                                                                         |
| ---------- | ------ | -------------------------------------------------------------------------------------------- |
| iterations | number | 输入Infinity就是无限循环，此时会覆盖掉默认动作 能cancel或者播放新的动作覆盖可选项，默认 1 次 |
| name       | string | 动作名字                                                                                     |

## ReturnValue 数据查询返回

类型别名 - ReturnValue

描述
ReturnValue 表示一个键值对的内容。它可以是一个对象或者 undefined。

定义

定义

```javascript
export type ReturnValue =

  | {

    key: string;

    value: JSONValue;

    updateTime: number;

    createTime: number;

  }

  | undefined;
```

●key: string: 键名称
●value: JSONValue: 值内容
●updateTime: number: key最近更新时间
●createTime: number: key创建时间

# Enums-枚举

## GameAnimationDirection 动画播放方向

枚举 - GameAnimationDirection
动画的播放方向

| 属性              | 值                  | 说明     |
| ----------------- | ------------------- | -------- |
| ALTERNATE         | 'alternate'         | 交替     |
| ALTERNATE_REVERSE | 'alternate-reverse' | 交替倒放 |
| NORMAL            | 'normal'            | 普通     |
| REVERSE           | 'reverse'           | 倒放     |
| WRAP              | 'wrap'              | 循环     |
| WRAP_REVERSE      | 'wrap-reverse'      | 循环倒放 |

## GameAnimationPlaybackState 动画播放状态

枚举 - GameAnimationPlaybackState
动画播放状态

| 属性     | 值         | 说明     |
| -------- | ---------- | -------- |
| FINISHED | 'finished' | 已完成   |
| PENDING  | 'pending'  | 挂起等待 |
| RUNNING  | 'running'  | 播放中   |

## GameBodyPart 身体部位

枚举 - GameBodyPart
玩家身体部位的类型

| 属性            | 值              | 说明   |
| --------------- | --------------- | ------ |
| HIPS            | 'hips'          | 臀部   |
| TORSO           | 'torso'         | 躯干   |
| NECK            | 'neck'          | 颈部   |
| HEAD            | 'head'          | 头     |
| LEFT_SHOULDER   | 'leftShoulder'  | 左肩   |
| LEFT_UPPER_ARM  | 'leftUpperArm'  | 左上臂 |
| LEFT_LOWER_ARM  | 'leftLowerArm'  | 左下臂 |
| LEFT_HAND       | 'leftHand'      | 左手   |
| LEFT_UPPER_LEG  | 'leftUpperLeg'  | 左上腿 |
| LEFT_LOWER_LEG  | 'leftLowerLeg'  | 左下腿 |
| LEFT_FOOT       | 'leftFoot'      | 左脚   |
| RIGHT_SHOULDER  | 'rightShoulder' | 右肩膀 |
| RIGHT_UPPER_ARM | 'rightUpperArm' | 右上臂 |
| RIGHT_LOWER_ARM | 'rightLowerArm' | 右下臂 |
| RIGHT_HAND      | 'rightHand'     | 右手   |
| RIGHT_UPPER_LEG | 'rightUpperLeg' | 右上腿 |
| RIGHT_LOWER_LEG | 'rightLowerLeg' | 右下腿 |
| RIGHT_FOOT      | 'rightFoot'     | 右脚   |

## GameButtonType - 按钮类型

枚举 - GameButtonType
玩家按下的按钮类型

| 属性        | 值        | 说明                 |
| ----------- | --------- | -------------------- |
| WALK        | 'walk'    | 步行按钮             |
| RUN         | 'run'     | 奔跑按钮             |
| CROUCH      | 'crouch'  | 下蹲按钮             |
| JUMP        | 'jump'    | 跳跃按钮             |
| DOUBLE_JUMP | 'jump2    | 二段跳按钮           |
| FLY         | 'fly'     | 飞行按钮             |
| ACTION0     | 'action0' | 鼠标左键 / 虚拟按钮A |
| ACTION1     | 'action1' | 鼠标右键 / 虚拟按钮B |

## GameCameraMode 视角模式

枚举 - GameCameraMode
玩家的相机视角模式

| 属性   | 值       | 说明                   |
| ------ | -------- | ---------------------- |
| FIXED  | 'fixed'  | 第三人称固定视角       |
| FOLLOW | 'follow' | 第三人称跟随视角(默认) |
| FPS    | 'fps'    | 第一人称视角           |

## GameDialogType 对话框类型

枚举 - GameDialogType
对话框样式类型

| 属性   | 值       | 说明           |
| ------ | -------- | -------------- |
| TEXT   | 'text'   | 文本样式对话框 |
| INPUT  | 'input'  | 输入样式对话框 |
| SELECT | 'select' | 选择样式对话框 |

## GameEasing 缓动效果

枚举 - GameEasing
动画的缓动效果，EaseIn缓入，EaseOut缓出

| 属性      | 值          | 说明   |
| --------- | ----------- | ------ |
| BACK      | 'back'      | 反向   |
| BOUNCE    | 'bounce'    | 弹性   |
| CIRCLE    | 'circle'    | 圆     |
| ELASTIC   | 'elastic'   | 橡皮筋 |
| EXP       | 'exp'       | 指数   |
| LINEAR    | 'linear'    | 线性   |
| NONE      | 'none'      | 无     |
| QUADRATIC | 'quadratic' | 二次方 |
| SINE      | 'sine'      | 正弦波 |

## GameInputDirection 玩家输入方向

枚举 - GameInputDirection
玩家通过输入设备控制移动时的方向，可用于 [GamePlayer.disableInputDirection](https://box3.yuque.com/staff-khn556/wupvz3/ddctd6h29w3myth0#aahNx) 禁用对应方向的输入，以控制玩家移动的表现。

| 属性       | 值           | 说明           |
| ---------- | ------------ | -------------- |
| NONE       | 'none'       | 无，代表不禁用 |
| VERTICAL   | 'vertical'   | 垂直方向       |
| HORIZONTAL | 'horizontal' | 水平方向       |
| BOTH       | 'both'       | 所有方向       |

## GamePlayerMoveState 玩家运动状态

PlayerMoveState运动状态
玩家的运动状态

| 属性        | 值       | 说明     |
| ----------- | -------- | -------- |
| FLYING      | 'fly'    | 飞行中   |
| GROUND      | 'ground' | 在地上   |
| SWIM        | 'swim'   | 游泳中   |
| FALL        | 'fall'   | 下落中   |
| JUMP        | 'jump'   | 跳跃中   |
| DOUBLE_JUMP | 'jump2'  | 二段跳中 |

## GamePlayerWalkState 玩家行走状态

枚举 - GamePlayerWalkState
玩家的行走状态

| 属性   | 值       | 说明     |
| ------ | -------- | -------- |
| NONE   | ''       | 非行走中 |
| CROUCH | 'crouch' | 下蹲行走 |
| WALK   | 'walk'   | 正常步行 |
| RUN    | 'run'    | 奔跑     |

## SocialType 玩家社交关系

枚举 - SocialType交关系类型，用于在 [GamePlayer 玩家](https://box3.yuque.com/staff-khn556/wupvz3/ddctd6h29w3myth0#V8jWi)

 中查询玩家的社交关系。

| 属性      | 值 | 说明 |
| --------- | -- | ---- |
| FOLLOWING | 0  | 关注 |
| FOLLOWERS | 1  | 粉丝 |
| FRIENDS   | 2  | 好友 |

# 高级功能

## 代码速建

### 文档说明

本文档中的代码，如果出现“-snip-”表示省略了上文中重复的代码

### 建筑代码

#### 岛三的建筑代码

voxels.setVoxel()可以指定最多5个参数：X, Y, Z, voxel, rotation

##### 限制

参数X, Y, Z必须是string；voxel, rotation可以是string或者number类型

```javascript
voxels.setVoxel(X, Y, Z, voxel, rotation)
/*
(x: number, y: number, Z: number, voxel: string | number, rotation?: string | number) : number
*/
```

#### 举例

如 `voxels.setVoxel(1, 1, 1, 'grass', 0)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为0即方块旋转0*90=0度

如 `voxels.setVoxel(1, 1, 1, 'grass', 1)`，可以在x、y、z为1的位置放置一个草方块，旋转（rotation）为1即将方块逆时针旋转1*90=90度

又如 `voxels.setVoxel(1, 2, 3, 'stone', 2)`，可以在x=1,y=2,z=3的位置放置一个石头，因为旋转（rotation）的值为2，所以会将原始的方块逆时针旋转2*90=180度

`voxels.setVoxel(12, 3, 45, 'glass', 3)`，在x=12,y=3,z=45的位置放置一个玻璃方块，逆时针旋转3*90=270度

`voxels.setVoxel(12, 3, 45, 'dirt', 4)`，在x=12,y=3,z=45的位置放置一个土方块，逆时针旋转了4*90=360度，所以相当于不旋转，作用效果等于 `voxels.setVoxel(12, 3, 45, 'dirt', 0)`

说明：rotation值可以不加，默认为0

#### 返回值

##### 方块存在时

如果传入的方块存在，使用此方法的返回值会返回第四个参数即voxel对应的方块ID

例如 `voxels.setVoxel(1, 2, 3, 'stone')`会返回名为“stone”的方块对应的id

##### 方块不存在时

如果方块不存在，会返回0

例如 `voxels.setVoxel(1, 2, 3, 'this_is_not_a_block_name')`会返回0

### 快速建造

快速建造可以更高效地批量化建筑方块

#### 建造一个长方体

```javascript
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}
```

##### 举例

```javascript
// 定义函数
/**
 * 快速建造一个长方体
 * 
 * @param {number | string} voxel - 方块名称或者id
 * @param {number} xmin - x的最小值
 * @param {number} ymin - y的最小值
 * @param {number} zmin - z的最小值
 * @param {number} xmax - x的最大值
 * @param {number} ymax - y的最大值
 * @param {number} zmax - z的最大值
 * @param {number | string} rotation - 方块旋转
*/
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	for(let x=xmin;x<=xmax;x++){
		for(let y=ymin;y<=ymax;y++){
			for(let z=zmin;z<=zmax;z++){
				voxels.setVoxel(x, y, z, voxel, rotation)
			}
		}
	}
}

// 调用函数
// 调用快速建造函数用“grass”（草方块）建造一个起于{x=1,y=1,z=1}，止于{x=100,y=64,z=101}，所有方块都旋转3*90=270度的长方体
quick_build('grass', 1, 1, 1, 100, 64, 101, 3)
// 调用快速建造函数用“stone”（草方块）建造一个起于{x=2,y=3,z=4}，止于{x=100,y=64,z=101}，此时不传入参数rotation，方块默认不旋转
quick_build('stone', 2, 3, 4, 100, 64, 101, 3)
```

##### 解决分不清x,y,z的最大值和最小值的问题

有时候并不知道xmin,ymin,zmin,xmax,ymax,zmax到底该传入什么值，以下两种方法可以解决：

###### 如果已经知道定值，可以自行判断

例如：

```javascript
var pos1 = new GameVector3(1,1,1)
var pos2 = new GameVector3(5,5,5)
```

因为pos1的x、y、z值都小于pos2的x、y、z值，所以此时应如此传入：

```javascript
quick_build('方块名', pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos3.z)
```

###### 如果两坐标完全随机，可以使用函数判断

```javascript
function quick_build(voxel, xmin, ymin, zmin, xmax, ymax, zmax, rotation=0){
	-snip-
}
function quick_build_pro(voxel, pos1, pos2, rotation=0){
	// 判断pos1和pos2的位置关系并正确传入
	if(pos1.x<=pos2.x&&pos1.y<=pos2.y&&pos1.z<=pos2.z){ // 当pos1的xyz坐标均小于等于pos2的xyz坐标时的调用方式
		quick_build(voxel, pos1.x, pos1.y, pos1.z, pos2.x, pos2.y, pos2.z, rotation)
	}
	else if(pos1.x>pos2.x&&pos1.y>pos2.y&&pos1.z>pos2.z){ // 当pos2的xyz坐标均小于pos1的xyz坐标时的调用方式
		quick_build(voxel, pos2.x, pos2.y, pos2.z, pos1.x, pos1.y, pos1.z, rotation)
	}
	else{ // 否则输出错误
		console.error('不支持的判断类型')
	}
}
```

#### 以某一位置为中心建造球体

```javascript
/**
 * 快速建造一个球体
 * 
 * @param {GameVector3} centerPos - 球体中心位置
 * @param {number | string} voxel - 方块id或名称
 * @param {number} r - 球体半径
 * @param {number | string} rotation - 方块旋转
*/
function ball(centerPos, r, voxel, rotation=0){
	// 创建嵌套循环，这样创建的妙处在于不必遍历地图每个方块，如果遍历地图每个方块的话地图会崩溃
	for(let x=centerPos.x-r;x<=centerPos.x+r;x++){
		for(let y=centerPos.y-r;y<=centerPos.y+r;y++){
		for(let z=centerPos.z-r;z<=centerPos.z+r;z++){
        	const position2 = new GameVector3(x, y, z);

                // 计算两个位置之间的距离
                const distance1 = Math.sqrt(Math.pow(position2.x - centerPos.x, 2) + Math.pow(position2.y - centerPos.y, 2) + Math.pow(position2.z - centerPos.z, 2));
          	if(distance1<=r){// 如果距离小于传入的r的值，则放置方块
                     	voxels.setVoxel(x,y,z,voxel,rotation)
            	}
                }
            	}
     	}
}
```

##### 限制

因为神奇代码岛的服务器能力问题，当r过大时可能会导致服务器崩溃，所以不要传入一个较大的值

##### 举例

```javascript
function ball(centerPos, r, voxel, rotation=0){
	-snip-
}

var center = new GameVector3(50, 50, 50)
ball(center, 10, 'dirt', 2) // 以{x=50,y=50,z=50}为球体中心、填充旋转了2*90=180度的“dirt”（草方块），半径为10，快速建造一个球体
```

#### 在某一位置创建底面为l，高为l的三棱锥

```javascript
function pyramid(l, pos, voxel, rotation){
	let cx = pos.x;
	let cy = pos.y;
	let cz = pos.z;
	let height = l;
	let xend = cx + l;
	let zend = cz + l;
	for(let y = cy; y < cy + height; y++){
	  	let ylevel = y - cy;
	  	let xstart = cx + ylevel;
	  	let xend = cx + l - ylevel;
	  	let zstart = cz + ylevel;
	  	let zend = cz + l - ylevel;
	  	for(let x = xstart; x < xend; x++){
	    	for(let z = zstart; z < zend; z++){
	      		voxels.setVoxel(x, y, z, voxel, rotation);
	    	}
	  	}
	}
}
```

##### 举例

```javascript
function pyramid(l, pos, voxel, rotation){
	-snip-
}
var pos = new GameVector3(60,10,60)
pyramid(5, pos, 'stone', 3); // 在{x:60,y:10,z:60}使用“stone”（石头）建造一个底面为5*5，高度为5的三棱锥，所有方块逆时针旋转3*90=270度
```
