- html的语义化：语义化的含义就是用正确的标签做正确的事情，语义化就是让标签和其所包裹的内容的意思想吻合，html语义化就是让页面的内容结构化，便于对浏览器、搜索引擎解析；在没有样式CCS情况下也以一种文档格式显示，并且是容易阅读的。搜索引擎的爬虫依赖于标记来确定上下文和各个关键字的权重，利于SEO。使阅读源代码的人对网站更容易将网站分块，便于阅读维护理解。
    1.方便机器理解代码,利于SEO
    还拿上面两段代码举例子，第二段代码，别说机器了，就是人也看不出它表达的意思啊。而第一段代码无论是人还是机器，都是可以去理解的。
    搜索引擎爬虫理解了你的代码，你的网站排名自然有加分了。
    2.代码更简洁，复用性更高。使用合适的标签，可以少些很多css或者js。
    3.访问性更好
    这个主要就是针对读屏器或者其他一些对CSS理解不好的浏览器。语义化的HTML可以做到脱离CSS还能看，而非语义化的就难了。

如何让代码语义化：[让标签做正确的事情](http://www.w3school.com.cn/tags/html_ref_byfunc.asp)

- em和px以及一些度量单位
1em=16px
1. body选择器中声明Font-size=62.5%;
2. 将你的原来的px数值除以10，然后换上em作为单位;
3. 重新计算那些被放大的字体的em数值。避免字体大小的重复声明。
em有如下特点：  
1. em的值并不是固定的；  
2. em会继承父级元素的字体大小。

- img标签的title、alt属性的区别
alt 
此属性的实质作用是图片在无法正确显示的时候起到文本替代的作用,不过在IE6下还起到了title的作用（鼠标放上去后的文字提示），IE的实现方法实际上是错误的。如果想在鼠标滑过时显示提示,应该用title属性。
title 
鼠标滑过时显示的文字提示，用户体验上很重要。当然不必要所有的img标签都加此属性，比方说logo这样比较重要或者说用户会体验到的图片内容建议一定要加此属性。

- **css布局（涉及各种常见的布局，如两列布局、三列布局等）**


- 清除浮动的知识（最好给出多种方法及它们的区别，而且能解释原理，可以加分）
    - 添加新的元素 、应用 clear：both；
    - .over-flow{ overflow: auto/hidden;<!-- auto对seo友好 -->}
    - .outer :after {clear:both;content:'.';display:block;width: 0;height: 0;visibility:hidden;} 先说原理：这种方法清除浮动是现在网上最拉风的一种清除浮动，他就是利用:after和:before来在元素内部插入两个元素块，从面达到清除浮动的效果。其实现原理类似于clear:both方法，只是区别在于:clear在html插入一个div.clear标签，而outer利用其伪类clear:after在元素内部增加一个类似于div.clear的效果。 其中clear:both;指清除所有浮动；content: '.'; display:block;对于FF/chrome/opera/IE8不能缺少，其中content（）可以取值也可以为空。visibility:hidden;的作用是允许浏览器渲染它，但是不显示出来，这样才能实现清楚浮动。

- **CSS伪元素**

- **zoom 是什么意思**
- 实现ajax的过程

- http状态码
    - 200：服务器成功返回网页   一切正常，对GET和POST请求的应答文档跟在后面
    - 304：未修改 客户端有缓冲的文档并发出了一个条件性的请求（一般是提供If-Modified-Since头表示客户只想比指定日期更新的文档）。服务器告诉客户，原来缓冲的文档还可以继续使用。
    - 404：请求的网页不存在    请求出现语法错误。
    - 503服务器暂时不可用   服务器由于维护或者负载过重未能应答。例如，Servlet可能在数据库连接池已满的情况下返回503。服务器返回503时可以提供一个Retry-After头
    - 500：服务器内部错误     服务器遇到了意料不到的情况，不能完成客户的请求


- 取消a链接的默认跳转行为
- 水平垂直居中的各种方式
- js的数据类型判断
- 事件模型
- IE和DOM中事件绑定的区别（要求详细）
- js动画的知识（面试官考了我一个淡入淡出的动画）
- 定时器深入理解
- 获取元素的页面坐标（设计offsetTop、clientHeight等属性的深入理解）
- JsonP的相关知识
- http状态码（与第5题挂钩了）
- 块级元素与内联元素的详细区别（千万不要只答占满一行的区别，要求深入）
总结：一面涉及到的都是前端的基础知识，但是需要注意很多细节，不然会暴露自己的基础不扎实，而且当你答对之后，面试官还会深入，考察知识的深度，所以在平时的学习中，务必要把基础打扎实，不能似是而非。
- 什么叫CDN
- 什么叫restful
- <!DOCTYPE>标签定义、、用法
- 列举html标签中的行内元素、块级元素
- 引入样式表CSS的四种实现方式
- 你怎么理解 web2.0标准的
- 前端页面有那层三构成，都是什么？
- 你对 html5、css3的理解，都有什么新增功能
- 简化下面的代码
.main{font-family:"微软雅黑",Arial,"宋体";font-size:12px;font-weight:normal;line-height:1.8em;color:#333333;text-decoration:none;background-color:#333333;background-repeat:no-repeat; background-position: 0px 0px; padding-top: 5px; padding-right:6px; padding-bottom: 5px; padding-left: 6px; border-top-width: 1px; border-top-style: solid; border-top-color:#00CC66;}
8.根据图片，编写出来HTML结构 (图片没有，就是那种很常见的格式，左面一个商品图片，右边从上到下依次是产品名称，原价多少，秒杀价多少。) 　
9.编写一个HTML结构，是三列布局的，要求适应分辨率100%高度
10.最近看过什么书，平时关注的网站亦或是博客

什么叫做跨域，如何跨域的
- 谈谈自己所做过的项目（前端+后台）
- 盒模型
- 定位方式
- css3新增的属性
- css3实现IE盒模型
- css实现省略号
- 图片格式的区别（png24、png8的区别，出发点是考查兼容性）
- HTML5新增的属性
- 事件绑定
- this
- prototype
- construct
- 创建对象的各种模式
- css预处理（SASS,LESS）
- 如何对网站进行优化
- JS模块化
- 谈谈你熟悉的JS框架、类库
- 闭包
- 使用哪些工具来管理代码
- 移动端的知识
- 单页web应用
总结:二面涉及的知识明显升级了，考查了js里面的各种关键概念以及框架、类库等等，主要是看被面试者的知识掌握情况及运用能力。

谈谈数据结构中的时间复杂度如何计算的，链表和数组区别
写出快排，并说出快排的时间复杂度，还有最差情况是什么情况下
两个DIV说出你知道的一行排列方法
什么是文档流
行元素和块元素区别
什么是浮动，浮动的特点是什么
浮点数在计算机中如何存储，0.1+0.2为什么等于0.30000000000000004
谈一谈原型链
new一个对象时构造函数发生了什么，如果主动return一个对象，那返回的是什么

二面：
一个数组从1到100无序排列100个数，现在随机删除一个（length改变，数组长度变为99），如何找出那个数【我投机取巧说累加减去5050，谁知道他立马换了法子问我

一个数组n个乱序的字母，现在随机删除一个……【我想不到了只能说循环去找

数组去重 【我使用了ES6的sort类型，然后面试官立刻用换法子问我

两层循环的方式数组去重，何如缩减成一层循环 【我是‘，’ + arr.join(',') + ‘，’ ，在indexOf去找的，强行少一层循环，也不知对不对
谈谈原型链
domReady和window.onload的区别，什么时候不能使用domReady

1.对HTTP的了解，比如Get和Post的区别，200，404,这些分别代表什么含义？ 
2.HTML的一些基础知识，CSS选择器的优先问题，一般综合来问就是如何让一个div垂直居中，如何让图片与文字水平排列。。等等 
3.最主要的就是JS部分了。包括js的闭包，基本类型有几种，函数的一些，DOM的操作，事件的一些处理，绑定事件有几种方法等等，还有就是作用域，原型和原型链，如何实现继承，封装等等，考的深入的话就还包括AMD,CMD是什么了？以及MVVM(AngularJS BackboneJS等)，还有对Nodejs的了解。接着就一些一些框架，比如最常见的JQuery，一些基础的知识，问的问题基本上和js中的差不多，绑定事件、DOM操作等，也有喜欢问是否看过JQuery源码的。 
个人的一些面试了解吧，应该还有很多需要补充的。。针对楼主，应该还会问到Bootstrap的一些问题，主要还是看项目能够说明问题。祝楼主好运。希望可以一起了解学习

从浏览器输入 URL 到页面渲染发生了什么事？
浏览器接收用户输入
解析域名对应 IP，发送到服务器（被打断：谁解析 IP？答：DNS。）
向服务器请求网页
服务器返回网页请求
浏览器把得到的网页数据从字节流变成一个个 token
生成 DOM tree
渲染页面
同时异步加载网页中 CSS、JavaScript 等外部资源
这部分我是照记忆中《WebKit技术内幕》的回答的，摘录如下。

当用户输入网页 URL 的时候，WebKit 调用其资源加载器加载该 URL 对应的网页。
加载器依赖网络模块建立连接，发送请求并接收答复。
WebKit 接收到各种网页或者资源的数据，其中某些资源可能是同步或异步获取的。
网页被交给 HTML 解释器转变成一系列的词语（Token）。
解释器根据词语构建节点（Node），形成 DOM 树。
如果节点是 JavaScript 代码的话，调用 JavaScript 引擎解释并执行。
JavaScript 代码可能会修改 DOM 树的结构
如果节点需要依赖其他资源，例如图片、CSS、视频等，调用资源加载器来加载它们，但是它们是异步的，不会阻碍当前 DOM 树的创建，直到 JavaScript 的资源加载并被 JavaScript 引擎执行后才继续 DOM 树的创建。

JavaScript 事件模型（很重要，建议掌握，后续两轮面试都问到了）
Ajax如何跨域，有几种方法（当时只写了一个 JSONP，但是具体的原理的确没摸懂）
用 js 和 jquery 创建一个 table（虽然写出来了，但是不清楚这个问题有什么深意）
简述css盒模型（当时一哆嗦把 border 和 padding 的顺序写反了）
写一个左边定宽，右边自动扩展的网页布局

display 有哪几种值，分别是什么意思
text-decoration 分别有哪几种值
常见的浏览器兼容性问题有哪些
什么是 JS 事件冒泡
你知道的 CSS Hack 有哪些
会不会 SEO
怎么增加页面的加载速度
设计轮播效果

，如何判断当前的域名是属于腾讯的，也就是主域名要是qq.com。我就说，通过location.hostname取得服务器名，然后判断这个字符串是否包含qq.com，写了一个正则，/*.qq.com*/，很快就被否定了，面试官说，如果是qq.com.baidu.com呢，改为/*.qq.com$/。面试官说域名恰好是qq.com呢。由于正则只是打了个基础，再用正则来匹配就不会了，面试官提醒，正则不会可以用原始的方法嘛。想了想，可以取得字符串最后六个字符，判断是不是qq.com，似乎是没了问题，但面试官又说假如是aqq.com呢，哦，对呀，不行，我说那就先判断服务器名的长度，如果恰好只有六个字符，且是qq.com，那么就判断是，如果长于六个字符，那就用正则来匹配，就这样第一个问题过了。

，前端性能优化有哪些。基本的我还是知道一些的，答了几条，其实从这个时候我就知道他不懂前端，他很可能是通过你答的流畅度来判断你说的是否正确，答完之后他没有深究，继续下一题。

什么叫负载均衡

然问我知道不知道 ARP 协议， 我隐约记得早上看到过但是想不起来，后来一查是 地址解析协议

1.如何实现一个三栏布局

三栏布局，问到的时候我以为是左右固定，中间自适应，后来发现他就是想考我float。

    *{
        margin: 0;
        padding: 0;
    }
    .left,.right,.middle{
        float:left;
        border: solid 1px #777;
        width: 30%;
        margin:1.55%;
    }
然后面试官问我，这三个元素float了之后，对下面的元素有影响要怎么处理。

清除浮动问题我发现是前端面试CSS方面经常问的一个问题，详细可参考文章：那些年我们一起清除过的浮动。

主要的方法有添加多余标签，然后clear: both一下

    <div class="left"></div>
    <div class="middle"></div>
    <div class="right"></div>
    <div class="clear"></div>
然后CSS改一下

    .clear{
        clear: both;
    }
第二个方法是在父层容器添加overflow:auto属性

    <div class="overflow">
        <div class="left"></div>
        <div class="middle"></div>
        <div class="right"></div>
    </div>
    .overflow{
        overflow: auto;
    }
第三个方法是用伪类::after

    <div class="clearfix">
        <div class="left"></div>
        <div class="middle"></div>
        <div class="right"></div>
    </div>
由于IE6-7不支持:after，使用 zoom:1触发 hasLayout。

    .clearfix::after{
        display: block;
        content: "";
        visibility: hidden;
        clear: both;
    }
    .clearfix{
        *zoom:1;
    }
2.position的几种属性

我发现这个面试官的问题都不算刁钻，position也是在学布局的时候一定要接触到的。常用的position有static、fix、absolute和relative。

position:static
这个static是默认的，对块级框的块格式化，对行级框的行格式化，元素按照块格式化上下文或行格式化上下文正常排版。

position:relative
相对定位，元素正常排版，并可以用top left right bottom进行位置的偏移，然而后面的元素不会调整位置去适应这个相对定位的元素。

position:absolute
绝对定位，元素脱离正常排版，使用top left right bottom相对于第一个非static的父层定位。

position:fixed
与absolute类似，不过使用top left right bottom定位是在视口的固定位置上。

3.如何实现一个响应式布局

这个是一个经验题。我原以为他要问我对Bootstrap等类库的使用，加之我从没接触过移动端，对于除了使用过Bootstrap和使用百分比宽度没再尝试过别的。

面试官说明是要自己写响应式，然后我就说我就是用百分比设置宽度。然后他问半分比相对于谁？

所以说还是基础硬伤，因为自己做的时候没注意过相对于谁，而且大多是外框，所以就说相对于窗口。面试官一笑，窗口？我说好吧，我再查查。。。顺便查了一下盒模型设置的各个百分比都是相对于谁的。

CSS中：width、margin和padding百分比是相对于包含块的！
一般情况下包含块是父元素，当position: fixed的时候，包含块为视口；当position: absolute的时候，包含块为最近的position不是static的祖先。

除此之外，响应式布局的方法还有：
CSS3 Media Query

通过在<head>里面插入这段内容，使分辨率在小于1024分辨率的情况下和大于1024分辨率的情况下能响应不同的css文件。

    <meta name="viewport" content="width=device-width; initial-scale=1.0">
设置原始缩放比例和视窗的大小

    <link rel="stylesheet" type="text/css" href="common.css" media="all" />
    <link rel="stylesheet" type="text/css" href="normalScreen.css" media="screen and (max-width: 1024px)" />
    <link rel="stylesheet" type="text/css" href="widthScreen.css" media="screen and (min-width: 1024px)" />
同样，可以在样式表中镶嵌@media，文章推荐参考响应式布局这件小事

    1.Jquery中$('').click()和$('').on('click')的分别

我为了学基础，学原生的Javascript，已经很久没碰Jquery了。问到这个问题的时候，我只能很诚实的说我没有考虑过这个问题，如果让我说的话，可能是原生的JS中onclick事件与addEventListener("click")的区别。

在面试完之后，我立刻又上网查了这两个的分别，其实在效果上作用不大，就是说下列代码在实现上并没有很大差距。

    $("#myDiv").click(function(){
        alert("clicked");
    })
    $("#myDiv").on("click",function(){
        alert("clicked");
    })
不同的是，on()方法可以实现动态绑定。可以将所有的点击事件绑在一个父层元素上，也可以用off()方法解绑定。

    $("body").on("click","button",function(){
        var btnValue = this.val();
        alert(btnValue+"clicked");
    });
//为每一个按钮绑定点击事件

    $("#myDiv").off("click");//解除点击事件绑定
2.JS实现一个类

我发现，这个问题也是面试常会问到的，而且我觉得这也是我在学习JS的时候遇到的一个难点。
说起类，就要提起原型链的问题，这里直接上例子。对于原型，可以直接参考我大神男友的博文Javascript 面向对象特性(1)——抛弃类、Javascript 面向对象特性(2)——找回类。

《Javascript高级程序设计》中讲到继承的时候提到了六种方式：原型链、借用构造函数、组合继承、原型式继承、寄生式继承、寄生组合式集成。

原型链方式的具体用法是创建一个构造函数，然后创建继承这个构造函数的引用类型，将这个引用的原型指向构造函数。在原型链的问题是，Student的原型为Person的实例，那么所有Student的实例会共享它引用类型的属性，所以实例在修改这个属性的时候会导致其他实例的实例都被修改。

    function Person(name,age){
        this.name=name;
        this.age=age;
        this.sayName=function(){
            alert(this.name);
        }
    }
    function Student(school){
        this.school=school;
    }
Student.prototype= new Person();
借用构造函数的用法是在一个引用类型中调用构造函数，使用apply()和call()方法可以在函数内部调用构造函数。问题是，对于Student的实例找不到哪些是Person中定义的。

    function Person(name,age){
        this.name=name;
        this.age=age;
    }
    Person.prototype.sayName=function(){
        alert(this.name);
    }
    function Student(name,age,school){
        Person.call(this,name,age);
        this.school=school;
    }
组合方式是综合了原型链与借用构造函数两种方式。

    function Person(name,age){
        this.name=name;
        this.age=age;
    }
    Person.prototype.sayName=function(){
        alert(this.name);
    }
    function Student(name,age,school){
        Person.call(this,name,age);
        this.school=school;
    }
    Student.prototype= new Person();
    Student.prototype.constructor=Student;

    Student.prototype.saySchool=function(){
        alert(this.school);
    }
    var instance1=new Student("Kathy","23","UQ");
    var instance2=new Student("Visper","24","KMUST");

    instance1.saySchool();//UQ
    instance2.sayName();//Visper
    原型式继承，方法是通过一个现有的对象创建一个新的对象。

    //引自《Javascript高级程序设计》
    function object(o){
        function F(){}
        F.prototype = o;
        return new F();
    }
    var person = {
            name: "Kathy",
            age: "23"
    };
    var anotherPerson = Object.create(person);
    anotherPerson.name = "Visper";
    anotherPerson.age = "24";
寄生式继承的方法是将原型式继承封装在一个方法内，然后再用工厂式的创建对象的方法。

    //引自《Javascript高级程序设计》
    function object(o){
        function F(){}
        F.prototype = o;
        return new F();
    }
    var person = {
        name: "Kathy",
        age: "23"
    };
    function createPerson(original){
        var clone=object(original); 
        clone.sayName=function(){
            alert(this.name);
        };
        return clone;
    ￼}
    var anotherPerson = createAnother(person);
    anotherPerson.name = "Visper";
    anotherPerson.age = "24";
2.如何统计一个字符串中哪个字母出现的次数最多

这个问题又是算法题，而算法题是我相当不擅长的。。。不过有上次选取“字符串中第一个只出现一次的字符”的经验，这次也是比较快的想出了一个方法。不过，也还是不知道这个问题的最快解决办法是什么。

思路还是将字符串变成数组，然后再sort()排序，之后为每一组字符计算数字，将目前出现次数最多的字符以及其次数记下来。

```

    function maxCountValue(string){
        var letterArray=Array.prototype.slice.apply(string);
        var sortArray=letterArray.sort();
        var arrayLen=letterArray.length;
        var countNow=0,count=0,value=sortArray[0],maxCountValue="";
        for(var i=0;i<arrayLen;i++){
            //判断是否进入下个字符组
            if(value==sortArray[i]){
                countNow=countNow+1;
                //判断是否为最后一组并且判断当前次数以及目前最大次数
                if(i==arrayLen-1&count<countNow){
                    maxCountValue=value;
                }
            }
            else{
                //如果当前次数大于目前最大次数
                if(count<countNow){
                    count=countNow;
                    maxCountValue=value;
                }
                value=sortArray[i];
                countNow=0
                countNow=countNow+1;
            }
        }
        alert(maxCountValue);
    }
```

HTTP题目以及新技术题目
HTTP题目继续问到了AJAX的问题，上一篇面试题中有整理。

面试官紧接着有问到form提交和ajax提交的区别？
Form在提交的时候，会跳转页面或者原页面刷新。而AJAX是异步的，无需页面刷新而只是部分刷新。
Form提交时，JS不是必需的，而且数据按照表单结构提交。AJAX需要JS来实现，而且数据也要用程序处理。

之后面试官问到开发环境问题：

1、目前的开发环境是什么
曾用PC开发，使用EverEdit；这几个月转用Mac，使用HBuilder

2、shell操作 命令行用过什么
简单的前进到文件目录cd
列出当前文件夹内的文件 ls -li
改变所有人权限 chown
该文件读写模式 chmod

3、chrome的调试方法
Elements中查询元素结构、以及元素的样式
Network中查看每个资源的请求反馈时间
Sources中调试程序，在左栏程序文件上打断点，并在右侧输入变量名查看变量值的变化
Resource中查询Session、Cookie、本地存储及缓存的状态
Console中执行函数并查看错误行号或错误代码

4、代码管理工具使用过么？做哪些操作呢？
使用过Git：建立远程仓库，拉取本地仓库，更改之后submit，之后push到远程仓库。曾经Fork过别人的，然后修改过后也是submit再push。
说实话我做的个人项目比较多，对于GitHub的使用仅限于提交推送更新代码。所以也是大概的说了一下我的使用情况。

新技术题目

接触过什么比较前沿的技术？js框架、模块化 、自动化工具、预编译语言？
呃。。呃。。呃。。。

当时我的反应好尴尬，不过也是实话实说我没接触过什么，只不过听说过angular.js、backbone.js之类的。其余的都没太听说过。。。汗

不过我有表示我以后会努力学习，迎头赶上！

最后问道面试官对我的印象：1、经验不足，2、新技术接触的太少。

因为我目前时间有限，只有每天晚上整理面试题，所以这短短的几个题整理了接近一个星期，很多问题也期待大神们的补充。。。目前也算是找到了工作，今后会继续努力，让我的羽翼丰满起来！
2015年09月02日发布

饿了么：
http状态码都知道那些
数组去重
怎么构造一棵树
十进制数判断有多少位二进制码
性能优化了解多少
响应式    我只答了@media 
setTimeout 和setInterval的区别
setTimeout时间设为0是否立即执行，为什么？
构造函数的运行机制
this的绑定
call()和apply()的区别
Js继承有哪些？原型继承是什么样的
解释一下模块化，举例模块化的方法
GET和POST的区别
函数声明和函数字面量的区别
jQuery的联级有什么好处
如何平铺一张背景图？  

      css方法：设置一张图片 {position: absolute; top: 0; left: 0; bottom: 0; right: 0; z-index: -1;}
            
 js方法： 判断浏览器高度，设置图片的高度
如果让图片按比例放大缩小呢？    用Js来判断宽高，然后按比例放大（面试官说屏幕壁板都是横屏，所以width设置为100%就可以了）
Doctype的作用
渐进增强 优雅降级
css hack
条件注释
dispaly的值
css3动画的性能优化你知道什么？   我只答了最好不要使用all
什么是语义化
html5 语义化的标签
CSS
JavaScript
其他
position 定位
dom操作元素
两列布局
inline-block空隙怎么解决
事件代理
什么是冒泡什么是捕获
BFC，haslayout是什么，怎么触发
C++
jQuery取到的元素和原生Js取到的元素有什么区别
项目（这里聊了很久）
CSS
JavaScript
其他
给我介绍一下你都做过哪些项目吧？   
你是怎么进行团队项目的合作呢？  
你现在在学些什么呀？    
做前端有用不到C++，你学他有什么用呀？    我不只是一个写前端的，我还是一个程序员，C和C++是这些语言的基础，所以巴拉巴拉~
你最满意的C++程序讲一下？    Qt呀，类呀~什么的~
很长一段话要进行截取，超过之后是三个点怎么做？ 
不考虑兼容的话CSS3有 text-overflow：ellipsis   然后或者overfloww:hidden 再在边框前侧加入一个三个点的span
或者用伪元素：after{content:"..."}之类的吧
时间太久不记得了
鼠标滑过一个元素出现一个弹出层    就dom 0级来举例子的话是 onmouseover dispaly:block
鼠标滑的快不让他出现怎么办    设置一个setTimeout 当鼠标在上面停留的时间小于设定的时间的话他还没有出来事件就被取消掉了
那setTimeout应该设置多久的时间呢?    这个我不知道有什么约定俗成的时间设置，如果是我的话，应该回去试一下，看那个时间合适
现在我想要这个元素在页面下方是弹出层在上方显示，元素在上方时弹出层在下方显示？    判断元素距离页面底端的位置，位置大于弹出层的高度的话就在下方弹出，否则在上方弹出
如果我现在想把他做成一个工具给别人用要怎么做？    呃~首先使用模块化，注意不要和其他的方法什么的有冲突，然后子啊里面设置方法出入所需的参数，比如那个元素，什么事件，弹出层的大小等等
那想做一个好的工具参数肯定很多，你怎么能方便别人使用呢？毕竟参数这么多别人会记不住的    呃~我可能会设置成一个对象，传入对象的属性，这样就方便记住了。
你觉得淘宝首页有哪些技术优势？     页面很大，要承载的东西也很多，但是可以让用户清晰明了的找到想要找的东西证明布局做的非常好，然后里面包括图片轮播呀个中点击事件呀什么的事件也很多，所以避免事件冲突也很腻害~
那你觉的你用多久可以写出淘宝首页？    呃~一个星期吧（这个可真的不知道什么样的答案合适）
你为什么想来淘宝技术部？    因为技术牛，而且有很多大牛在这个团队里，如果我有机会的成为其中一员的话就业可以学到更多的东西啦~
你觉得你有什么优势可以来淘宝技术部？    嘿嘿，就不告诉你我是怎么答得
项目
版本控制
JavaScript
css
其他
css3翻书是怎么做的呀？    巴拉巴拉讲了一堆
你这个翻页有个bug呀，什么原因怎么改呀？    z-index的问题，怎么改布吉岛~
canvas绘图怎么做的呀？    巴拉巴拉讲了一堆
你这个绘制有bug呀，什么原因怎么改呀？    滚动条的问题，怎么改又布吉岛。。。（加上滚动条的距离，面试官告诉我的~）
了解版本控制器么？    了解一些github
基本操作会么？    我都用的windows的图形界面进行操作的（面试官心中可能有一万只草泥马在奔腾....）
github的工作原理是什么呀？    我把我的代码上传到github的仓库上，然后别人可以下载进行代码添加然后上传更新仓库，我可以再下载更新过的继续进行添加修改
那如果你们两个修改同一份代码发生冲突怎么办？    我知道的方法只有回滚，就是和队友交流看谁的代码更重要，然后进行一个回滚操作。
只能这样么，必须有一个人牺牲么？    我了解到github的功能其实非常强大，所以肯定有更好的方法吗，只是我现在对github的使用仅限于自己代码的存储以及一些小的修改，所以并不了解更好的方法。。。。
Array都有哪些方法呀？    join slice splice reverse sort foreach every等迭代方法  暂时只能想起这些
sort方法工作原理是什么样的？    我不知道怎么讲他的工作原理，只知道他在排序上的问题巴拉巴拉的讲了一下。。。
那如果想要sort排序数字怎么办？   function(a,b){return b-a;}这样是降序
String有哪些方法呀？   concat  charAt slice substr substring 等等（其实现在觉得应该加一句说string是基本数据类型，没有方法，string的方法是String构造函数创建的引用类型的方法~）
那replace方法怎么用的呀？    我很认真的答成了splice的用法。。。。（两个参数   1.RegExp对象或者是字符串2.字符串或者函数  然后替换可以用正则进行全局替换。。。。）
一个div怎么垂直居中呀？   饿了么说过了~
css3你常用的属性有什么呀？    动画的transform transmation  border-radious box-sizing box-shadow 
你常用的代码编写工具是什么？    sublime text
你要修改很多相同的地方怎么办？    选中一个 按Ctrl+D 选取多个 然后一起改
photoshop怎么样？    可以进行简单的psd页面图的ps 不会人物风景的美化
想要导出一个文件提及比较小的png怎么做    存储为web所用格式。。。（应该不对~）
优先队列
堆
快速排序
float高度塌陷解决方案：
 clearfix:after{clear:both;content:".";height:0;display:block;visibility:hidden;}(给自己挖了个坑after是伪元素不是伪类，我说错了~)
line-height像素单位和百分比的单位的计算方法： length 设置固定的行间距。
单位em，px，pt等等。百分比% ，基于当前字体尺寸的百分比行间距。（我觉得我答得是对的，但是他有重复了一遍：我说的是line-height）
一个ul里有若干个li，想要每个li都有一个border-bottom，最后一个li不想要boder-bottom要怎么做：(ul:last-child{border-bottom:none;}或者给最后一个li加一个class选择器设置border:none;(他说还有，查了一下什么加载jQuery可之类的~)
css 选择器过长怎么判断他的优先级：行内样式1000 -- id100 -- 类、伪类、属性选择器10 -- 类型选择器、伪元素选择器1  通过相加计算大的优先级高，值相等的话后声明的优先级高。
addEventListener最后一个参数是做什么用的    答：规定事件是冒泡还是捕获。false是冒泡，true是捕获
什么是冒泡，什么是捕获    答：当一个元素触发了一个事件之后就会像上层传递直至body，document。捕获是从最不具体的传至最具体的
所有的事件都可以冒泡么    答：不是，blur focus change不可冒泡
怎么取消事件冒泡    答：eve.preventDefault(阻止事件默认行为)（这都没答上来，我一定是个逗比）
怎么判断是不是数组    答：a instanceof Array  Array.isArray(a)  他问我还有么~ 所以我说试一下Array的内置函数，可以使用是Array不可以则不是，其实还有 Object.prototype.toString === '[object Array]'
怎么把一个类数组对象转化为数组    答：Array.prototype.slice.call()；
讲一下继承：巴拉巴拉的讲了一大堆（因为他看了我的博客）
JavaScript :
CSS：

1.html的语义化
2.img标签的title、alt属性的区别
3.css布局（涉及各种常见的布局，如两列布局、三列布局等）
4.清除浮动的知识（最好给出多种方法及它们的区别，而且能解释原理，可以加分）
5.实现ajax的过程（在最后的一步的响应中，还问到了其他的http状态码的作用，所以基本的http知识是必备的，而且加分）
6.取消a链接的默认跳转行为
7.水平垂直居中的各种方式
8.js的数据类型判断
9.事件模型
10.IE和DOM中事件绑定的区别（要求详细）
11.js动画的知识（面试官考了我一个淡入淡出的动画）
12.定时器深入理解
13.获取元素的页面坐标（设计offsetTop、clientHeight等属性的深入理解）
14.JsonP的相关知识
15.http状态码（与第5题挂钩了）
16.块级元素与内联元素的详细区别（千万不要只答占满一行的区别，要求深入）
总结：一面涉及到的都是前端的基础知识，但是需要注意很多细节，不然会暴露自己的基础不扎实，而且当你答对之后，面试官还会深入，考察知识的深度，所以在平时的学习中，务必要把基础打扎实，不能似是而非。

1.谈谈自己所做过的项目（前端+后台）
2.盒模型
3.定位方式
4.css3新增的属性
5.css3实现IE盒模型
6.css实现省略号
7.图片格式的区别（png24、png8的区别，出发点是考查兼容性）
8.HTML5新增的属性
9.事件绑定
10.this
11.prototype
12.construct
13.创建对象的各种模式
14.css预处理（SASS,LESS）
15.如何对网站进行优化
16.JS模块化
17.谈谈你熟悉的JS框架、类库
18.闭包
19.使用哪些工具来管理代码
20.移动端的知识
21.单页web应用
总结:二面涉及的知识明显升级了，考查了js里面的各种关键概念以及框架、类库等等，主要是看被面试者的知识掌握情况及运用能力。


前端优化
这个是老生常谈的问题了，方法一搜一大把。回答了一些常用的方法：样式表放在head标签内，脚本放在body闭标签前，图片预加载，懒加载，选择合适的图片压缩格式，CSS Sprite，代码压缩，优化JS中性能开销较大操作(for循环、DOM操作之类的)，合并代码，使用CDN等，其中有些原理都是减少HTTP请求。面试官详细问了是怎么使用CSS Sprite的，大概原理就是把许多小的png图片整合到一张大的png图里，文件总大小还是一样，但之前有多少张图片就得请求多少次，而现在只要请求一次，使用的时候得用到CSS的background-position属性，这个图像合并和样式表和脚本合并都是为了减少HTTP请求来提升速度，面试官又问我怎么合并图片的，我是找了一个在线工具，把许多图片打包上传，填写相关参数之后就可以合并了，最后把大图下载下来就可以使用了，面试官还问了，如果再添加一张小图上去应该怎么办？没遇到这种问题啊，又懵了，机智的回答把小图添加到之前的小图里去，再打包生成？还是和大图打包再生成？算了，这个问题Pass吧

CSS3动画
我没有听清楚这个问题，我只听到了动画这个关键字，这个小Case啦，先JS获取这个元素，再添加事件，再在函数里写 动画的语句，主要是用到定时器，信心满满的等面试官的回话，他说不是这个，是用CSS3来实现动画，顿了一会儿模凌两可说animation，然后用transform和transition搞搞，我只是有点印象，还好面试官说知道就行了，当时我就在想，这面试官很适合我啊，心中一阵窃喜飘过，哈哈！

JavaScript连接字符串的几种方法
这个问题，还是有+这个操作符更常用的来连接字符串吗？有些书上又说，使用+=的性能会更好，还记得有个字符串方法可以连接字符串，只是记得，具体不知道是啥，事后查了一下是concat()，该方法用于连接两个或多个字符串

盒子模型
盒子模型从内到外分别是content、padding、border、margin，万恶的IE的content包含了padding和border，说到这个必须要说CSS的兼容性，其实兼容IE6我是打死都要拒绝的，所以，只要你的CSS中没有使用太多的横向padding值，网页也不会发生严重的错位。当然，前提是你的其他CSS写法是符合标准的。这个问题我也是瞎蒙

CSS Hack写法
因为IE的盒子模型不按标准来，So，用CSS Hack来让它“标准”起来，原理就是针对不同的IE浏览器写只有它们各自能识别的代码

```

    .hack{
        color:gray; /* FF,OP支持 */
        color:pink\9; /* IE678支持，但是后面的IE67会覆盖该条样式，所以这种顺序的写法使得该条样式只用于IE8*/
        *color:red; /* IE7支持 */
        _color:blue; /* IE6支持 */
    }
```
注意代码的先后顺序！

    <div id="outer">
        <p id="inner">Click me!</p>
    </div>
上面的代码当中一个div元素当中有一个p子元素，如果两个元素都有一个click的处理函数，那么我们怎么才能知道哪一个函数会首先被触发呢

事件冒泡
当一个元素上的事件被触发的时候，比如说鼠标点击了一个按钮，同样的事件将会在那个元素的所有祖先元素中被触发，这一过程被称为事件冒泡，这个事件从原始元素开始一直冒泡到DOM树的最上层，因此上面的例子在事件冒泡的概念下发生click事件的顺序应该是p -> div -> body -> html -> document

阻止事件冒泡
在IE和FF浏览器内阻止冒泡行为是不同的。IE中使用cancelBubble，FF中使用stopPropation()

事件捕获
与事件冒泡相反，事件会从最外层开始发生，直到最具体的元素。上面的例子在事件捕获的概念下发生click事件的顺序应该是document -> html -> body -> div -> p

事件代理

    <ul id="color">
        <li>red</li>
        <li>yellow</li>
        <li>blue</li>
        <li>green</li>
        <li>black</li>
        <li>white</li>
    </ul>
如果点击页面中的li元素，然后输出li当中的颜色字符串，我们通常会用循环给每个li添加点击事件，但是，利用事件代理，像下面这样

    var color_list = document.getElementById('color');
    color_list.addEventListener('click', showColor, false);
    function showColor(e){
        var x = e.target;
        if(x.nodeName.toLowerCase() === 'li'){
            console.log('The color is ' + x.innerHTML);
        }
    }
跨域
在页面上使用Ajax请求访问其他服务器的数据，此时会出现跨域问题。跨域问题是由于JavaScript语言安全限制中的同源策略造成的。简单来说，同源策略是指一段脚本只能读取来自同一来源的窗口和文档的属性，这里的同一来源指的是主机名、协议和端口号的组合。解决跨域大多使用JSONP(JSON with Padding)，原理是script标签是可以跨域访问服务器上的数据的，因此，可以指定script的src属性为跨域的url，从而实现跨域访问

原型
没用过这东西，不过感觉应该是太深奥了所以没用到，面试官问我这个问题，我就说prototype，面试官说只知道，没用过是吧？我自信满满的回答嗯，面试官说行，运气真好啊

Cookie
哈哈！又是我不明白的问题，笑着笑着就哭了，腾讯的面试比较难我算是见识了，问的都是我不常用的东西，Cookie可以在客户端存储数据，可以实现记住账号密码，购物车和换肤之类的功能。浏览器存储Cookie的大小和条数是有区别的，总的来说应该尽量保证Cookie的数量以及相应的大小。Cookie个数最好不超过20~30个，大小最好小于4K，被问倒了。问题还没完，Cookie还有domain，它用来表示Cookie所在的域，默认为请求的地址，还有path表示Cookie所在的目录，默认为/，就是根目录。这个真是一点不懂，他用test.qq.com和qq.com和我解释了一会儿，我算是懂了一点儿，被虐

正则表达式
不会啊，只是偶尔用来过滤表单啊，尼玛完全没系统学过啊！我就“挑衅”的说你问一个看看，他问，怎么用正则检测中文字符串，我就记得检测中文的正则表达式里含有u这个东东，后面跟几个字符，后来查了一下才知道是下面这样的

var regChinese = new Regex("[\u4e00-\u9fa5]");
只怪自己没好好学习，还瞎显摆，面试官主动跳过这个问题

后面还问我有没有用过CSS样式表，我当时是一愣一愣的，当然用过，还问我CSS选择符，这是什么鬼？不都是叫CSS选择器么？后面还问了事件，其他的和阿里的面的差不多。


HTML 有哪些块级元素，与行内元素的区别。
怎么添加事件
JavaScript 代码实现数组去重
JavaScript 类怎么实现，继承，私有变量怎么实现
给了一段代码写出运行结果，这道题主要考了作用域和闭包的概念
Ajax 跨域怎么实现
是否使用过 Linux，是否熟悉 Linux 指令
Ajax 原理
服务端状态码的含义，比如：1xx，2xx，3xx，4xx，5xx
前端加载优化的方法 我主要答了 JavaScript 加载优化的方法
怎么合并数组，删除数组指定位置的元素

百度前端学院
localStorage, sessionStorage, cookie
个人博客的创建
响应式布局

字体的控制，媒体查询中，文字大小应该使用 em 或 rem 做单位，不应该使用 px。这个其实我是知道的，但是我没有用过，并且当时也忘了。

前端代码压缩
使用过什么框架，是否用过 jQuery
模块化框架
……还有一些，我还是想不起来了

之前下载视频的题目是怎么实现的，这个问的很详细
是否会翻墙
关于 GitHub 被 DDoS 攻击是怎么回事
你做项目遇到过的难点
怎么攻克难点的，为什么选择这种方法？
有没有尝试别的方法？
为什么不选择别的方法？
有没有发布过自己的应用、软件
个人博客为什么选择 Jekyll 实现
具体是怎么实现的，是否有响应式设计
除了 GitHub 还用过什么代码托管的网站
为什么选择 GitHub
技术来源有哪些，关于 StackOverFlow、知乎之类
……还有我想不起来了

答：最长的一段代码，就是基于Ajax的评论功能。。。blabla。。。（没说完，玉伯打断）
玉伯：除了Ajax，你了解像JSONP这种跨域的方式？
答：了解，我知道除了JSONP还有图像Ping，Comet之类的方式
玉伯：图像ping？（一脸诧异，好像没听过这个方法一样）能给我解释一下吗？
答：blabla。。。（稍作解释，然后说了下和JSONP的不同）
玉伯：你知道通过XHR实现的这种跨域方式吗？
答：您是说CORS方式吗？
伯：（重新拼了一下）CORS，对
答：知道。。blabla。。。
玉伯：那为什么要有CORS这种方式？
答：刚开始跨域并没有标准的 方法去实现，程序员就使用了像JSONP这种方式来实现。然后官方为了支持跨域，就实现了CORS方式
玉伯：CORS方式是标准的官方方式
答：应该是吧
玉伯：那CORS和JSONP最大的不同是什么？


事件代理（事件冒泡模型）
javascript闭包
Linux 和 Github 操作
MongoDB
jQuery插件的写法
javascript的面向对象

html文档第一行的用处
区分块级元素和行内元素
javascipt的面向对象（很重要，必问）
ES5的严格模式

模块化
ES5的数组方法
前端自动化工具

inline-block的问题
前端安全，cookie，xss等等


一、   耐心填一填！（每空4分，共24分）

1. 为div设置类a与b,应编写HTML代码 _<div class=”a b”>_</div>_________。
2. 设置CSS属性clear的值为 _both___________时可清除左右两边浮动。
3.   ____li________标签必须直接嵌套于ul、ol中。
4. CSS属性 _____margin_______可为元素设置外补丁。
5. 设置CSS属性float的值为 ___none_________时可取消元素的浮动。
6. 文字居中的CSS代码是 ____text-align:center________。
二、   精心选一选！（每题4分，共16分）
1. 下列哪个样式定义后,内联(非块状)元素可以定义宽度和高度( C  )
A. display:inline      B. display:none     C. display:block    D. display:inheric
2. 选出你认为最合理的定义标题的方法( C    )
A. <span class=”heading”>文章标题</span>
B. <p><b>文章标题</b></p>
C. <h1>文章标题</h1>
D. <strong>文章标题</strong>
3. br标签在XHTML中语义为( A    )
A.换行          B.强调          C.段落          D.标题
4. 不换行必须设置(  AC  )
A.word-break        B.letter-spacing        C.white-space       D.word-spacing
5. 在使用table表现数据时，有时候表现出来的会比自己实际设置的宽度要宽，为此需要设置下面哪些属性值(  AD   )
A. cellpadding=”0″      B. padding:0        C. margin:0     D.  cellspacing=”0″
三、判断对或错！ （每题4分，共24分）
1. CSS属性font-style 用于设置字体的粗细。                 (  ×   )
2. CSS属性overflow用于设置元素超过宽度时是否隐藏或显示滚动条。 (   √  )
3. 在不涉及样式情况下,页面元素的优先显示与结构摆放顺序无关。(   ×  )
4. 在不涉及样式情况下,页面元素的优先显示与标签选用无关。     (   √  )
5. display:inline兼容所有的浏览器。                  (  √   )
6. input属于窗体元素,层级显示比flash、其它元素都高。  (   ×  )

四、用心想一想，你一定是生活中的智者！ （每题9分，共36分）
1. 写出ul、ol、dl三种列表的html结构。
答：

    <ul> 
             <li> </li> 
       </ul> 
       <ol> 
             <li> </li> 
       </ol> 
       <dl> 
            <dt> </dt> 
            <dd> </dd> 
       </dl> 
2. 将以下CSS代码进行缩写，注意要符合缩写的规范。
a) 代码一：

    border-width:1px;  
    border-color:#000;  
    border-style:solid;  

b)
 代码二：

    background-position:0 0;  
    background-repeat:no-repeat;  
    background-attachment:fixed;  
    background-color:#f00;  
    background-image:url(background.gif);  
c)代码三：

    font-style:italic;  
    font-family:"Lucida Grande",sans-serif;  
    font-size:1em;  
    font-weight:bold;  
    font-variant:small-caps;  
    line-height:140%;  

d) 代码四：

    list-style-position:inside;  
    list-style-type:square;  
    list-style-image:url(image.gif); 

e)代码五：

    margin-left:20px;  
    margin-right:20px;  
    margin-bottom:5px;  
    margin-top:20px; 

f)代码六

    color:#336699;  
    color:#ffcc00; 
答：

    代码一：border:1px #000 solid;
    代码二：background: #f00 url(background.gif) no-repeat fixed 0 0;
    代码三：font:italic bold small-caps 1em/140% "lucida Grande",sans-serif;
    代码四：list-style: url(image.gif) square inside;
    代码五：margin:20px 20px 5px 20px;
    代码六：color:#369;color:#fc0;

3. 修改以下代码，使其结构更加合理以及符合W3C标准。（XHTML 1.0 Strict）

代码：

    <div> <h2>Don’t buy these electronics used</h2> Money may be tight, but you may kick yourself for purchasing these electronics secondhand. <br /> Even when the price is low, the risk may be too high. <br /> <p><img src=”album.jpg”></p> <p> <a href=”home.html” target=”_blank”>home</a> <a href=”content.html” target=”_blank”>content</a> </p> </div>

答：

    <div>  <h2>Don’t buy these electronics used</h2>  <p> Money may be tight, but you may kick yourself for purchasing these electronics secondhand. </p>  <p>Even when the price is low, the risk may be too high.</p>  <img src="album.jpg" alt="album" />  <ul>    <li><a href="home.html" rel="external" title="home">home</a></li>    <li><a href="content.html" rel="external" title="content">content</a></li>  </ul></div>

4. 简述border:none以及border:0的区别，并给出使用建议。

答：border:none表示边框样式无,border:0表示边框宽度为0;当定义了border:none,即隐藏了边框的显示,实际就是边框宽度为0.
当定义边框时,必须定义边框的显示样式.因为边框默认样式为不显示none,所以仅设置边框宽度,由于样式不存在,边框的宽度也自动被设置为0.

五、勇气拼一拼，让你超越别人的加分题目来了！ （不限于一种方法，共30分）

使用重构的方式制作出一个如下图的水平、垂直都居中短边为50px，长边为150px的红色十字架。



十字架

要求：
1.使用2个div完成
2.使用3个div完成
3.使用5个div完成

答案：

1.使用2个div完成

    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> 
    <html xmlns="http://www.w3.org/1999/xhtml"> 
    <head> 
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" /> 
    <title>2个DIV</title> 
    <style type="text/css"> 
    #heng,#shu{left:50%;top:50%;position:absolute; background-color:#f00;}  
    #shu{width:50px;height:150px;margin-left:-25px;margin-top:-75px;}  
    #heng{width:150px;height:50px;margin-left:-75px;margin-top:-25px;background-color:#f00;}  
    </style> 
    </head> 
    <body> 
         <div id="heng"></div> 
         <div id="shu"></div> 
    </body> 
    </html> 
2.使用3个div完成

    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> 
    <html xmlns="http://www.w3.org/1999/xhtml"> 
    <head> 
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" /> 
    <style type="text/css"> 
    .main{width:150px; height:150px; top:50%; left:50%; position:absolute; margin:-75px 0 0 -75px; border:2px #F00 solid;}  
    .heng{width:150px; height:50px; background:#F00; margin-top:50px;}  
    .shu{width:50px; height:150px; background:#F00; margin-left:50px; margin-top:-100px;/*margin上边界叠加*/}  
    </style> 
    <title>3个DIV</title> 
    </head> 
    <body> 
      <div class="main"> 
             <div class="heng"></div> 
             <div class="shu"></div> 
    </div> 
    </body> 
    </html> 
3.使用5个div完成

    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> 
    <html xmlns="http://www.w3.org/1999/xhtml"> 
    <head> 
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" /> 
    <title>5个DIV(www.hemin.cn)</title> 
    <style type="text/css"> 
    #top,#middle,#left,#right,#bottom{height:50px;width:50px;position:absolute;top:50%;left:50%;}  
    #top{margin:-75px 0 0 -25px;background:#F00;}  
    #middle{margin:-25px 0 0 -25px;background:#000;}  
    #left{margin:-25px 0 0 -75px;background:#00F;}  
    #right{margin:-25px 0 0 25px;background:#0F0;}  
    #bottom{margin:25px 0 0 -25px;background:#FF0;}  
    </style> 
    </head> 
    <body> 
    <div id="top"></div> 
    <div id="middle"></div> 
    <div id="left"></div> 
    <div id="right"></div> 
    <div id="bottom"></div> 
    </body> 
    </html> 

