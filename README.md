![cover](./Supplemental/cover.png)

# 使用Typora代替LaTex编写论文

本项目的初衷是为了简化中国大陆本科生**小型通识课论文**（或**实小型验报告**）撰写的负担。我已将其修改为**天津大学论文模板**所需样式，但大部分同学都可以自行在 CSS 中修改适合自己学校的格式。

markdown 的轻量化特性，使您可以专注于论文内容而不用担心格式。书写时仅通过简单的标记，并通过替换样例模板中的个人信息，您就可以输出媲美卷王由LaTeX​排版的精美论文与报告。

这是一个 Typora 的 markdown 主题样式，该主题理论上适用于所有平台，CSS 也适用于部分其他编辑器。macOS 和 Windows 中的个别特性可能不同。

## 预览

[天津大学封面样式预览](Supplemental/tju-cover-template.pdf)

[论文样式预览](Supplemental/essay-template.pdf)

![天津大学本科毕业论文封面](image/cover_1.jpg)

### 封面，摘要和关键词

| ![sample-essay_1](https://gitee.com/Keldos-Li/picture/raw/master/img/sample-essay_1.png) | ![sample-essay_2](https://gitee.com/Keldos-Li/picture/raw/master/img/sample-essay_2.png) |
| :----------------------------------------------------------: | :----------------------------------------------------------: |

### 预览与编写

| ![preview-l](https://gitee.com/Keldos-Li/picture/raw/master/img/preview-l.png)|![preview-d](https://gitee.com/Keldos-Li/picture/raw/master/img/preview-d.png)|
| :----: | :----: |
| ![edit-l](https://gitee.com/Keldos-Li/picture/raw/master/img/edit-l.png)|![edit-d](https://gitee.com/Keldos-Li/picture/raw/master/img/edit-d.png)|

#### 层级标题 

|![heading-l](https://gitee.com/Keldos-Li/picture/raw/master/img/heading-l.png)|![](https://gitee.com/Keldos-Li/picture/raw/master/img/heading-d.png)|
| :----: | :----: |

```markdown
层级标题：

### 标题3

#### 标题4

##### 标题5

###### 标题6
```

#### 表格 
|![table-l](https://gitee.com/Keldos-Li/picture/raw/master/img/table-l.png)|![table-d](https://gitee.com/Keldos-Li/picture/raw/master/img/table-d.png)|
| :----: | :----: |

```markdown
表格：

<center><strong>表 2  全球/中国桌面操作系统市场份额占比（%）</strong></center>

| OS   | Windows | macOS | Unknown | Linux | Chrome OS | 其他 |
| ---- | ------- | ----- | ------- | ----- | --------- | ---- |
| 全球 | 76.56   | 17.1  | 2.68    | 1.93  | 1.72      | 0.01 |
| 中国 | 87.55   | 5.44  | 6.24    | 0.75  | 0.01      | 0.01 |
```

#### 项目列表
|![item-l](https://gitee.com/Keldos-Li/picture/raw/master/img/item-l.png)|![item-d](https://gitee.com/Keldos-Li/picture/raw/master/img/item-d.png)|
| :----: | :----: |

```markdown
项目列表：

1.  有序列表项
2.   有序列表项2
    +   无序列表项1
    +   无序列表项2. 
        *   [x] 表示已完成。 ***==(请尽量不要使用此功能，因为它的对齐效果不佳)==***
        *   [ ] 表示未完成。

*   项目1 
    *   项目2 
        *   项目3 

1. 项目1 
2. 项目2 
    1. 项目2.1 
    2. 项目2.2 
        1. 项目2.2.1 
        2. 项目2.2.2
```

#### 代码块 
|![code-l](https://gitee.com/Keldos-Li/picture/raw/master/img/code-l.png)|![code-d](https://gitee.com/Keldos-Li/picture/raw/master/img/code-d.png)|
| :----: | :----: |

```markdown
代码块

​```html

<!DOCTYPE html>
<html>
<body>

<h1>The *= Operator</h1>

<p id="demo"></p>

<script>
var x = 10;
x *= 5;
document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>
​```
```

#### Mermaid
|![mermaid-l](https://gitee.com/Keldos-Li/picture/raw/master/img/mermaid-l.png)|![mermaid-d](https://gitee.com/Keldos-Li/picture/raw/master/img/mermaid-d.png)|
| :----: | :----: |

```markdown
mermaid 图形

​```mermaid
graph LR
A(开始) -->
input[/输入a,b/] --> if{a%b=0 ?}
if --->|yes| f1[GCD = b] --> B(结束)
if --->|no| f2["a, b = b, a % b "]-->if
​```
```

#### 公式

|![equation-l](https://gitee.com/Keldos-Li/picture/raw/master/img/equation-l.png)|![equation-d](https://gitee.com/Keldos-Li/picture/raw/master/img/equation-d.png)|
| :----: | :----: |

```markdown
公式:

$$
\iint\limits_{x^2 + y^2 \leq R^2} f(x,y)\,\mathrm{d}x\,\mathrm{d}y = \int_{\theta=0}^{2\pi} \mathrm{d}\theta\int_{r=0}^R f(r\cos\theta,r\sin\theta) r\,\mathrm{d}r\, \tag{1}
$$
```

#### 其他

还有支持其他语法特性功能，这里不再展示，请参考Typora的语法库。

## 安装

*   安装前，请确保您已经安装 Typora 或其他 markdown 编辑器（也可以用某些 IDLE），并拥有基本的 markdown 语法知识；

    *   [如果您没有](#什么是typora)

*   最简单的安装办法是在该GitHub页面的右侧找到最新的（或较早的正式版）release，然后下载`Source code (zip)`；
    release中包含了单独的`.css`样式文件，如果您不需要字体文件和样例文件，可以仅下载它们，这会大大减小下载大小。
    
    *   当然你也可以使用命令行下载最新的打包代码（虽然没用，只是可能酷一点？）：
    
    ```bash
    $ cd <你常用的下载文件夹>
    $ git clone https://github.com/Keldos-Li/typora-latex-theme.git
    ```
    
*   解压这个文件，然后将`css`文件夹中的`latex.css`和`latex-dark.css`两个文件复制到你的[Typora主题文件夹](#怎么找到typora主题文件夹)下；

*   打开`/Supplemental/Fonts`文件夹，安装[需要的字体](#该主题都包含了哪些字体)；

*   启动或重新启动Typora，然后从主题菜单中选择`Latex`或`Latex Dark`选项。

## 使用

*   在Typora的`偏好设置` – `Markdown` 中选取`保留连续的空格与单个换行` *（如果您不希望您的论文有段后的额外行距的话）*；
*   按照您学校的要求修改css文件；[（为什么？）](#为什么要修改css文件)

    *   修改CSS后请重新启动Typora以查看效果
*   `Supplemental`文件夹中的`essay-template.md`和`essay-template.pdf`展示了一篇小论文在该主题下的效果（其中文字来源于我本人的课程作业以及一些拼凑，请不要在意过多细节），其中论文封面（也单独放置在`cover-template.md`文件中）、摘要、关键词和其他一些特别的元素使用HTML代码来编写。您可以自行取用修改它们的文字内容部分和代码部分来完成您的课程论文。
    *   如果您看不懂HTML代码，请先自行百度/谷歌/必应，然后尝试联系您在计算机系的同学；
*   如果可以的话，或许您可以在论文致谢中提到这个项目。(/ω＼)

　　这本质是一个适用于所有 markdown 编辑器的 CSS 样式（但对 Typora 编辑器做了额外的优化），您也可以将其用于其他您喜欢的 markdown 编辑器的自定义样式（尚未经过完整测试）。

### 特别注意

*   PDF页面**页边距**：

    在 Windos / Linux 中，您可以很好地使用

    ```css
    @media print{
      @page{
        margin: 1.8cm 2cm 1.2cm 2cm !important; 
        /* 按次序为 上 右 下 左 的页边距 */
      }
    }
    ```

    来更改打印 PDF 的页边距。
    
    但对于 macOS 用户，因为 [Typora 本身的问题](https://github.com/typora/typora-issues/issues/998)，暂时不能使用这一方法调整页边距。
    
    *   可以在 Typora 的导出设置里重新设置自定义页边距。
    *   或先导出为 html ，然后在 Chrome 中打开打印。
        <br>（不能用 Safari！Safari 会自行设置它认为的最小边距，这会导致您无法精确控制页边距；另一方面，在某次更新后 Safari 取消了对 CSS 本地字体读取的支持（理由是隐私问题），会导致您无法显示很多字体！）
    *   或者直接用 pandoc 的命令行设置。

*   **超链接**：

    显然，我们不希望打印的论文存在蓝色的超链接（？），我在 CSS 中修改了部分代码，使得在页面编辑和导出html预览中可以得到正常的超链接样式，但打印时会取消颜色和下划线（仍可以点击链接）。

    不知道大家是否有这个需求，如果有更合适的方法可以联系我。

*   **多级列表**：

    因为我的技术原因，请暂时不要在**二级有序列表**之后**混用** *有序列表* 和 *无序列表* 以及*核对清单*，会出现一些 bug。（虽然感觉会这么干的人应该不多。）如果您有解决方案，请联系我。

*   **页眉和页脚**：

    目前似乎不能直接定义，请在 Typora 的导出设置里设置好您需要的页眉和页脚文字，导出后在 PDF 编辑器中调整您喜欢的样式风格。

*   **引用参考文献**

    目前没有更好的方式，请您主动编号……（或许小型课程论文不需要大量参考文献。）

*   **专注模式**和**打字机模式**：

    还没写这部分的代码。本主题样式初衷不在于此，如果您有需求，可以提交 issue 或进入讨论区讨论，我视需求和精力再进行开发。

## Q&A

### 什么是**Typora**？

[Typora](https://typora.io/) 是一个超级好用的实时预览markdown编辑器；

### 什么是**markdown**？

[markdown](https://daringfireball.net/projects/markdown/) 是一种轻量级标记语言，用于使用纯文本创建格式化文本。
约翰·格鲁伯和亚伦·斯沃茨于2004年创建了 Markdown，作为一种以源代码形式吸引人类读者的标记语言。
Markdown 排版语法简洁，让人们更多地关注内容本身而非排版。它可与 HTML 混编，可导出 HTML、PDF 以及本身的 .md 格式等文件。
Markdown 广泛用于博客、即时消息、在线论坛、协作软件、文档页面和阅读文件。

参考：

*    [Markdown中文语法简介](https://markdown.com.cn/)
*    [Typora使用的markdown语法参考](https://support.typora.io/Markdown-Reference/)

### 怎么找到Typora主题文件夹？

*   从`文件` – `偏好设置`中打开设置面板，然后单击“打开主题文件夹”即可。

*   如果您需要手动打开，对于 Windows / Linux，这个文件夹一般是`C:\Users\{username}\AppData\Roaming\Typora\themes\`；对于 macOS，这个文件夹一般是`/Users/{username}/Library/Application Support/abnerworks.Typora/themes/`。

### 该主题都包含了哪些字体？

字体文件都存放在`/Supplemental/Fonts`文件夹。

具体请参阅[这里](./Supplemental/Fonts/)。

*   **所有的字体文件请自行获取授权**，本人不对您使用字体造成的法律纠纷负责。

### 为什么要修改CSS文件？

每个学校所要求的格式略有不同，尽管老师不会肉眼查看您的格式是否符合要求，但或许您为了自己的需要仍需要稍作修改，例如加大字体、行间距和页边距使得论文显得更长。

尽管 Typora 不希望您直接编辑您下载的主题文件，但我暂时推荐您**直接修改**我们的样式文件，得以充分达到自定义的效果，我为此写了大量的注释。

*   在当前版本中设置点较为分散，我后期应该会将设置点整合到`:root`设置中，届时您将可以直接在 CSS 样式表的最顶端修改。但目前，您不得不记住所有您更改过的位置，并在获取我们之后的更新后重新修改一遍（对不起！🙇🏻）

#### 我该如何修改CSS文件？

*   确保您电脑中拥有**文本编辑软件**，如*记事本*（Windows）或*文本编辑*（macOS），如果有代码编辑软件就更好了。如果双击 CSS 文件无法打开，请在系统让您选取应用程序时选取上述软件；
    *   *绝对不要用 Microsoft Word 打开它！！！就算它可以！*
*   根据代码中的注释提示修改源代码中样式选择器的变量取值；
*   如果您看不懂注释，或不知道修改代码会造成什么效果，请先自行百度/谷歌/必应，然后尝试联系我。

### 该主题不能满足我的需求？

该样式只能作为**轻量级**排版输出，如果您需要更复杂的排版，请使用 LaTeX 或 Word 进行排版。

*   [天津大学LaTex模板](https://github.com/xnth97/TJUThesisLatexTemplate)



## 反馈

- 为该仓库提issue或者提出PR
- 联系本人

## 说明

- 本人二次开发将其修改成天津大学论文模板样式，如有问题请提issue或者PR或者直接联系本人

已知的bug: 

- 无编号项目列表有很大的bug！！在二级项目之后，你不能混用有序列表和无序列表！因为全都是重新定义的content，我不能理解它为什么会对子项目产生影响！！可恶！
- 当行间代码太长跨页的时候好像也会有点问题，到时候再改……
- mermaid字体无法修改，我找遍了mermaid的最新文档和Typora的其他样式资源都没找到这个应该怎么在CSS样式表里修改……呜呜呜。

## 帮助

### Word字体与HTML字体对照

| word字字号 | word字体值（pt） | CSS字体值（px） |
| ---------- | ---------------- | --------------- |
| 初号       | 44pt             | 58.6px          |
| 小初       | 36pt             | 48px            |
| 一号       | 26pt             | 34.6px          |
| 小一       | 24pt             | 32px            |
| 二号       | 22pt             | 29.3px          |
| 小二       | 18pt             | 24px            |
| 三号       | 16pt             | 21.3px          |
| 小三       | 15pt             | 20px            |
| 四号       | 14pt             | 18.6px          |
| 小四       | 12pt             | 16px            |
| 五号       | 10.5pt           | 14px            |
| 小五       | 9pt              | 12px            |
| 六号       | 7.5pt            | 10px            |
| 小六       | 6.5pt            | 8.6px           |
| 七号       | 5.5pt            | 7.3px           |
| 八号       | 5pt              | 6.6px           |



## 鸣谢

该项目最初来自于知乎作者 @让幻想飞 （清华大佬，没想到和我一样年轻，但可能不喜欢及时回消息\_(:з」∠)\_）

他的原注释：

> 这篇样式基于知乎大佬LAN DU的样式，
>
> 原文知乎链接：https://zhuanlan.zhihu.com/p/158767474
>
> GitHub链接：
> https://github.com/du33169/typora-theme-essay_cn
>
> 主要改动：
>
>  - 适配LaTeX的字体。选用像LaTeX的字体是装“哔”的重要手段。
>
>  - 更改标题、目录和大纲的编号样式。改成1. ，1.1 ， 1.1.1 ，……这样的编号更有一种浓厚的论文感觉。
>
>  - 二级及以下标题全部靠左，适应文章样式。后面加上大空白，适配LaTeX样式
>     
>  不足之处：
>     
>  - 仍然无法添加页眉页脚。
>     适用于小论文、实验报告等对格式要求较松的情况，在不写代码的前提下装“哔”

@让幻想飞 的**知乎文章地址**：https://zhuanlan.zhihu.com/p/357096043

**GitHub项目地址**: https://github.com/yfzhao20/Typora-markdown
