
- 这是什么 : 美化后的 Aplayer css 和 js 配置文件

- 如何使用 : 参考 [Aplayer 文档](https://aplayer.js.org/#/home)

- 推荐使用 cssv3 和 jsv2 两份文件 ( Aplayer.min.css 和 Aplayer.min.js 也行, 但是旧一点)

- 推荐使用 CDN 加速后的远程 js / css, 链接 :
    - https://jsd.onmicrosoft.cn/gh/Daleveral/csslivb/cssv3.css
      
    - https://jsd.onmicrosoft.cn/gh/Daleveral/csslivb/jsv2.js

- 美化前后对比 :

  <br/>

![配置前](https://wkphoto.cdn.bcebos.com/aa64034f78f0f7360be03a6a1a55b319ebc413ba.jpg)

<br/>

![配置后](https://wkphoto.cdn.bcebos.com/3c6d55fbb2fb4316889d0d1130a4462308f7d3df.jpg)



<br/>

- 现在简单的将播放器分为两块, 如上图所示, 一是底下的长栏 : 显示当前播放的歌曲即歌手名, 进度条, 控制按钮等; 二是展开后上面的歌单: 序号, 歌名, 歌手名等.

- 两份配置文件为 Aplayer.min.css ( 或 cssv3.css ) 和 Aplayer.min.js ( 或 jsv2.js ) 

- 下面我给出了两个无序列表 ( 当然配置文件的最前面的注释里也有 ) , 你想更改哪里的配置就将对应的黑色实心小圆点后的文字复制后在  Aplayer.min.css  中搜索 ( 只有两处会涉及 js 文件有特别提醒 ), 然后你就能找到我埋在那里的定位注释了 ( 比如用 VS Code, 搜索指定文字的快捷键是 Ctrl F, 如果我想要更改 “歌单背景颜色”, 那么只需要选定这几个字按 Ctrl F, 即可找到对应的位置了 )

 -  觉得不错可以给个 **star** 谢谢 ~

___

<br/>

对于底部栏, 修改哪个即搜索哪个词条即能定位, 词条后的括号里为注释, 搜索时请忽略 :
- 底部栏歌曲名
- 底部栏歌手名
- 控制按钮颜色 (上/下一首, 暂停/播放, 歌单展开/折叠等)
- 时间颜色 ( 如 00:26/03:11 )
- 最右侧展开/折叠按钮 ( 负责底部栏横向的折叠与展开 )
- 音乐进度条 ( 这里会涉及 js 文件 )
- 播放器位置
 
<br/>

对于歌单 ( 歌单的高度并不在 css 或 js 中, 需要你在创建 Aplayer 对象时自定义参数 listMaxHeight, 如 listMaxHeight: '458px' ) :
- 歌单背景颜色
- 歌单中的序号
- 歌单中的歌曲名
- 歌单中的歌手名
- 当前鼠标在歌单中位置 ( 所在一行的背景色 )
- 当前正在播放的歌曲在歌单中位置 ( 所在一行的背景色 )
- 歌单内歌曲之间的分割线
- 歌单最外面的边框线
- 滚动栏颜色
- 滚动栏背景色

<br/>

___

- 也可以在我的博客中阅读此文档 :

- 帖子 : https://www.dalechu.cn/article/aplayer

- 备用地址 : https://www.epicurus.fun/article/aplayer
