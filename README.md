# 《数据结构》课程的学习报告
2020年兰州大学数据结构课程作业

根据学校要求，笔记要以论文方式提交，故采用兰州大学本科生毕业论文的格式改写我的课堂学习笔记。

论文模板Fork至余航学长的仓库。

使用方法如下：
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [兰州大学本科生2020（学士学位）LaTeX模板](#%e5%85%b0%e5%b7%9e%e5%a4%a7%e5%ad%a6%e6%9c%ac%e7%a7%91%e7%94%9f2020%e5%ad%a6%e5%a3%ab%e5%ad%a6%e4%bd%8dlatex%e6%a8%a1%e6%9d%bf)
  - [一、使用方法](#%e4%b8%80%e4%bd%bf%e7%94%a8%e6%96%b9%e6%b3%95)
    - [现状0：以前用的这个模板，现在需要升级](#%e7%8e%b0%e7%8a%b60%e4%bb%a5%e5%89%8d%e7%94%a8%e7%9a%84%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e7%8e%b0%e5%9c%a8%e9%9c%80%e8%a6%81%e5%8d%87%e7%ba%a7)
      - [如何使用兰州大学2007老版论文要求](#%e5%a6%82%e4%bd%95%e4%bd%bf%e7%94%a8%e5%85%b0%e5%b7%9e%e5%a4%a7%e5%ad%a62007%e8%80%81%e7%89%88%e8%ae%ba%e6%96%87%e8%a6%81%e6%b1%82)
    - [现状1：论文直接用这个模板开始写](#%e7%8e%b0%e7%8a%b61%e8%ae%ba%e6%96%87%e7%9b%b4%e6%8e%a5%e7%94%a8%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e5%bc%80%e5%a7%8b%e5%86%99)
    - [现状2：以前用的LZUThesis2017](#%e7%8e%b0%e7%8a%b62%e4%bb%a5%e5%89%8d%e7%94%a8%e7%9a%84lzuthesis2017)
      - [这个项目与LZUThesis2017主要区别](#%e8%bf%99%e4%b8%aa%e9%a1%b9%e7%9b%ae%e4%b8%8elzuthesis2017%e4%b8%bb%e8%a6%81%e5%8c%ba%e5%88%ab)
      - [你需要做什么](#%e4%bd%a0%e9%9c%80%e8%a6%81%e5%81%9a%e4%bb%80%e4%b9%88)
  - [二、常见问题](#%e4%ba%8c%e5%b8%b8%e8%a7%81%e9%97%ae%e9%a2%98)
    - [1、编译出来的没有**参考文献**或**目录**，或者直接失败：](#1%e7%bc%96%e8%af%91%e5%87%ba%e6%9d%a5%e7%9a%84%e6%b2%a1%e6%9c%89%e5%8f%82%e8%80%83%e6%96%87%e7%8c%ae%e6%88%96%e7%9b%ae%e5%bd%95%e6%88%96%e8%80%85%e7%9b%b4%e6%8e%a5%e5%a4%b1%e8%b4%a5)
    - [2、正文第一章，编号却是第二章？](#2%e6%ad%a3%e6%96%87%e7%ac%ac%e4%b8%80%e7%ab%a0%e7%bc%96%e5%8f%b7%e5%8d%b4%e6%98%af%e7%ac%ac%e4%ba%8c%e7%ab%a0)
    - [3、linux环境下编译失败](#3linux%e7%8e%af%e5%a2%83%e4%b8%8b%e7%bc%96%e8%af%91%e5%a4%b1%e8%b4%a5)
    - [4、为什么中文加粗命令`\textbf{}`或者`\bfseries`都没反应？](#4%e4%b8%ba%e4%bb%80%e4%b9%88%e4%b8%ad%e6%96%87%e5%8a%a0%e7%b2%97%e5%91%bd%e4%bb%a4textbf%e6%88%96%e8%80%85bfseries%e9%83%bd%e6%b2%a1%e5%8f%8d%e5%ba%94)
    - [5、编译的和预期有差别，你把缓存的文件清理一下，重新四步走进行编译](#5%e7%bc%96%e8%af%91%e7%9a%84%e5%92%8c%e9%a2%84%e6%9c%9f%e6%9c%89%e5%b7%ae%e5%88%ab%e4%bd%a0%e6%8a%8a%e7%bc%93%e5%ad%98%e7%9a%84%e6%96%87%e4%bb%b6%e6%b8%85%e7%90%86%e4%b8%80%e4%b8%8b%e9%87%8d%e6%96%b0%e5%9b%9b%e6%ad%a5%e8%b5%b0%e8%bf%9b%e8%a1%8c%e7%bc%96%e8%af%91)
    - [6、表格居中、换页、换行、图片并列排等，怎么用](#6%e8%a1%a8%e6%a0%bc%e5%b1%85%e4%b8%ad%e6%8d%a2%e9%a1%b5%e6%8d%a2%e8%a1%8c%e5%9b%be%e7%89%87%e5%b9%b6%e5%88%97%e6%8e%92%e7%ad%89%e6%80%8e%e4%b9%88%e7%94%a8)
    - [7、其他的](#7%e5%85%b6%e4%bb%96%e7%9a%84)
  - [三、更新日志](#%e4%b8%89%e6%9b%b4%e6%96%b0%e6%97%a5%e5%bf%97)
    - [2020.5.19](#2020519)
    - [2020.5.10](#2020510)
    - [2020.4.13](#2020413)
    - [2020.4.10](#2020410)
    - [2020.4.7](#202047)
    - [2020.4.4](#202044)
  - [四、其他](#%e5%9b%9b%e5%85%b6%e4%bb%96)
    - [学校的要求有哪些变化](#%e5%ad%a6%e6%a0%a1%e7%9a%84%e8%a6%81%e6%b1%82%e6%9c%89%e5%93%aa%e4%ba%9b%e5%8f%98%e5%8c%96)
    - [项目主要文件](#%e9%a1%b9%e7%9b%ae%e4%b8%bb%e8%a6%81%e6%96%87%e4%bb%b6)
    - [编译器选择](#%e7%bc%96%e8%af%91%e5%99%a8%e9%80%89%e6%8b%a9)
    - [高级操作](#%e9%ab%98%e7%ba%a7%e6%93%8d%e4%bd%9c)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# 兰州大学本科生2020（学士学位）LaTeX模板

为什么选择这个模板？

1. 因为这是i兰大易班（兰朵儿）app的开发者制作的 ~
2. 因为这个模板经过了多人多平台测试，包括Mac、Windows、Linux三种平台
3. 因为这是目前与学校要求最为符合的一个LaTex模板
4. 因为这个项目有最为详尽的文档说明
5. 在国内[Gitee: LZUThesis2020](https://gitee.com/yuhldr/LZUThesis2020)和国外[Github: LZUThesis2020](https://github.com/yuhlzu/LZUThesis2020)开源网站同步发布，防止被墙

根据[这个项目](https://github.com/suchot/LZUThesis2017)进行修改的，mac、linux、windows三系统全部测试通过，linux缺一个字体，看[常见问题：linux环境下编译失败](#3%e3%80%81linux%e7%8e%af%e5%a2%83%e4%b8%8b%e7%bc%96%e8%af%91%e5%a4%b1%e8%b4%a5)，其他出现什么问题，也看下面的[常见问题](#%e4%b8%89%e5%b8%b8%e8%a7%81%e9%97%ae%e9%a2%98)

> 另：template.pdf和template.tex两个文件可以用来学习latex，写了点东西

我强烈建议你用git管理毕业论文，每天写完以后就提交到gitee（速度比github快无数倍）上！！！不然不小心删除了或者中病毒了什么的，哭都没地方哭去

## 一、使用方法

据说这个网站：[overleaf](https://cn.overleaf.com/)挺好用（我没用，不喜欢在线版的），可以直接直接上传这个模板，在线使用。如果你就这一次用LaTex，以后都不需要了，可以试一下，但是如果你还上研究生要发文章，还是按照下面的本地安装一下吧

### 现状0：以前用的这个模板，现在需要升级

请下载[lzubib.bst](bib/lzubib.bst)和[LZUThesis.cls](/LZUThesis.cls)，替换你论文项目中原有的这两个文件。并且开启伪加粗！

```tex
% \documentclass{LZUThesis}
% 注意2020.5.19（2.0.0）以后的版本，开启伪加粗将会非常完美！
\documentclass[AutoFakeBold]{LZUThesis}
```

**注意！**

#### 如何使用兰州大学2007老版论文要求

很多学院还是要求之前的模板，详见官网通知：[关于做好2020届本科生毕业论文（设计）工作的通知](http://jwc.lzu.edu.cn/lzupage/2020/02/25/N20200225120630.html)

如果你要用2007的模板，请下载[LZUThesis2007.cls](/LZUThesis2007.cls)，我已经适配，但是注意：

- 1、把第一行LZUThesis换成LZUThesis2007！并且开启伪加粗。

    ```tex
    % \documentclass{LZUThesis}
    % 把上面那个注释掉用2007的模板，或者改成2007的模板，注意2020.5.19（2.0.0）以后的版本，开启伪加粗将会非常完美！
    \documentclass[AutoFakeBold]{LZUThesis2007}
    ```

- 2、把成绩页放在最后！
- 3、把中文摘要放在英文摘要前面！

- 4、绪论（引言）是要再用`\Intro`这个命令，按照正文一样用章节命令！

    ```tex
    \mainmatter
    %在上面那个命令以后，注释掉  % \Intro{ 以及后面的 }
    % \Intro{
    \chapter{绪论}
        你的绪论内容
    % }
    ```

注意更新以后，请使用四步走重新编译出pdf文件

### 现状1：论文直接用这个模板开始写

**前3步详细请见[template.pdf](template.pdf)**

1. 安装texlive2020

2. 测试安装是否成功

3. 配置编译器，可见[编译器选择](#%e7%bc%96%e8%af%91%e5%99%a8%e9%80%89%e6%8b%a9)

4. texlive安装好并且把编译器配置完成后，只要把[paper.zip](paper.zip)下载然后解压就可以了，所有的都在那单独有一份，直接在那里面的`paper.tex`里写论文（很多学院还是要求之前的模板，如果你要用2007的模板，请在里面的`paper2007.tex`里写论文）


### 现状2：以前用的[LZUThesis2017](https://github.com/suchot/LZUThesis2017)

#### 这个项目与[LZUThesis2017](https://github.com/suchot/LZUThesis2017)主要区别

- lzubib.bst移动到了bib里面，并且修改了参考文献的一些问题
- 打包的里面LZUthesis.cls名字修改了
- LZU.cfg被合并到LZUthesis.cls里面了
- 适配了2020兰大毕业论文要求，并修改了他遗留下了的诸多问题！！！！！
- 文件名我看着不舒服，改成LZUThesis了，T大写

#### 你需要做什么

如果你配置好了LaTex的书写环境，先下载解压 [paper.zip](paper.zip)

模板已经适配2020，但是如果你已经写了文章，直接复制你的.tex到解压以后的文件夹里，需要你自己调整下面的：

1. 模板名字
    > 如果以前的.tex文件复制过来，必须要把前面一行名字改掉，以前是

    ```tex
    \documentclass{LZUthesis}
    % 或
    \documentclass{LZUthesisonline}
    ```

    > 注意，我的这里面 *Thesis*第一个字母大写了，不大写我看着不舒服，敲代码的人应该明白

    ```tex
    \documentclass{LZUThesis}
    ```

2. 成绩页在责任书之后，以前在前面，需要你自己移动，位置如

    ```tex
    \maketitle

    %======%
    %诚信说明页
    %授权说明书
    %======%
    \makestatement

    %=====%
    %论文（设计）成绩
    %=====%

    \supervisorcomment{导师评价你人很好}
    \recommendedgrade{80}

    \supervisorsignature{
        \raisebox{-10pt}{
            \includegraphics[width=60pt]{signature.pdf}
        }
    }

    \committeecomment{优秀}
    \finalgrade{100}
    \Grade

    % 注意成绩页在这个命令前面

    \frontmatter
    ```

3. 英文摘要请放在中文摘要前面！

4. 正文最前面有绪论（引言），模板中已经给了相关命令`\Intro`

    ```tex
    \tableofcontents
    %文章主体
    \mainmatter

    \Intro{
        这里是绪论，也可以说是引言，在LZUThesis2020.clc里面改
    }

    \chapter{latex部分用法简介}
    ```

## 二、常见问题

你可一定要先安装texlive2020，可参考[现状1：论文直接用这个模板开始写](#%e7%8e%b0%e7%8a%b61%e8%ae%ba%e6%96%87%e7%9b%b4%e6%8e%a5%e7%94%a8%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e5%bc%80%e5%a7%8b%e5%86%99)
    
### 1、编译出来的没有**参考文献**或**目录**，或者直接失败：

不要用pdflatex那个！需要四步走xelatex - bibtex - xelatex - xelatex，具体什么意思，百度吧；

### 2、正文第一章，编号却是第二章？

> 那是因为绪论当做了第一章，你可以在正文前面重新计数

```tex
%生成目录
\tableofcontents
%文章主体
\mainmatter

\Intro{
    这里是绪论

    \section{二级标题}
    绪论其实也可以有二级标题
}

% =======正文从第一章开始，需要把章节的编号归0
\setcounter{chapter}{0}

\chapter{latex部分用法简介}
```

### 3、linux环境下编译失败

> 因为linux上默认没有Arial字体

- 方法一：可以自己网上找一下，下载安装，注意名字（不是文件名，而是安装以后的字体名）要完全对上
- 方法二：可以搜索在[LZUThesis.cls](LZUThesis.cls)文件中搜索`\fontspec{Arial}`，将这一个命令删除，这个字母不用这个字体了（有点不符合论文对英摘要的要求）。

### 4、为什么中文加粗命令`\textbf{}`或者`\bfseries`都没反应？

   >2020.5.29(2.0.0)版已经解决该问题，开启伪加粗即可，详见：[现状0：以前用的这个模板，现在需要升级](#%e7%8e%b0%e7%8a%b60%e4%bb%a5%e5%89%8d%e7%94%a8%e7%9a%84%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e7%8e%b0%e5%9c%a8%e9%9c%80%e8%a6%81%e5%8d%87%e7%ba%a7)

   ~~不仅你没反应，你有没有发现“关键字”等需要宋体加粗的我用的都是黑体？你可以根据你自己的字体修改，但是对于latex中，中文加粗，大家的普遍做法都是改成黑体~~

   ~~详情查看[高级操作](#%e9%ab%98%e7%ba%a7%e6%93%8d%e4%bd%9c)~~

### 5、编译的和预期有差别，你把缓存的文件清理一下，重新四步走进行编译

缓存的文件：比如你的文件名是paper.tex，那就删除以paper开头的所有文件，当然，paper.tex不要删除！！！！

理论上是这么做的，但是你删错了不关我的事。。。

我用的sublime或者vscode点一下就删除了，好吧最多点两下，删错了，如果之前用了git的话，可以恢复

### 6、表格居中、换页、换行、图片并列排等，怎么用

你仔细看[template.pdf](template.pdf)和[template.tex](template.tex)吧，里面都有

### 7、其他的

> 百度错误的提示，基本上都能找到原因

以后再补充，如果是bugs，可以在issues里提交bugs，请**勿**直接QQ联系我！

我已经多次多人测试通过，如果你在[paper.zip](paper.zip)什么都没写，就直接编译失败的肯定是你自己的原因！！

不要用CTEX！不要用CTEX！不要用CTEX！不要用CTEX！

如：

- 没有安装或者没有成功安装texlive2020（mac是mactex），请查看：[现状1：论文直接用这个模板开始写](#%e7%8e%b0%e7%8a%b61%e8%ae%ba%e6%96%87%e7%9b%b4%e6%8e%a5%e7%94%a8%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e5%bc%80%e5%a7%8b%e5%86%99)

- vscode等编译器配置有问题，没有采用四步走，请查看：[四步走编译](#1%e7%bc%96%e8%af%91%e5%87%ba%e6%9d%a5%e7%9a%84%e6%b2%a1%e6%9c%89%e5%8f%82%e8%80%83%e6%96%87%e7%8c%ae%e6%88%96%e7%9b%ae%e5%bd%95%e6%88%96%e8%80%85%e7%9b%b4%e6%8e%a5%e5%a4%b1%e8%b4%a5)

- 不怎么懂模板，还非要乱改
- ……


-----

## 三、更新日志

### 2020.5.19

1. 新增怀旧版 [LZUThesis2007.cls](/LZUThesis2007.cls)，如何切换详见：[如何使用兰州大学2007老版论文要求](#%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8%E5%85%B0%E5%B7%9E%E5%A4%A7%E5%AD%A62007%E8%80%81%E7%89%88%E8%AE%BA%E6%96%87%E8%A6%81%E6%B1%82)
2. 修复一些细节问题，并且完美实现伪加粗，可省去高级操作！
3. 参考文献连续引用优化([1-4]，以前是[1,2,3,4]
4. 自带换页长表格，可见 [template.pdf](template.pdf)

### 2020.5.10

更新方法请查看：[现状0：以前用的这个模板，现在需要升级](#%e7%8e%b0%e7%8a%b60%e4%bb%a5%e5%89%8d%e7%94%a8%e7%9a%84%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e7%8e%b0%e5%9c%a8%e9%9c%80%e8%a6%81%e5%8d%87%e7%ba%a7)

1. 修复参考文献的历史遗留问题
2. 修复windows上目录页码显示的问题
3. 完善文档

### 2020.4.13

1. 对于宋体加粗使用了黑体，黑体加粗没有效果，做了作了说明：请看[高级操作](#%e9%ab%98%e7%ba%a7%e6%93%8d%e4%bd%9c)
2. 测试了texlive2020，适配完美
   > 2020里面可以识别`a.b.png`这样文件名的图片了，以前要写成`{a.b.}.png`，但是现在这样反而会报错
3. 修复英文摘要标题的字体问题
4. [后续计划](#%e5%90%8e%e7%bb%ad%e8%ae%a1%e5%88%92)：你们也可以提交问题修复的，开源项目一起贡献，为学弟学妹做些事。

### 2020.4.10

1. 说明：上个版本的介绍中绪论写错位置了，应在正文最前面
2. 去除雅黑字体，windows、linux、macos三合一，注意使用的时候最前面修改一下，别打我，这个以后绝对不改了

    ```tex
    % 现在应该是
    \documentclass{LZUThesis}

    % 之前是
    \documentclass{LZUThesis-mac}
    % 或
    \documentclass{LZUThesis-windows}
    ```

3. 优化封面和成绩评语界面，与word版更相似
4. 参考文献中可以由url、doi（mendeley生成的参考文献会携带），这样编译出来的pdf，点击参考文献可以直接跳转到原文界面
5. 新增 `textcomp`包，可以输入 `\textcelsius`，会变成摄氏度
6. 删除一些过时的内容，减少编译警告
7. 修改兰大logo为透明图，防止黑边
8. 以前那个库的历史遗留问题（错的地方太多了……）
   - 目录中一级标题加粗
   - 图表序号中间用点连接，序号与文字空一个字符
   - 中英文摘要字体大小、行间距等问题
   - 修复一些字号、字体设置不正确的问题

### 2020.4.7

mac版与windows分开打包，增加说明文件

### 2020.4.4 

适配了兰州大学2020最新的毕业论文（草拟稿）要求，最近还会修改

1. 页眉：单条线、页脚：页码居中
2. 封面、包括logo、和一些细节
3. 成绩表各种加黑问题，并且放在了前面
4. 添加了图片并排的一些库，里面提供了**常用的示例**
5. 针对mac电脑进行了测试和适配，修复了部分警告问题，合并一些文件，修复部分不符合论文要求的地方

------

## 四、其他


### 学校的要求有哪些变化

- 责任书有变化，模板中已经修改
- 正文页眉单线，模板中已经修改
- 封面有变化，模板中已经修改
- 成绩页提到了前面
- 英文摘要在中文摘要前面！并且摘要字体变成了2号（以前3号，我想不明白为啥要变成2号，太大了！标题都换行了，尤其是英文标题）
- 增加绪论
- 图表、目录等严格要求

### 项目主要文件

本项目精简了文件，只有LZUThesis.clc和bib、figure文件夹是必须的

1. bib文件夹里，database.bib是用来放你的参考文献的，

2. figure文件夹是一个图和导师签名

3. LZUThesis.clc这是模板配置文件，lzubib.bst是参考文献配置文件，小白请千万不要更改；

4. template.tex是用来写论文的，这个文件名字可以修改


--------

### 编译器选择

1. 不喜欢texStudio或者texmaker，用vscode吧，配置很简单，习惯sublime text3的也行

    [windows系统 vscode用法](https://zhuanlan.zhihu.com/p/38178015)

    [mac系统 vscode用法](https://www.jianshu.com/p/c09b3409317f)

    [linux系统 vscode用法](https://www.jianshu.com/p/c09b3409317f)

-------

### 高级操作

一般人，不要按照下面的操作！！！你会把模板改坏的，最后改到编译错误让你自己崩溃（改到你仰望我的LaTex水平😂，好吧，其实我也是一天学会的，不过本科阶段你们好好学习时我就折腾过……）。。。

1. 如果你觉得封面上“本科生毕业论文（设计）”和“毕业论文（设计）成绩表”这几个字的字体与学校的范例不一样（我现在用的是黑体）你可以修改LZUThesis.cls文件，把它设置成雅黑字体。windows电脑上应该是有yahei这个命令，可以直接用；linux和mac需要你自己安装字体，然后自己新建一个这样的命令。

    ```tex
    %windows系统不需要这个操作，只有linux与mac需要先百度去安装字体，再自定义如下命令

    \setCJKfamilyfont{yahei}{MicrosoftYaHei}
    \newcommand{\yahei}{\CJKfamily{yahei}}
    ```

    然后把现在设置在那几个字前面的`\heiti`改成`\yahei`

    >MicrosoftYaHei为你的字体在你电脑上上显示的名字，比如苹果电脑上：打开字体册应用，找到你自己安装的雅黑字体的PostScript名称

2. ~~成绩页等加粗字体有问题，并不是宋体加粗而是黑体！~~
   >2020.5.29(2.0.0)版已经解决该问题，开启伪加粗即可，详见：[现状0：以前用的这个模板，现在需要升级](#%e7%8e%b0%e7%8a%b60%e4%bb%a5%e5%89%8d%e7%94%a8%e7%9a%84%e8%bf%99%e4%b8%aa%e6%a8%a1%e6%9d%bf%e7%8e%b0%e5%9c%a8%e9%9c%80%e8%a6%81%e5%8d%87%e7%ba%a7)

    ~~中文在xelatex中，windows并不支持加粗命令`\textbf{}`或者`\bfseries`，为了方便和适配更多的系统，[大家一般都换成了黑体](https://www.zhihu.com/question/58456658)，我测试过打开全局伪加粗，windows并没有效果（mac和linux不打开就有效果），你要是很严谨（强迫症），可以自己安装加粗字体，自定义命令实现加粗（mac和linux用户，可以直接使用加粗的命令，会自动伪加粗，效果也不错，我就是这么用的），需要改的地方如下~~

    ~~在最新版的LZUThesis.cls文件中搜索：`应该是加粗`，可以找到应该改的地方，把这里的黑体设置，改成旁边注释括号里的要求~~

    ~~示例如下：~~

    ```tex
    原本是

    \begin{center}
        {\heiti\zihao{3}{诚信责任书}} % “诚信责任书”这几个字，应该是加粗（宋体加粗）
    \end{center}

    mac或linux可以改成伪加粗

    \begin{center}
        {\songti\bfseries\zihao{3}{诚信责任书}} % “诚信责任书”这几个字，应该是加粗（宋体加粗）
    \end{center}

    windows需要改成：

    %先百度安装字体，再在最前面合适的地方自定义加粗字体，比如你安装的字体名是：宋粗体
    \setCJKfamilyfont{csong}{宋粗体}
    \newcommand{\csong}{\CJKfamily{csong}}

    %然后修改需要修改的地方
    \begin{center}
        {\csong\zihao{3}{诚信责任书}} % “诚信责任书”这几个字，应该是加粗（宋体加粗）
    \end{center}
    ```

以上问题我在模板中没有修改的原因：

> 一个模板，对于大多数人来说，拿来就可以用（兼容性好、体验也可以）才是最重要的
，而一些细节问题，是为那些有能力（或者说爱折腾，不是贬义词）的人留下的，所以我对于遗留的问题在cls文件里，都做了注释说明

1. 如果你曾经修改过参考文献格式lzubib.bst文件，请到bib文件夹中覆盖或修改，但是我觉得我的可能更完美 ~

