
<!DOCTYPE html>
<html>

  <head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

  <title>OneV&#39;s Den</title>
  <meta name="description" content="嗨，我是王巍 (@onevcat)，一名 iOS 开发者。">
  <meta name="author" content="Wei Wang">

  <meta name="twitter:card" content="summary">
  <meta name="twitter:title" content="OneV&#39;s Den">
  <meta name="twitter:description" content="嗨，我是王巍 (@onevcat)，一名 iOS 开发者。">
  
  <meta property="og:type" content="article">
  <meta property="og:title" content="OneV&#39;s Den">
  <meta property="og:description" content="嗨，我是王巍 (@onevcat)，一名 iOS 开发者。">
  
  <link rel="icon" type="image/png" href="/assets/images/favicon.png" />
  <link href="/assets/images/favicon.png" rel="shortcut icon" type="image/png">
  
  <link rel="stylesheet" href="/css/main.css">
  <link href="//netdna.bootstrapcdn.com/font-awesome/4.1.0/css/font-awesome.min.css" rel="stylesheet">

  <link rel="canonical" href="https://onevcat.com/">
  <link rel="alternate" type="application/rss+xml" title="OneV's Den" href="https://onevcat.com/feed.xml">
  
  <meta name="google-site-verification" content="1-1ZlHoRvM0T2FqPbW2S-qLgYXN6rsn52kErlMPd_gw" />
  
</head>


  <body>

    <span class="mobile btn-mobile-menu">
        <i class="fa fa-list btn-mobile-menu__icon"></i>
        <i class="fa fa-angle-up btn-mobile-close__icon hidden"></i>
    </span>
    
    <header class="panel-cover " style="background-image: url('/assets/images/background-cover.jpg')">
  <div class="panel-main">

    <div class="panel-main__inner panel-inverted">
    <div class="panel-main__content">

        <a href="/#blog" title="前往 OneV's Den 的主页" class="blog-button"><img src="/assets/images/avatar.jpg" width="80" alt="OneV's Den logo" class="panel-cover__logo logo" /></a>
        <h1 class="panel-cover__title panel-title"><a href="/#blog" title="link to homepage for OneV's Den" class="blog-button">OneV's Den</a></h1>

        
        <span class="panel-cover__subtitle panel-subtitle">上善若水，人淡如菊</span>
        
        <hr class="panel-cover__divider" />
        <p class="panel-cover__description">嗨，我是王巍 (@onevcat)，一名 iOS 开发者。</p>
        <hr class="panel-cover__divider panel-cover__divider--secondary" />
        
        
        <p class="panel-cover__description"><a href="https://objccn.io/products/">我组织的 ObjC 中国与 objc.io 合作发布了一系列 iOS/Swift 相关图书，欢迎访问了解更多</a></p>
        
        
        <div class="navigation-wrapper">
          <div>
            <nav class="cover-navigation cover-navigation--primary">
              <ul class="navigation">
                <li class="navigation__item"><a href="/#blog" title="访问博客" class="blog-button">博客</a></li>
                
                  <li class="navigation__item"><a href="//onev.cat" target="_blank" title="我的简历">简历</a></li>
                
                  <li class="navigation__item"><a href="/apps" target="_blank" title="我所使用的 app 们">工具</a></li>
                
                  <li class="navigation__item"><a href="//objccn.io/subscribe" target="_blank" title="邮件订阅本站">订阅</a></li>
                
              </ul>
            </nav>
          </div>
          
          <div><nav class="cover-navigation navigation--social">
  <ul class="navigation">

  
  <!-- Weibo -->
  <li class="navigation__item">
    <a href="http://weibo.com/onevcat" title="@onevcat 的微博" target="_blank">
      <i class='social fa fa-weibo'></i>
      <span class="label">Weibo</span>
    </a>
  </li>
  

  
  <!-- Github -->
  <li class="navigation__item">
    <a href="https://github.com/onevcat" title="@onevcat 的 Github" target="_blank">
      <i class='social fa fa-github'></i>
      <span class="label">Github</span>
    </a>
  </li>
  
  
  
  <!-- Twitter -->
  <li class="navigation__item">
    <a href="http://twitter.com/onevcat" title="@onevcat" target="_blank">
      <i class='social fa fa-twitter'></i>
      <span class="label">Twitter</span>
    </a>
  </li>
  

  
  <!-- Google Plus -->
  <li class="navigation__item">
    <a href="https://plus.google.com/107108267983477358170" rel="author" title="Google+" target="_blank">
      <i class='social fa fa-google-plus-square'></i>
      <span class="label">Google Plus</span>
    </a>
  </li>
  

  <!-- RSS -->
  <li class="navigation__item">
    <a href="/feed.xml" rel="author" title="RSS" target="_blank">
      <i class='social fa fa-rss'></i>
      <span class="label">RSS</span>
    </a>
  </li>

  
  <!-- Email -->
  <li class="navigation__item">
    <a href="mailto:onev@onevcat.com" title="Contact me">
      <i class='social fa fa-envelope'></i>
      <span class="label">Email</span>
    </a>
  </li>
  

  </ul>
</nav>
</div>
        </div>
      </div>
    </div>
    
    
    <div class="panel-cover--overlay cover-disabled"></div>
    
  </div>
</header>


    <div class="content-wrapper">
        <div class="content-wrapper__inner">
            <div class="main-post-list hidden">

  <ol class="post-list">
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/11/defer/" title="访问 关于 Swift defer 的正确使用">关于 Swift defer 的正确使用</a></h2>
      <p class="excerpt">其实这篇文章的缘起是由于在对 Kingfisher 做重构的时候，因为自己对 defer 的理解不够准确，导致了一个 bug。所以想藉由这篇文章探索一下 defer 这个关键字的一些 edge case。典型用法Swift 里的 defer 大家应该都很熟悉了，defer 所声明的 block 会在当前代码执行退出后被调用。正因为它提供了一种延时调用的方式，所以一般会被用来做资源释放或者销毁，这在某个函数有多个返回出口的时候特别有用。比如下面的通过 FileHandle 打开文件进行操作的...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-11-16 10:38:00 +0900" class="post-list__meta--date date">2018-11-16</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2018/11/defer/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/10/swift-result-error/" title="访问 Result&lt;T&gt; 还是 Result&lt;T, E: Error&gt;">Result&lt;T&gt; 还是 Result&lt;T, E: Error&gt;</a></h2>
      <p class="excerpt">  我之前在专栏文章里曾经发布这篇文章，由于这个话题其实还是挺重要的，可以说代表了 Swift 今后发展的方向流派，所以即使和专栏文章内容有些重复，我还是想把它再贴到博客来。经过半年以后，自己对于这个问题也有了更多的实践和想法，所以同时也更新了一下。我没有直接改动原文，而是把新的想法和需要补充的说明，用类似这段话的引用的方式写在合适的上下文里。开始先打个广告我个人经常会在数码荔枝用优惠价格购买面向中国用户的一些软件，相比于花美金直接购买，价格非常实惠。近年来国内的正版风气和对知识知识产权的...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-10-31 11:38:00 +0900" class="post-list__meta--date date">2018-10-31</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2018/10/swift-result-error/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/10/diary/" title="访问 十年前的日记们">十年前的日记们</a></h2>
      <p class="excerpt">假如我有时光机最近把工作上的事情忙完了，也把主机从美国换到了日本的机房，解决了国内的访问问题，所以准备开始好好重新拾掇一下，恢复定期更新 blog。其实我从大学时就有开始写 blog 的习惯了。不过不像最近的独立博客，那时候更多地是用新浪或者搜狐这样的平台，所以也就在那些地方也留下了不少“足迹”。既然是自己“存在过的证明”，我想可能还是把它们汇总一下，留个存档为好。于是就有了这篇和“技术”没什么关系的文章。这里面是我从 2006 年底到 2010 年三月期间的一些碎碎念，时间跨越从大二上半...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-10-23 10:11:26 +0900" class="post-list__meta--date date">2018-10-23</time> &#8226; <span class="post-list__meta--tags tags">胡言乱语集</span><a class="btn-border-small" href=/2018/10/diary/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/06/wwdc-2018/" title="访问 开发者所需要知道的 WWDC 2018 新特性">开发者所需要知道的 WWDC 2018 新特性</a></h2>
      <p class="excerpt">一直阅读我的博客的朋友可能知道，我在每年 WWDC 之后都会写 (水) 一篇关于新 SDK 和开发工具的文章。之前这个系列叫做《开发者所需要知道的 iOS SDK 新特性》，但是最近虽然 Craig 嘴上说着不要，身体却很诚实地将 iOS 和 macOS 带到一起，所以今年我觉得可以改一改题目，就总览一下作为 Apple 生态圈的开发者，在今年 WWDC 上我个人的一些观察，以及可能应该注意的有趣的地方。在会前，Apple 就已经放出消息要放慢增加新功能的脚步，转而提升软件稳定性和可靠性。...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-06-05 12:15:00 +0900" class="post-list__meta--date date">2018-06-05</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2018/06/wwdc-2018/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/05/mvc-wrong-use/" title="访问 关于 MVC 的一个常见的误用">关于 MVC 的一个常见的误用</a></h2>
      <p class="excerpt">  写在前面：ObjC 中国 (或者说我个人) 现在正和 objc.io 合作打造一本关于 app 架构的书籍。英文版本已经提前预售，书本身也进入了最后的 review 阶段。我们也将在第一时间进行本书中文版的工作，还请大家关注。  本文的内容也是有关 app 架构的一些思考，如果你对架构方面的话题有兴趣的话，我之前还写过一篇利用 reducer 的单向数据流动的函数式 View Controller 的文章可供参考。如何避免把 Model View Controller 写成 Massi...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-05-11 09:15:00 +0900" class="post-list__meta--date date">2018-05-11</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2018/05/mvc-wrong-use/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2018/03/swift-meta/" title="访问 不同角度看问题 - 从 Codable 到 Swift 元编程">不同角度看问题 - 从 Codable 到 Swift 元编程</a></h2>
      <p class="excerpt">  最近开设了一个小专栏，用来记录日常开发时遇到的问题和解决方案，同时也会收藏一些学习时记录的笔记，随想等。其中一些长文 (包括本文) 会首发于专栏，之后再同步到博客这边。虽然现在的文章还不多，但是因为计划更新比较勤快，所以适当进行收费，也算是对自己写作的一种鼓励和鞭笞。欢迎感兴趣的同学进行订阅，谢谢~起源前几天看到同事的一个 P-R，里面有将一个类型转换为字典的方法。在我们所使用的 API 中，某些方法需要接受 JSON 兼容的字典 (也就是说，字典中键值对的 value 只能是数字，字...&hellip;</p>
      <div class="post-list__meta"><time datetime="2018-03-12 09:15:00 +0900" class="post-list__meta--date date">2018-03-12</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2018/03/swift-meta/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/10/swift-error-category/" title="访问 关于 Swift Error 的分类">关于 Swift Error 的分类</a></h2>
      <p class="excerpt">在去年我应 IBM 编辑的邀请写过一篇关于 Swift 2 中 throws 的文章。现在回头看，Swift 2 其实是 Swift 语言发展的一个挺重要的节点：如果说 Swift 1 是一个更偏向于验证阶段的产品的话，Swift 2 中加入的特性为这门语言的基石进行了补足。在那篇文章里我们主要深入探索了新的 throw 关键字背后的事情，而同一时期其实 Swift 官方有过一次关于错误处理的讨论。随着 Swift 3 的开源，这些原始文档也被一同公开，展示了 Swift 设计的过程和轨迹...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-10-17 12:15:00 +0900" class="post-list__meta--date date">2017-10-17</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2017/10/swift-error-category/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/07/state-based-viewcontroller/" title="访问 单向数据流动的函数式 View Controller">单向数据流动的函数式 View Controller</a></h2>
      <p class="excerpt">View Controller 向来是 MVC (Model-View-View Controller) 中最让人头疼的一环，MVC 架构本身并不复杂，但开发者很容易将大量代码扔到用于协调 View 和 Model 的 Controller 中。你不能说这是一种错误，因为 View Controller 所承担的本来就是胶水代码和业务逻辑的部分。但是，持续这样做必定将导致 Model View Controller 变成 Massive View Controller，代码也就一天天烂下去...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-07-13 10:05:00 +0900" class="post-list__meta--date date">2017-07-13</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2017/07/state-based-viewcontroller/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/06/ios-11-sdk/" title="访问 开发者所需要知道的 iOS 11 SDK 新特性">开发者所需要知道的 iOS 11 SDK 新特性</a></h2>
      <p class="excerpt">年纪大了过了能熬夜看 WWDC 的时代了，但是还是在小小宝的哭闹和妈妈大人换尿布的催促中起了个大早。于是算趁着“热乎”把 WWDC 2017 的 Keynote 看完了。和往年差不多，虽然 WWDC 是一个开发者会议，但是 Keynote 并不是专门针对我们开发者的，它还承担了公司状况说明，新品发布等功能。作为技术人员，可能接下来的 session 会更有意义。要用一句话来评价今年 Keynote 所展现出来的内容的话，就是小步革新。大的技术方面可以说只有 ARKit 可堪研究，但是我们还...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-06-06 12:15:00 +0900" class="post-list__meta--date date">2017-06-06</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2017/06/ios-11-sdk/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/04/storyboard-argue/" title="访问 再看关于 Storyboard 的一些争论">再看关于 Storyboard 的一些争论</a></h2>
      <p class="excerpt">从 iOS 5 的时代 Apple 推出 Storyboard (以下简称 SB) 后，关于使用这种方式构建 UI 的争论就在 Cocoa 开发者社区里一直发生着。我在 2013 年写过一篇关于代码手写 UI，xib 和 SB 之间的取舍的文章。在四五年后的今天，SB 得到了多次进化，大家也积攒了很多关于使用 SB 进行开发的经验，我们不妨再回头看看当初的忧虑，并结合 SB 开发的现状，来提取一些现阶段被认为比较好的实践。这篇文章缘起为对使用 SB 的方式一文 (及其英文原文) 的回应，我...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-04-27 10:45:00 +0900" class="post-list__meta--date date">2017-04-27</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2017/04/storyboard-argue/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/02/ownership/" title="访问 所有权宣言 - Swift 官方文章 Ownership Manifesto 译文评注版">所有权宣言 - Swift 官方文章 Ownership Manifesto 译文评注版</a></h2>
      <p class="excerpt">Swift 团队最近在邮件列表里向社区发了一封邮件，讲述了关于内存所有权方面的一些未来的改变方向。作为上层 API 的使用者来说，我们可能并不需要了解背后所有的事实，但是 Apple 的这封邮件中对 Swift 的值和对象的内存管理进行了很全面的表述，一步步说明了前因后果。如果你想深入学习和了解 Swift 的话，这篇文章是非常棒的参考资料。我尝试翻译了一下全文，并且加上了一些自己的注解。虽然这篇文章比较长，但是如果你想要进阶 Swift 的话，不妨花时间通读全文 (甚至通读全文若干遍)。...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-02-27 15:40:00 +0900" class="post-list__meta--date date">2017-02-27</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2017/02/ownership/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2017/02/mailme-app/" title="访问 使用邮件来进行信息管理，顺便介绍最近写的一个小 app - Mail Me">使用邮件来进行信息管理，顺便介绍最近写的一个小 app - Mail Me</a></h2>
      <p class="excerpt">距离上一次自己在 App Store 发布个人 app 已经过去了两年多了。这段时间里把精力主要都放在了公司项目和继续进一步的学习中，倒也在日常工作和出书等方面取得了一些进展。个人 app 这块近两年虽然有写一些便捷的效率类应用，但是几次审核都被 Apple 无情拒掉以后，也就安心弄成自用的小工具了。看着自己逐渐发霉的开发者证书，果然觉得还是找时间倒腾点什么比较好。于是就有了现在想要介绍给大家的这个工具，Mail Me - 一个可以帮助你快速给自己发送邮件的小 app。基于邮件的信息管理方...&hellip;</p>
      <div class="post-list__meta"><time datetime="2017-02-22 10:05:00 +0900" class="post-list__meta--date date">2017-02-22</time> &#8226; <span class="post-list__meta--tags tags">胡言乱语集</span><a class="btn-border-small" href=/2017/02/mailme-app/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/12/concurrency/" title="访问 Swift 并行编程现状和展望 - async/await 和参与者模式">Swift 并行编程现状和展望 - async/await 和参与者模式</a></h2>
      <p class="excerpt">  这篇文章不是针对当前版本 Swift 3 的，而是对预计于 2018 年发布的 Swift 5 的一些特性的猜想。如果两年后我还记得这篇文章，可能会回来更新一波。在此之前，请当作一篇对现代语言并行编程特性的不太严谨科普文来看待。CPU 速度已经很多年没有大的突破了，硬件行业更多地将重点放在多核心技术上，而与之对应，软件中并行编程的概念也越来越重要。如何利用多核心 CPU，以及拥有密集计算单元的 GPU，来进行快速的处理和计算，是很多开发者十分感兴趣的事情。在今年年初 Swift 4 的...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-12-20 12:53:11 +0900" class="post-list__meta--date date">2016-12-20</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/12/concurrency/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/12/pop-cocoa-2/" title="访问 面向协议编程与 Cocoa 的邂逅 (下)">面向协议编程与 Cocoa 的邂逅 (下)</a></h2>
      <p class="excerpt">本文是笔者在 MDCC 16 (移动开发者大会) 上 iOS 专场中的主题演讲的文字整理。您可以在这里找到演讲使用的 Keynote，部分示例代码可以在 MDCC 2016 的官方 repo 中找到。在上半部分主要介绍了一些理论方面的内容，包括面向对象编程存在的问题，面向协议的基本概念和决策模型等。本文 (下) 主要展示了一些笔者日常使用面向协议思想和 Cocoa 开发结合的示例代码，并对其进行了一些解说。转・热恋 - 在日常开发中使用协议WWDC 2015 在 POP 方面有一个非常优秀...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-12-01 11:22:11 +0900" class="post-list__meta--date date">2016-12-01</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/12/pop-cocoa-2/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/11/pop-cocoa-1/" title="访问 面向协议编程与 Cocoa 的邂逅 (上)">面向协议编程与 Cocoa 的邂逅 (上)</a></h2>
      <p class="excerpt">本文是笔者在 MDCC 16 (移动开发者大会) 上 iOS 专场中的主题演讲的文字整理。您可以在这里找到演讲使用的 Keynote，部分示例代码可以在 MDCC 2016 的官方 repo 中找到。因为全部内容比较长，所以分成了上下两个部分，本文 (上) 主要介绍了一些理论方面的内容，包括面向对象编程存在的问题，面向协议的基本概念和决策模型等，下半部分主要展示了一些笔者日常使用面向协议思想和 Cocoa 开发结合的示例代码，并对其进行了一些解说。引子面向协议编程 (Protocol Or...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-11-29 10:22:11 +0900" class="post-list__meta--date date">2016-11-29</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/11/pop-cocoa-1/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/08/notification/" title="访问 活久见的重构 - iOS 10 UserNotifications 框架解析">活久见的重构 - iOS 10 UserNotifications 框架解析</a></h2>
      <p class="excerpt">TL;DRiOS 10 中以前杂乱的和通知相关的 API 都被统一了，现在开发者可以使用独立的 UserNotifications.framework 来集中管理和使用 iOS 系统中通知的功能。在此基础上，Apple 还增加了撤回单条通知，更新已展示通知，中途修改通知内容，在通知中展示图片视频，自定义通知 UI 等一系列新功能，非常强大。对于开发者来说，相较于之前版本，iOS 10 提供了一套非常易用的通知处理接口，是 SDK 的一次重大重构。而之前的绝大部分通知相关 API 都已经被标...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-08-08 10:22:11 +0900" class="post-list__meta--date date">2016-08-08</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/08/notification/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/06/ios-10-ats/" title="访问 关于 iOS 10 中 ATS 的问题">关于 iOS 10 中 ATS 的问题</a></h2>
      <p class="excerpt">  本文于 2016 年 11 月 28 日按照 Apple 最新的文档和 Xcode 8 中的表现进行了部分更新。WWDC 15 提出的 ATS (App Transport Security) 是 Apple 在推进网络通讯安全的一个重要方式。在 iOS 9 和 OS X 10.11 中，默认情况下非 HTTPS 的网络访问是被禁止的。当然，因为这样的推进影响面非常广，作为缓冲，我们可以在 Info.plist 中添加 NSAppTransportSecurity 字典并且将 NSAl...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-06-17 13:34:11 +0900" class="post-list__meta--date date">2016-06-17</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/06/ios-10-ats/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/06/ios-10-sdk/" title="访问 开发者所需要知道的 iOS 10 SDK 新特性">开发者所需要知道的 iOS 10 SDK 新特性</a></h2>
      <p class="excerpt">总览距离 iPhone 横空出世已经过去了 9 个年头，iOS 的版本号也跨入了两位数。在我们回顾过去四五年 iOS 系统的发展的时候，不免感叹变化速度之快，迭代周期之短。iOS 7 翻天覆地的全新设计，iOS 8 中 Size Classes 的出现，应用扩展，以及 Cloud Kit 的加入，iOS 9 里的分屏多任务特性等等。Apple 近年都是在 WWDC 发布新的系统和软件，然后在秋季和冬季 (或者来年春季) 召开硬件产品的发布会。WWDC 上每一项软件的更新其实都预示了相应的硬...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-06-15 15:10:11 +0900" class="post-list__meta--date date">2016-06-15</time> &#8226; <span class="post-list__meta--tags tags">能工巧匠集</span><a class="btn-border-small" href=/2016/06/ios-10-sdk/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/04/first-wwdc/" title="访问 写给初次参加 WWDC 的开发者的简明攻略">写给初次参加 WWDC 的开发者的简明攻略</a></h2>
      <p class="excerpt">今天 Apple 宣布了 WWDC 16 的抽选开始，而 4 月 22 日周五将出抽选结果并开始购票。随着我们国内开发者收入水平的逐步提升，以及日益增长的与全球开发者接触和自我提高的需求，最近参与 WWDC 的中国开发者明显比以前要多，而抽选机制也正给了我们很好的参加机会，至少我们不需要熬夜和一群“疯子”在十几秒内抢票了。如果您看到这篇文章的时候已经抽中了门票，并且付款成功并计划在 6 月的时候前往三藩的话，先大声说“恭喜恭喜恭喜你”！鉴于很多的参会者可能是第一次参加 WWDC，甚至可能是...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-04-19 21:10:11 +0900" class="post-list__meta--date date">2016-04-19</time> &#8226; <span class="post-list__meta--tags tags">南箕北斗集</span><a class="btn-border-small" href=/2016/04/first-wwdc/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
    <li>
      <h2 class="post-list__post-title post-title"><a href="/2016/04/objccn-plan/" title="访问 ObjC 中国的工作回顾和之后的计划">ObjC 中国的工作回顾和之后的计划</a></h2>
      <p class="excerpt">小时候因为成绩还算凑合，所以经常会被任命做个班干部什么的。其实这并不是一份很有意思的工作，除了上课要被老师重点“关照”点名起来回答问题以外，最烦人的事情就是开学要写工作计划，期末要写工作总结了。耗时耗力不说，写出来的东西也并不会有什么人看。所以我大抵对写计划和写总结这样的事情是抵触的。顺便还希望这篇总结加计划的东西能有人有兴趣看。时隔十几二十年后，再提笔 (其实是拿键盘) 开始写一份工作回顾和计划的时候，我却是怀着满心欢喜的。从 2014 年 3 月第一个 commit 开始，ObjC 中...&hellip;</p>
      <div class="post-list__meta"><time datetime="2016-04-07 10:51:24 +0900" class="post-list__meta--date date">2016-04-07</time> &#8226; <span class="post-list__meta--tags tags">南箕北斗集</span><a class="btn-border-small" href=/2016/04/objccn-plan/>继续阅读</a></div>
      <hr class="post-list__divider" />
    </li>
    
  </ol>

  <hr class="post-list__divider " />

<nav class="pagination" role="navigation">
    
    <span class="pagination__page-number">1 / 6</span>
    
        <a class="older-posts pagination__older btn btn-small btn-tertiary" href="/page/2/#blog">更早 &rarr;</a>
    
</nav>


</div>

            <section class="footer">
    <footer>
    	<span class="footer__copyright">本站点采用<a href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享 署名-非商业性使用-相同方式共享 4.0 国际 许可协议</a></span>
        <span class="footer__copyright">由 <a href="https://jekyllrb.com">Jekyll</a> 于 2018-11-20 生成</span>
        <span class="footer__copyright">本站由 <a href="https://onev.cat">@onevcat</a> 创建，采用 <a href="https://github.com/onevcat/vno-jekyll">Vno - Jekyll</a> 作为主题，您可以在 GitHub 找到<a href="https://github.com/onevcat/OneV-s-Den">本站源码</a> - &copy; 2018</span>
    </footer>
</section>

        </div>
    </div>
    
    <script type="text/javascript" src="//code.jquery.com/jquery-1.11.3.min.js"></script>



<script type="text/javascript" src="/js/main.js"></script>


<script>
    (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
    })(window,document,'script','//www.google-analytics.com/analytics.js','ga');
    ga('create', 'UA-25719337-1', 'onevcat.com');
    ga('send', 'pageview');
</script>


    
  </body>

</html>
