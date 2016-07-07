
移动应用是如何运行的
===

如何识别不同的编程语言
===

漫谈编程语言：数量
---

这又是一个有趣的话题~~，要知道编程语言有那么的多。引自Quora上一个相关问题（《[How many programming languages are there in the world?](https://www.quora.com/How-many-programming-languages-are-there-in-the-world)》）的答案，从ABC到Z Shell就有256个。

但是这并不是最佳的答案，要知道维基百科上的《[List of programming languages](https://en.wikipedia.org/wiki/List_of_programming_languages)》就有500+种编程语言了。

而据另外一个历史悠久的网站“[99 Bottles of Beer](http://www.99-bottles-of-beer.net/)”(创办于1994-1998年期间，当时大概就收录了227语语言了)所统计，已经有1500+种语言了。

根据德国语言学家在1979年的统计，当时世界上已经查明的语言有5651种。要知道世界人口有75亿左右，而程序员才有18.5M（引自Quora: 《[Approximately how many programmers are there in the world?](https://www.quora.com/Approximately-how-many-programmers-are-there-in-the-world)》）。

这就意味着平均每10000个人中就会创建一个新的语言。等等，这些语言里面还没有算上很多程序员在大学学龙书（《编译原理》）时创造的各种奇怪的语言。还有，我打算在未来写的一门叫xo的语言。

![Most Popular Language](./images/most-popular-language.jpg)

然而和这一个世界类似的，不是很有人都会使用使用的语言。汉语是这个世界上使用人数最多的语言，英语是这个世界上最流行的语言。同样的，Java是这个世界上使用人数最多的语言(依据[Tiobe](http://www.tiobe.com/tiobe_index)统计的结果)，JavaScript是这个世界上最流行的编程语言。

等等，Java和JavaScript是什么关系？他们两的关系就是汉语和英语的关系，都带了一个“语”(Java)字。

漫谈编程语言：语系
---

虽然说编程语言有那么多，但是实际上平时人们在社交网络上讨论的应该就那么几十种吧。同样的这些编程语言也有语系这种概念，以母语使用人口排列（引自维基百科: 《[语言系属分类](https://zh.wikipedia.org/wiki/%E8%AF%AD%E8%A8%80%E7%B3%BB%E5%B1%9E%E5%88%86%E7%B1%BB)》），最流行的就是印欧语系、然后就是汉藏语系，当然还有其他的小类型咯。同样的，这也适用于编程语言，只是维基百科将编程语言的类型分为了四十几种（《[List of programming languages by type](https://en.wikipedia.org/wiki/List_of_programming_languages_by_type)》）——这有点超乎我的想象了。换句话来说，这TM太扯了。

要知道小时候我学编程的时候，可只有：``机器语言``、``汇编语言``、``高级语言``、``系统语言``这几种概念。但是这种分类一点都无助于我们来对编程语言进行分类。这里我们就不考虑汇编语言这一类的低级语言，直接从高级语言下手，可以将程序语言简单的分为两类：

  - 解释型语言
  - 编译型语言

简单的让我们来了解一下这两类的编程语言：

编译型语言，顾名思义就是编译一下再运行的语言。而在其编译过后，会生成一个目标平台的指令，这样才能在那上面运行。因此在每次编译的时候，我们都需要保证代码是可以编译的，然后才是保证代码是可以工作的。这一类的语言总的来说都比较繁琐、复杂，但是相当有挑战性，其代表语言有：C++、C、Java，还有Go、Rust等等。不对，Java其实是解释型语言，因为它会编译成与平台无关的代码。

解释型语言，我不知道为什么Interpreted Language会翻译成解释型语言，总觉得“演绎”这个词来得更加精彩。简单地来说，就是在一步步演绎的过程中，演绎过一段精彩的故事。又扯远了，解释型语言就是在运行的时候才将代码翻译成机器可以执行的语言。这意意味着，我们可以在边写代码的时候，边试运行我们的代码。但是由于它需要在每次运行的时候才编译，所以总的来说效率会相对比较低一些。这一类的语言往往有比较好的跨平台能力，多数的语言都可以直接运行在不同的平台上。如Python、Perl、Ruby，还有直接可以运行于浏览器之上的JavaScript。

哈哈，现在我们可以来对不同的编程语言做一些了解。

不同的编程语言
---

扯那么多废话，也是时候进入正题了，现在让我们先从 Tiobe 上排名第一的语言说起。没错，这就是最近舆论的一个焦点——Java。

### Java和XML

那些写Java的程序员，实际上也都是个个都XML[^xml]高手，Java是他们的第二语言。

![XML](./images/xml.png)

所以如果你看到有一个项目使用到了XML，并且用到了Java语言，那么它应该就是一个Java项目了。

SUN推出的打算运行在嵌入式设备的一种通用语言，James Gosling等人发明这个语言的原因是因为 C++ 太难用了——后来，有一些人也因为难用改称C++为C艹。不过，Java语言运行在你家微波炉的计划很快就破灭了，于是它们就打算运行在浏览器之上。结果它运行在浏览器上的计划又失败了，但是这种做法便诞生了JavaScript。所以，其实Java和JavaScript还是有蛮大的关系的。

今天，Java又运行在嵌入式设备上了——Android手机，也驱动着相当数量的网站。只是拿它做桌面应用的话，真的不是一般的丑：

![Swing GUI](./images/java-gui.png)

看到这样的界面，你应该有足够的理由想到这是一个Java的GUI应用。丑是丑了点，但是它毕竟可以直接在不同的平台上运行啊。

现在，让我们来看看Java的代码一般都长什么样？首先，它一定是以.java作为后缀而结尾的。

```java
package com.phodal.java;
import java.io.IOException;

import org.apache.http.HttpEntity;
import org.apache.http.HttpResponse;
import org.apache.http.client.ClientProtocolException;
import org.apache.http.client.HttpClient;
import org.apache.http.client.methods.HttpGet;
import org.apache.http.impl.client.DefaultHttpClient;
import org.apache.http.params.BasicHttpParams;
import org.apache.http.params.HttpConnectionParams;
import org.apache.http.params.HttpParams;
import org.apache.http.util.EntityUtils

public class NetWorkUtil {

    public static String loginCheck_Get_HttpClient(String url) {
        String result = "";

        HttpGet get = new HttpGet(url);
        HttpParams params = new BasicHttpParams();
        HttpConnectionParams.setConnectionTimeout(params, 5*1000);
        HttpConnectionParams.setSoTimeout(params, 5*1000);

        HttpClient client = new DefaultHttpClient(params);
        // ...
        return result;
    }
}
```

如上是一个Java代码文件，在最开始的地方写的是包名。它可以很好的用于组织类、目录结构、防止命名冲突等等。通常来说，Java的包名以一定的规律来命名的，即：公司名称.开发组名称.项目名称。这一点同样可以见于Android应用的包名，如QQ是叫``com.tencent.qq``，而微信的是叫``com.tencent.mm``，微信的英语好像是WeChat，所以这个项目名称就不是叫WC了。不过，这看上去就有像网站的域名倒过去的样子，如上的com.phodal.java，倒过来就是java.phodal.com，同理也适用于tencent等等。

接着出现了长长的``import``开头的代码，这表示了它要调用的包，上面就有相当数量的apache的包名了。Apache，Java世界的最大基金会之一，其代码软件是HTTP服务器Apache。以及其下属的一系列Java相关的开源软件，如：Hadoop、Storm、Lucene、Maven、Struts、Tomcat等等，以及诸如Cassandra、OpenOffice、Subversion、ActiveMQ、CouchDB、Cordova这样顶顶大名的软件。总而言之，它为世界和平做出了重要的贡献。

顺便提一下另外一家写Java出名的基金会，Eclipse——最初是由IBM公司开发的替代商业软件Visual Age for Java的下一代IDE开发环境，后来它变成了Eclipse基金会，其代表作品是Eclipse IDE。

![Eclipse IDE](./images/eclipse.png)

有相当数量的IDE都是基于Eclipse，也有相当数量的Java GUI用的也是它，它的开头是:

```java
import org.eclipse.swt.*;
import org.eclipse.swt.widgets.*;

public class HelloWorld
{
    //...
}
```

如果是Web应用，那么它使用Spring的概率是相当大的：

```java
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;
import org.springframework.web.servlet.ModelAndView;
```

好了，让我们继续XML的话题，对于每个Java程序员来说，他们写的XML代码可能比Java还多。当一个程序员引用第三方库的时候，她多半需要这样写，以此来添加这个依赖库：

```xml
<!-- https://mvnrepository.com/artifact/org.mybatis/mybatis -->
<dependency>
    <groupId>org.mybatis</groupId>
    <artifactId>mybatis</artifactId>
    <version>3.2.8</version>
</dependency>
```

当然，在今天很多人可能会用Gradle：

``` groovy
compile group: 'org.mybatis', name: 'mybatis', version: '3.2.8'
```

通常来说，它会写上这两种方法来表明这是一个Java项目。除此，还有一种方法可以证明这是一个Java语言的项目，那就是它的代码写起来很繁琐——看看最前端的Java代码你就知道了，它为了调用一个HTTP请求，居然需要这么多的类。除此，你还需要这样的代码用来对某个变量进行操作。。。

```java
	public Long getId() {
		return this.id;
	}

	public void setId(Long id) {
		this.id = id;
	}

	public String getName() {
		return this.name;
	}

	public void setName(String name) {
		this.name = name;
	}
```

我受不了，人生本来就如此的短暂，我居然要写这么没有意义的代码。

### 人生苦短，我用Python

那个装着“人生苦短，我用Python”衣服的大叔就是写了Python语言的大叔：

![人生苦短 我用Python](./images/guido-python.jpg)

这么语言的最大特别是，格式固定，你不能写出下面的这种代码：

![浪客剑心](./images/ioccc-ke.jpg)

在哪个地方是一个缩进，你就应该用一个缩进：

![Python缩进](./images/python-demo.jpg)

不对，我应该用两个空格：

![Tabs vs Space](./images/tab-space.png)

Python语言的人喜欢争论的是Tab和空格的问题，就好比是两个不同的帮派。但是你不能这样混合着用（点的地方是空格，长线的是Tab），会被打死的：

![Tabs Space Both](./images/hybrid-tabs-spaces.png)

与Java相比，Python相比来说更为简单些。以致于它成为了相当多的科学家、数学家的使用语言，它在这方面颇有建树。

//TODO 待续

然而，Python毕竟是一门相对比较简单的语言，她追求做事只有一种方法。而有一些程序员就不喜欢如此了，它们喜欢最事有很多方法，并且可以按自己的规则来办事。

### Ruby

Ruby和Python看上去有点相似——如果只是一行简单的代码的话。不过，有一点值得注意的事，应该没有人愿意去维护别人写的Ruby代码——新手Ruby程序员一般看不懂有经验的Ruby程序员写的代码：


Ruby 是一个宝石，不知行弘想送给谁。RoR 火车上的宝石，但是太重了，比不上新干线

Ruby on Rails Girl

话说，Ruby是继承自另外一种神奇的语言Lisp的风格。

### Lisp

Lisp语言的特征是“（）”，如果你看到一个大的Lisp项目，那么它的结果可能是这样的：

![Lisp Styles](./images/lisp-styles.jpg)


这是一个很老的笑话了：某黑客从美国国防部某个机密系统里拿到了一份源码，不过由于时间有限，只有最后几页，黑客想好歹仔细分析也有用，然而打开后就精神崩溃了——

### C

结构化

Linux基金会


### JavaScript

当然JavaScript也是，不过它是一门没有经过深思熟虑设计出来的语言：

![Terrible JavaScript](./images/terrible-javascript.png)

Most Popular Language

$$$$$$$$$$$$$$$$$$$$$$

jQuery -> Angular.js -> React -> Vue.js

### Scala

Scalar

### Go

Google的Go 原本是要叫Goooooooooogle后来太长了就变成Go了

安德森說到了
“googol”一詞，指的是10的100次冪（方），寫出的形式為數字1後跟100個零，可用來代表在互聯網上可以獲得的海
量的資源。

### PHP

PHP原本是用于作个人首页，还有一些不法份子用于拍xx


### Perl

> 如果你给一百万只猴子每人一台电脑让它们在上面敲字儿.
> 最终会有一只猴子能写出一段Java程序来,
> 其余的猴子写出来的都是Perl代码.

问：如何得到一段随机字符串？
答：读取一个perl脚本

http://stackoverflow.com/questions/234075/what-is-your-best-programmer-joke?sort=votes&page=1




### 二进制和汇编

这个世界上最初的编程语言就是1和0了，他们也是所有现有的编程语言的一个结局。毕竟计算机世界里的数字都要被转换为1和0，。

如将八进制的31转换为十进制就会得到25，这就是为什么OCT 31=DEC 25。

[^xml]: 可扩展标记语言（英语：Extensible Markup Language，简称：XML），是一种标记语言。标记指计算机所能理解的信息符号，通过此种标记，计算机之间可以处理包含各种信息的文章等。来自维基百科: [https://zh.wikipedia.org/wiki/XML](https://zh.wikipedia.org/wiki/XML)

网站是如何构建的
===

生活中的程序
===

软件是如何开发出来的
===
