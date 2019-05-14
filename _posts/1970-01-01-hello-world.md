---
title: Hello World !!!
layout: post
comments: true
language: chinese
usemath: true
category: [misc]
keywords: hello world,示例,sample,markdown
description: 简单记录一下一些与 Markdown 相关的内容，包括了一些使用模版。
---

[TOC]

***

## 1、重要链接

### 1.1、Typora

1. []:

Typora官网下载地址：<https://typora.io/> 、[帮助文档](https://support.typora.io/)
Pandoc下载地址：<http://pandoc.org/installing.html>
Markdown 语法说明：<https://www.appinn.com/markdown/index.html>
pandoc下载地址：<http://pandoc.org/installing.html>
[Typora Markdown 手册](https://www.jianshu.com/p/b30955885e6d "未读")、[Typora学习笔记](https://wenku.baidu.com/view/0b88b7c618e8b8f67c1cfad6195f312b3169eb6a.html)
[Typora软件学习总结（这里以Mac版的为例）](https://blog.csdn.net/wwWFrank2/article/details/52801127)
[Markdown中数学公式整理](https://blog.csdn.net/zdk930519/article/details/54137476)
[Markdown官网](https://daringfireball.net/)
[markdown官方指导 ](http://www.markdown.cn/#overview/)
[CSDN：Markdown博客专栏](https://blog.csdn.net/testcs_dn/column/info/markdown)
[Typora的使用](https://blog.csdn.net/qq_27035123/article/details/77574030?locationNum=3&fps=1)

扩展链接：
[美化Typora的中文字体，让编辑简书成为一种享受](https://www.jianshu.com/p/5634b207d516)

[steemit](https://steemit.com/cn/@jubi/typora-typora-tutorial-font-color)

### 1.2、YAML-Front Matter

[**Front-matte**](http://wiki.jikexueyuan.com/project/hexo-document/front-matter.html)

### 1.3、CSS（Cascading Style Sheets）层叠样式表

[系统学CSS](http://www.divcss5.com/)  、

## 2、Typora使用说明

### 2.1、基本markdown语法

#### 2.1.1、基本操作

1. 显示特殊符号：（1）转义符‘\··*’  \* ；（2）字符 `*字符串*`

2. *斜体*或_斜体_ CTRL+i、**粗体** CTRL+b、~~删除线~~ ALT+SHIFT+5、<u>下划线</u> CTRL+U、==高亮==、`<center>居中</center>`

3. ***或--- + Enter （顶端处为front matte，其他处为分割线）

4. 列表：

   （1）无序：-、+、*之一+空格（2）有序：数字+“.”+空格
   （3）任务：-[空格]空格 文字   （4）任务列表 

   - [ ] a task list item
   - [ ] incomplete
   - [x] completed

5. 分级标题：几个#后+空格+标题，或者CTRL+数字；CTRL+"+/-"调级；生成目录：[TOC]+Enter 引用：

6. 引用：">"后加引文 或者 CTRL+SHIFT+Q

> 上一级引用
>
> > 下一级引用

7. 超链接：

（1）、行内式：[百度搜索](www.baidu.com) 或 [百度搜索]<www.baidu.com>、CTRL+L

（2）、参考式：常用的网站：[百度搜索][1]、[Google][ ]

[1]:<www.baidu.com> "百度搜索"
[Google]: www.google.com "Google搜索"

（3）、URL/自动链接式：[百度搜索]<www.baidu.com 或者<www.baidu.com>
（4）、内部链接：

8. 插入图片（直接拖动到指定位置即可或者CTRL+SHIFT+i、[链接](https://support.typora.io//Images/)）
   行内式：`![alt text](/path/to/img.jpg "Title")` 或者 `![alt text](www.***.jpg "Title")`
   参考式：`![alt text][id]` 、`[id]: /path/to/img.jpg "Title"`
   **配置相关**：
   STEP1: File>Preferences..>Images Insert
   ![3](img.assets/3.png)
   STEP2：Edit>Image Tools > when Insert Local Image> Copy Image File to Floder.

9. 插入图表：CTRL+T
   ypora支持[sequence](https://link.jianshu.com/?t=https://bramp.github.io/js-sequence-diagrams/), [flowchart](https://link.jianshu.com/?t=http://flowchart.js.org/) 和 [mermaid](https://link.jianshu.com/?t=https://knsv.github.io/mermaid/#mermaid)，可以在设置中启用此功能。详情请看[document](https://link.jianshu.com/?t=http://support.typora.io/Draw-Diagrams-With-Markdown/)

10. 插入ex/LaTeX公式：创建行内公式（**Alt+Shift+M**），例如 $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$。或块级公式**Ctrl+Shift+M**：

  					$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

11. 插入表情 : （两边两个:号） :happy:、:weary: 、:cry:

12. 上标（H^2^O 、下标（H~2~O）、注释/注脚（[^注释ID]）

13. 代码块（\`\`\`+语言+Enter）、流程图（\`\`\`flow）和时序图（\`\`\`sequence）

    ```python
    @requires_authorization 代码块
    def somefunc(param1='', param2=0):
        return (param2 - param1 + 1) or None
    class SomeClass:
    ```

    ```flow
    st=>start: Start "流程图"
    e=>end
    op=>operation: My Operation
    cond=>condition: Yes or No?
    
    st->op->cond
    cond(yes)->e
    cond(no)->op
    ```

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks  时序图
Bob-->Alice: I am good thanks!
```

	**详见**：流程图[语法](http://flowchart.js.org/)以及 时序图[语法](http://bramp.github.io/js-sequence-diagrams/)

14. 快捷键：<https://support.typora.io/Custom-Key-Binding/>

|                |           |                |              |                    |             |
| -------------- | --------- | -------------- | ------------ | ------------------ | ----------- |
| 选中一整行     | ctrl+L    | 选中单词       | ctrl+d       | 选中相同格式的文字 | ctrl+e      |
| 跳转到文章开头 | ctrl+home | 跳转到文章结尾 | ctrl+end     | 搜索               | ctrl+f      |
| 替换           | ctrl+h    | 代码块         | ctrl+alt+f   | 删除线             | alt+shift+5 |
| 下划线         | ctrl+u    | 加粗           | ctrl+b       | 倾斜               | ctrl+i      |
| 插入链接       | ctrl+k    | 插入图片       | ctrl+shift+i | 插入表格           | ctrl+t      |
| ENTER          | 换段      | SHIFT+ENTER    | 换行         |                    |             |

     **自定义快捷键**
STEP1：打开**首选项设置**选到**高级设置**->File>Perferences>Advances Settings >Open Advanced Settings
STEP2：打开 用户配置文件 **conf.user.json**
STEP3： // Custom key binding, which will override the default ones. 下方加自定义快捷键

#### 2.1.2、 LaTeX数学公式，

参考链接： [博客1](http://blog.sina.com.cn/s/blog_5e16f1770100fs38.html)、[博客2](https://blog.csdn.net/jyfu2_12/article/details/79207643)、[博客3](https://blog.csdn.net/u011089523/article/details/77164490)

##### 2.1.2.1、公式概要

 1. 数学公式的前后要加上 \$ 或者使用“$$”；

 2. 普通字符在数学公式中含义一样。若要在数学环境中表示这些符号、需在个字符前加上\；

 3. 用 \^ 来表示上标，用 \_ 来表示下标，内容多于一个字符，注意用 { } 把上标括起来；例如：
     $\sum_{i=1}^n a_i=0$、$f(x)=x^{x^x}$

4. 在公式中插入文本，通过 \mbox{ } 添加text；例：$\mbox{对任意的$x>0$}, \mbox{有 }f(x)>0. $

5. 分数$\frac{1}{100}$、开方$\sqrt{x_2}$、$\sqrt[3]{x_2}$

6. “\ldots ”底线对齐、“\cdots”中线对齐的省略号 ：$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $

7. 括号和分隔符：() 和 [ ] 和｜对应于自己；{} 对应于 \{ \}；|| 对应于 \|。
     （1）当要显示**大号的括号或分隔符**时，要对应用 \left 和 \right，如：

$f(x,y,z) = 3y^2 z \left( 3 + \frac{7x+5}{1 + y^2} \right)$、$f(x,y,z) = 3y^2 z ( 3 + \frac{7x+5}{1 + y^2} )$

     （2）\left. 和 \right. 只用与匹配，本身是不显示的：$\left. \frac{du}{dx} \right|_{x=0}$、$\frac{du}{dx} |_{x=0}$

8. 多行的数学公式：$\begin{eqnarray*}\cos 2\theta & =& \cos^2 \theta - \sin^2 \theta \\
     & = & 2 \cos^2 \theta - 1.\end{eqnarray*}$  或者 $\begin{eqnarray}\cos 2\theta & =& \cos^2 \theta - \sin^2 \theta \\
     & = & 2 \cos^2 \theta - 1.\end{eqnarray}$  ?*

     其中&是对其点，表示在此对齐。使latex不自动显示序号，如果想让latex自动<u>标上序号，则把*去掉</u>

9. 矩阵：c表示向中对齐，l表示向左对齐，r表示向右对齐?
    The **characteristic polynomial** $\chi(\lambda)$ of the$3 \times 3$~matrix  $\left( \begin{array}{ccc}
    a & b & c \\
    d & e & f \\
    g & h & i \end{array} \right)$is given by the formula

  $$ \chi(\lambda) = \left| \begin{array}{rrr}
  \lambda - a & -b & -c \\
  -d & \lambda - e & -f \\
  -g & -h & \lambda - i \end{array} \right|$$

    10. 导数、极限、求和、积分(Derivatives, Limits, Sums and Integrals)

  $\frac{du}{dt} and \frac{d^2 u}{dx^2}$、 $\frac{\partial u}{\partial t}= h^2 \left( \frac{\partial^2 u}{\partial x^2}+ \frac{\partial^2 u}{\partial y^2}+ \frac{\partial^2 u}{\partial z^2}\right)$、 $\lim_{x \to \infty} \frac{3x^2 +7x^3}{x^2 +5x^4} = 3$、$\inf_{x > s}$ 

  $\sum_{k=1}^n k^2 = \frac{1}{2} n (n+1)$、 $\int_a^b f(x)\,dx$、 $\int_0^{+\infty} x^n e^{-x} \,dx = n!$、 $\int \cos \theta \,d\theta = \sin \theta$$\int_{x^2 + y^2 \leq R^2} f(x,y)\,dx\,dy= \int_{\theta=0}^{2\pi} \int_{r=0}^R f(r\cos\theta,r\sin\theta) r\,dr\,d\theta$、$\int_0^R \frac{2x\,dx}{1+x^2} = \log(1+R^2)$

  $\int_0^1 \! \int_0^1 x^2 y^2\,dx\,dy$、$\int_0^1 \int_0^1 x^2 y^2\,dx\,dy$、$\int \!\!\! \int_D f(x,y)\,dx\,dy$、$\int \int_D f(x,y)\,dx\,dy$、例子：

       One would typeset this in LaTeX by typing In non-relativistic wave mechanics, the wave function$\psi(\mathbf{r},t)$ of a particle satisfies the Schr\"{o}dinger Wave Equation。$i\hbar\frac{\partial \psi}{\partial t} = \frac{-\hbar^2}{2m} \left(\frac{\partial^2}{\partial x^2}+ \frac{\partial^2}{\partial y^2}+ \frac{\partial^2}{\partial z^2}\right) \psi + V \psi$
It is customary to normalize the wave equation by demanding that $\int \!\!\! \int \!\!\! \int_{\textbf{R}^3} \left| \psi(\mathbf{r},0) \right|^2\,dx\,dy\,dz = 1$
        A simple calculation using the Schr wave equation shows that$\frac{d}{dt} \int \!\!\! \int \!\!\! \int_{\textbf{R}^3} \left| \psi(\mathbf{r},t) \right|^2\,dx\,dy\,dz = 0$
  and hence  $\int \!\!\! \int \!\!\! \int_{\textbf{R}^3} \left| \psi(\mathbf{r},t) \right|^2\,dx\,dy\,dz = 1$. for all times~$t$. If we normalize the wave function in this way then, for any (measurable) subset~$V$ of $\textbf{R}^3$ and time~$t$,$\int \!\!\! \int \!\!\! \int_V \left| \psi(\mathbf{r},t) \right|^2\,dx\,dy\,dz$ represents the probability that the particle is to be found within the region~$V$ at time~$t$.

累乘 $\prod{x}$、$\prod_{n=1}^{99}{x_n}$

##### 2.1.2.2、希腊字母（Greek Letter）

|    lower    |    default    |  upper   |  default   |      \mathbf      |      \mathit      |
| :---------: | :-----------: | :------: | :--------: | :---------------: | :---------------: |
|   \alpha    |   $\alpha$    |    A     |    $A$     |                   |                   |
|    \beta    |    $\beta$    |    B     |    $B$     |                   |                   |
|   \gamma    |   $\gamma$    |  \Gamma  |  $\Gamma$  | $\mathbf \Gamma$  | $\mathit \Gamma$  |
|   \delta    |   $\delta$    |  \Delta  |  $\Delta$  | $\mathbf \Delta$  | $\mathit \Delta$  |
|  \epsilon   |  $\epsilon$   |    E     |    $E$     |                   |                   |
| \varepsilon | $\varepsilon$ |          |            |                   |                   |
|    \zeta    |    $\zeta$    |    Z     |    $Z$     |                   |                   |
|    \eta     |    $\eta$     |    H     |    $H$     |                   |                   |
|   \theta    |   $\theta$    |  \Theta  |  $\Theta$  | $\mathbf \Theta$  | $\mathit \Theta$  |
|  \vartheta  |  $\vartheta$  |          |            |                   |                   |
|    \iota    |    $\iota$    |    I     |    $I$     |                   |                   |
|   \kappa    |   $\kappa$    |    K     |    $K$     |                   |                   |
|   \lambda   |   $\lambda$   | \Lambda  | $\Lambda$  | $\mathbf \Lambda$ | $\mathit \Lambda$ |
|     \mu     |     $\mu$     |    M     |    $M$     |                   |                   |
|     \nu     |     $\nu$     |    N     |    $N$     |                   |                   |
|     \xi     |     $\xi$     |   \Xi    |   $\Xi$    |   $\mathbf \Xi$   |                   |
|  \omicron   |  $\omicron$   |    O     |    $O$     |                   |                   |
|     \pi     |     $\pi$     |   \Pi    |   $\Pi$    |   $\mathbf \Pi$   |   $\mathit \Pi$   |
|   \varpi    |   $\varpi$    |          |            |                   |                   |
|    \rho     |    $\rho$     |          |            |                   |                   |
|   \varrho   |   $\varrho$   |          |            |                   |                   |
|   \sigma    |   $\sigma$    |  \Sigma  |  $\Sigma$  | $\mathbf \Sigma$  | $\mathit \Sigma$  |
|  \varsigma  |  $\varsigma$  |          |            |                   |                   |
|    \tau     |    $\tau$     |    T     |    $T$     |                   |                   |
|  \upsilon   |  $\upsilon$   | \Upsilon | $\Upsilon$ |                   |                   |
|    \phi     |    $\phi$     |   \Phi   |   $\Phi$   |  $\mathbf \Phi$   |  $\mathit \Phi$   |
|   \varphi   |   $\varphi$   |          |            |                   |                   |
|    \chi     |    $\chi$     |    X     |    $X$     |                   |                   |
|    \psi     |    $\psi$     |   \Psi   |   $\Psi$   |  $\mathbf \Psi$   |  $\mathit \Psi$   |
|   \omega    |   $\omega$    |  \Omega  |  $\Omega$  | $\mathbf \Omega$  | $\mathit \Omega$  |
|             |               |          |            |                   |                   |
|             |               |          |            |                   |                   |

#### 2.1.2.3、运算符


|             |           |              |            |              |            |
| :---------: | :-------: | :----------: | :--------: | :----------: | :--------: |
|  $\coprod$  |  \coprod  |  $\bigvee$   |  \bigvee   | $\bigwedge$  | \bigwedge  |
| $\biguplus$ | \biguplus |  $\bigcap$   |  \bigcap   |  $\bigcup$   |  \bigcup   |
|  $\intop$   |  \intop   |    $\int$    |    \int    |   $\prod$    |   \prod    |
|   $\sum$    |   \sum    | $\bigotimes$ | \bigotimes | $\bigoplus$  | \bigoplus  |
| $\bigodot$  | \bigodot  |   $\oint$    |   \oint    | $\bigsqcup$  | \bigsqcup  |
| $\smallint$ | \smallint |    $\pm$     |    \pm     |   $\times$   |   \times   |
|   $\cdot$   |   \cdot   |    $\div$    |    \div    |    $\neg$    |    \neg    |
|  $\equiv$   |  \equiv   |    $\leq$    |    \leq    |    $\geq$    |    \geq    |
|  $\forall$  |  \forall  |   $\infty$   |   \infty   | $\emptyset$  | \emptyset  |
|  $\exists$  |  \exists  |   $\nabla$   |   \nabla   |    $\bot$    |    \bot    |
|  $\angle$   |  \angle   |  $\because$  |  \because  | $\therefore$ | \therefore |
|    $\mp$    |    \mp    |   $\ngeq$    |   \ngeq    |  $\not\geq$  |  \not\geq  |
|   $\neq$    |   \neg    |  $\approx$   |  \approx   |              |            |
|             |           |              |            |              |            |
|             |           |              |            |              |            |



&copy;     版权  ，  &reg;    注册商标 ，&trade;    商标，&nbsp;  空格 &amp;      和号 &quot;     引号 &apos;     撇号 &lt;       小于号 &gt;      大于号 &ne;        不等号 &le;      小于等于 &ge;      大于等于 &cent;     分 &pound;    磅 &euro;     欧元 &yen;      元 &sect;     节 &times;     乘号 &divide;    除号 &plusmn;    正负号

### 2.2、HTML特殊字符编码对照表

[对照表链接](https://www.jb51.net/onlineread/htmlchar.htm)

| 特殊符号 | 命名实体 | 十进制编码 | 特殊符号 | 命名实体   | 十进制编码 | 特殊符号 | 命名实体  | 十进制编码 |
| -------- | -------- | ---------- | -------- | ---------- | ---------- | -------- | --------- | ---------- |
| Α        | &Alpha;  | &#913;     | Β        | &Beta;     | &#914;     | Γ        | &Gamma;   | &#915;     |
| Δ        | &Delta;  | &#916;     | Ε        | &Epsilon;  | &#917;     | Ζ        | &Zeta;    | &#918;     |
| Η        | &Eta;    | &#919;     | Θ        | &Theta;    | &#920;     | Ι        | &Iota;    | &#921;     |
| Κ        | &Kappa;  | &#922;     | Λ        | &Lambda;   | &#923;     | Μ        | &Mu;      | &#924;     |
| Ν        | &Nu;     | &#925;     | Ξ        | &Xi;       | &#926;     | Ο        | &Omicron; | &#927;     |
| Π        | &Pi;     | &#928;     | Ρ        | &Rho;      | &#929;     | Σ        | &Sigma;   | &#931;     |
| Τ        | &Tau;    | &#932;     | Υ        | &Upsilon;  | &#933;     | Φ        | &Phi;     | &#934;     |
| Χ        | &Chi;    | &#935;     | Ψ        | &Psi;      | &#936;     | Ω        | &Omega;   | &#937;     |
| α        | &alpha;  | &#945;     | β        | &beta;     | &#946;     | γ        | &gamma;   | &#947;     |
| δ        | &delta;  | &#948;     | ε        | &epsilon;  | &#949;     | ζ        | &zeta;    | &#950;     |
| η        | &eta;    | &#951;     | θ        | &theta;    | &#952;     | ι        | &iota;    | &#953;     |
| κ        | &kappa;  | &#954;     | λ        | &lambda;   | &#955;     | μ        | &mu;      | &#956;     |
| ν        | &nu;     | &#957;     | ξ        | &xi;       | &#958;     | ο        | &omicron; | &#959;     |
| π        | &pi;     | &#960;     | ρ        | &rho;      | &#961;     | ς        | &sigmaf;  | &#962;     |
| σ        | &sigma;  | &#963;     | τ        | &tau;      | &#964;     | υ        | &upsilon; | &#965;     |
| φ        | &phi;    | &#966;     | χ        | &chi;      | &#967;     | ψ        | &psi;     | &#968;     |
| ω        | &omega;  | &#969;     | ϑ        | &thetasym; | &#977;     | ϒ        | &upsih;   | &#978;     |
| ϖ        | &piv;    | &#982;     | •        | &bull;     | &#8226;    | …        | &hellip;  | &#8230;    |
| ′        | &prime;  | &#8242;    | ″        | &Prime;    | &#8243;    | ‾        | &oline;   | &#8254;    |
| ⁄        | &frasl;  | &#8260;    | ℘        | &weierp;   | &#8472;    | ℑ        | &image;   | &#8465;    |
| ℜ        | &real;   | &#8476;    | ™        | &trade;    | &#8482;    | ℵ        | &alefsym; | &#8501;    |
| ←        | &larr;   | &#8592;    | ↑        | &uarr;     | &#8593;    | →        | &rarr;    | &#8594;    |
| ↓        | &darr;   | &#8595;    | ↔        | &harr;     | &#8596;    | ↵        | &crarr;   | &#8629;    |
| ⇐        | &lArr;   | &#8656;    | ⇑        | &uArr;     | &#8657;    | ⇒        | &rArr;    | &#8658;    |
| ⇓        | &dArr;   | &#8659;    | ⇔        | &hArr;     | &#8660;    | ∀        | &forall;  | &#8704;    |
| ∂        | &part;   | &#8706;    | ∃        | &exist;    | &#8707;    | ∅        | &empty;   | &#8709;    |
| ∇        | &nabla;  | &#8711;    | ∈        | &isin;     | &#8712;    | ∉        | &notin;   | &#8713;    |
| ∋        | &ni;     | &#8715;    | ∏        | &prod;     | &#8719;    | ∑        | &sum;     | &#8722;    |
| −        | &minus;  | &#8722;    | ∗        | &lowast;   | &#8727;    | √        | &radic;   | &#8730;    |
| ∝        | &prop;   | &#8733;    | ∞        | &infin;    | &#8734;    | ∠        | &ang;     | &#8736;    |
| ∧        | &and;    | &#8869;    | ∨        | &or;       | &#8870;    | ∩        | &cap;     | &#8745;    |
| ∪        | &cup;    | &#8746;    | ∫        | &int;      | &#8747;    | ∴        | &there4;  | &#8756;    |
| ∼        | &sim;    | &#8764;    | ≅        | &cong;     | &#8773;    | ≈        | &asymp;   | &#8773;    |
| ≠        | &ne;     | &#8800;    | ≡        | &equiv;    | &#8801;    | ≤        | &le;      | &#8804;    |
| ≥        | &ge;     | &#8805;    | ⊂        | &sub;      | &#8834;    | ⊃        | &sup;     | &#8835;    |
| ⊄        | &nsub;   | &#8836;    | ⊆        | &sube;     | &#8838;    | ⊇        | &supe;    | &#8839;    |
| ⊕        | &oplus;  | &#8853;    | ⊗        | &otimes;   | &#8855;    | ⊥        | &perp;    | &#8869;    |
| ⋅        | &sdot;   | &#8901;    | ⌈        | &lceil;    | &#8968;    | ⌉        | &rceil;   | &#8969;    |
| ⌊        | &lfloor; | &#8970;    | ⌋        | &rfloor;   | &#8971;    | ◊        | &loz;     | &#9674;    |
| ♠        | &spades; | &#9824;    | ♣        | &clubs;    | &#9827;    | ♥        | &hearts;  | &#9829;    |
| ♦        | &diams;  | &#9830;    |          | &nbsp;     | &#160;     | ¡        | &iexcl;   | &#161;     |
| ¢        | &cent;   | &#162;     | £        | &pound;    | &#163;     | ¤        | &curren;  | &#164;     |
| ¥        | &yen;    | &#165;     | ¦        | &brvbar;   | &#166;     | §        | &sect;    | &#167;     |
| ¨        | &uml;    | &#168;     | ©        | &copy;     | &#169;     | ª        | &ordf;    | &#170;     |
| «        | &laquo;  | &#171;     | ¬        | &not;      | &#172;     |          | &shy;     | &#173;     |
| ®        | &reg;    | &#174;     | ¯        | &macr;     | &#175;     | °        | &deg;     | &#176;     |
| ±        | &plusmn; | &#177;     | ²        | &sup2;     | &#178;     | ³        | &sup3;    | &#179;     |
| ´        | &acute;  | &#180;     | µ        | &micro;    | &#181      | "        | &quot;    | &#34;      |
| <        | &lt;     | &#60;      | >        | &gt;       | &#62;      | '        |           | &#39;      |


## 3、扩展进阶

1. 字体设置： <font face="微软雅黑" size=12 color=#FF0000 >微软雅黑字体</font>

2. 背景颜色： 

   <table><tr><td bgcolor=orange><center>背景色是：orange</center></td></tr></table>

3. 分割线：你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线

4. 跳转链接
    <a href="http://askunix.top/" target="_blank">跳到自己博客列表</a>
    跳到自己博客列表：<a href="http://askunix.top/" target="_blank">http://askunix.top/</a>

5. 普通标题

   <h1 align = "center">这是居中标题</h1>
6. 插入图片及图片居中、定义大小
<div align="center">
<img src="http://pp.myapp.com/ma_pic2/0/shot_42391053_1_1488499316/550" height="330" width="190" >
<img src="http://pp.myapp.com/ma_pic2/0/shot_42391053_2_1488499316/550" height="330" width="190" >
<img src="http://pp.myapp.com/ma_pic2/0/shot_42391053_3_1488499316/550" height="330" width="190" > 
 </div>
7. 插入音乐
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=330 height=86 src="//music.163.com/outchain/player?type=2&id=528478901&auto=1&height=66"></iframe>
8. 插入视频
<iframe width="560" height="315" src="https://www.youtube.com/embed/Ilg3gGewQ5U" frameborder="0" allowfullscreen></iframe>

<iframe width="854" height="480" src="https://www.youtube.com/embed/SJldOOs4vB8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

9. MarkDown的[公式撰写](https://www.jianshu.com/p/df6a136d06d8)，可以考虑使用WORD原始公式撰写，使用[**Writage-1.12**](http://www.writage.com/)转换。表格可以使用[TableGenerate](http://www.tablesgenerator.com/)转换。

10. MarkDown链接打开本地文件操作：

    - 方法一： <a href="./typoraManual.assets/3.png"> 链接  </a>
    - 方法二： [链接 ](./typoraManual.assets/3.png) ， [链接 ](./typoraManual.assets/3.png)
11. <span style="font-size:14px;">filepath = uigetdir('*.*','请选择文件夹');%fliepath为文件夹路径</span>

[^注释ID]: 注释在本页最下方！

12. Typora如何设置字体颜色/Typora tutorial: Font color



|                                          |                                      |                                        |                                              |                                              |                                     |                                            |
| :--------------------------------------: | ------------------------------------ | -------------------------------------- | -------------------------------------------- | -------------------------------------------- | ----------------------------------- | ------------------------------------------ |
| $\textcolor{GreenYellow}{GreenYellow} $  | $\textcolor{Yellow}{Yellow}$         | $\textcolor{Goldenrod}{Goldenrod} $    | $\textcolor{Dandelion}{Dandelion}$           | $\textcolor{Apricot}{Apricot} $              | $\textcolor{Peach}{Peach}$          | $\textcolor{Melon}{Melon} $                |
| $\textcolor{YellowOrange}{YellowOrange}$ | $\textcolor{Orange}{Orange} $        | $\textcolor{BurntOrange}{BurntOrange}$ | $\textcolor{Bittersweet}{Bittersweet}$       | $\textcolor{RedOrange}{RedOrange} $          | $\textcolor{Mahogany}{Mahogany}$    | $\textcolor{Maroon}{Maroon} $              |
|     $\textcolor{BrickRed}{BrickRed}$     | $\textcolor{Red}{Red} $              | $\textcolor{OrangeRed}{OrangeRed}$     | $\textcolor{RubineRed}{RubineRed}$           | $\textcolor{WildStrawberry}{WildStrawberry}$ | $\textcolor{Salmon}{Salmon}$        | $\textcolor{CarnationPink}{CarnationPink}$ |
|     $\textcolor{Magenta}{Magenta} $      | $\textcolor{VioletRed}{VioletRed}$   | $\textcolor{Rhodamine}{Rhodamine} $    | $\textcolor{Mulberry}{Mulberry}$             | $\textcolor{RedViolet}{RedViolet} $          | $\textcolor{Fuchsia}{Fuchsia}$      | $\textcolor{Lavender}{Lavender} $          |
|      $\textcolor{Thistle}{Thistle}$      | $\textcolor{Orchid}{Orchid} $        | $\textcolor{DarkOrchid}{DarkOrchid}$   | $\textcolor{Purple}{Purple} $                | $\textcolor{Plum}{Plum}$                     | $\textcolor{Violet}{Violet} $       | $\textcolor{RoyalPurple}{RoyalPurple}$     |
|   $\textcolor{BlueViolet}{BlueViolet}$   | $\textcolor{Periwinkle}{Periwinkle}$ | $\textcolor{CadetBlue}{CadetBlue}$     | $\textcolor{CornflowerBlue}{CornflowerBlue}$ | $\textcolor{MidnightBlue}{MidnightBlue}$     | $\textcolor{NavyBlue}{NavyBlue} $   | $\textcolor{RoyalBlue}{RoyalBlue}$         |
|        $\textcolor{Blue}{Blue} $         | $\textcolor{Cerulean}{Cerulean}$     | $\textcolor{Cyan}{Cyan} $              | $\textcolor{ProcessBlue}{ProcessBlue}$       | $\textcolor{SkyBlue}{SkyBlue} $              | $\textcolor{Turquoise}{Turquoise}$  | $\textcolor{TealBlue}{TealBlue} $          |
|   $\textcolor{Aquamarine}{Aquamarine}$   | $\textcolor{BlueGreen}{BlueGreen} $  | $\textcolor{Emerald}{Emerald}$         | $\textcolor{JungleGreen}{JungleGreen}$       | $\textcolor{SeaGreen}{SeaGreen} $            | $\textcolor{Green}{Green}$          | $\textcolor{ForestGreen}{ForestGreen}$     |
|   $\textcolor{PineGreen}{PineGreen} $    | $\textcolor{LimeGreen}{LimeGreen}$   | $\textcolor{YellowGreen}{YellowGreen}$ | $\textcolor{SpringGreen}{SpringGreen}$       | $\textcolor{OliveGreen}{OliveGreen}$         | $\textcolor{RawSienna}{RawSienna} $ | $\textcolor{Sepia}{Sepia}$                 |
|       $\textcolor{Brown}{Brown} $        | $\textcolor{Tan}{Tan}$               | $\textcolor{Gray}{Gray} $              | $\textcolor{Black}{Black}$                   |                                              |                                     |                                            |
|                                          |                                      |                                        |                                              |                                              |                                     |                                            |

数学/方程式颜色设置：$ \textcolor{red}{\int_a^b}\textcolor{blue}{f(x)}\textcolor{green}{dx}\textcolor{brown}{=c}​$

13. [Typora 修改中文字体](https://link.jianshu.com/?t=http://andour.me/2017/04/08/Typora-%E4%BF%AE%E6%94%B9%E4%B8%AD%E6%96%87%E5%AD%97%E4%BD%93.html)： 在 body{ } 里的 font-family 后添加 ,'微软雅黑'（不识别）。**注意！**不要修改 @font-face{ }中的 font-family，仅修改在 body{ } 中的。[ref](https://www.jianshu.com/p/5634b207d516)