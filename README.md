UCASthesis：https://github.com/xiaoyao9933/UCASthesis
本模板在UCASthesis基础上做了少量修改,适用于中国科学院武汉物理与数学研究所学位论文

修改说明：
ucasthesis.cfg
%中国科学院武汉物理与数学研究所论文原创性声明和使用授权说明

ucasthesis.cls
%格式修改：中英文封面，原创性声明和使用授权说明，致谢，摘要

cover.tex
%单位为中国科学院武汉物理与数学研究所

abs.tex
%增加单独一个摘要文件

main.tex
%将致谢放在摘要之前


FAQ
===
[使用前必读的问题](https://github.com/xiaoyao9933/UCASthesis/wiki)

What's it?
==========

UCASThesis is a LaTeX thesis template package for University of Chinese Academy of Sciences in order to
make it easy to write thesises for either master or doctor. This template pacagge is derived from the 
ThuThesis.

UCASThesis 是中国科学院大学学位论文 LaTeX 模板，支持硕士、博士论文格式。该模板基于清华大学ThuThesis二次开发。
本模板目前已经针对中国科学院计算技术研究所的论文模板进行调整，但由于中科院各院所的模板规范并非完全一致，
其余院所的同学可能需要进行一些必要的修改。

版权须知
========
Copyright (C) 2005-2013 by Xue Ruini <xueruini@gmail.com>
Copyright (C) 2013-2016 derived by Chaolu <wuchaolu@gmail.com>

This file may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either version 1.3a
of this license or (at your option) any later version.
The latest version of this license is in:

http://www.latex-project.org/lppl.txt

and version 1.3a or later is part of all distributions of LaTeX
version 2004/10/01 or later.

使用须知
========

1. 本模板强烈建议使用texlive 2014或以上版本、MikTex2.9或以上版本编译，***请不要使用CTEX***。
  
  特别注意的是， CTEX 可能由于内置宏包老旧，暂时无法支持 UCASThesis 模板，随之可能会产生"ifxetex","zhnumber.sty not found"等问题。

2. 确定系统中存在xfig，transfig依赖(Mac OSX 系统可尝试通过port进行安装)。

3. 确保当前系统已安装配置SimSun，SimHei，KaiTi，FangSong字体，如果您使用的是Linux和Mac OSX系统，请自行
以“fc-cache 添加 win 字体”为关键字通过Google搜索解决方案)。
备用方案：如果您并不想安装其他字体，而仅使用系统自带的兼容字体（不建议这样做），则可利用以下命令交互式地完成字体配置

    python zhfonts.py

使用方法
========
1. 编译示例文档
   xelatex main
   bibtex main
   xelatex main
   xelatex main

   说明：也可以使用 pdflatex/latex+dvipdfmx 生成文档。

2. 编写自己的论文
   参考示例文档：
     main.tex   主控文档
     data/      论文具体内容
     ref/       参考文献目录
     figures/   图片目录
   

如何获取/升级
=============
1. 如需以git方式获取，git clone https://github.com/xiaoyao9933/UCASthesis
2. 如需直接获取压缩包文件，请下载 https://github.com/xiaoyao9933/UCASthesis/archive/master.zip
3. 建议通过git pull方式更新模板，如果你之前已经完成论文的一部分写作，则可以通过下载新版模板包里的ucasthesis.cls、ucasthesis.cfg以及ucasthesis.dtx文件，替换至你的论文目录中完成模板更新；也可以通过下载新版模板后，拷贝入含有写作内容的main.tex,data/figures/ref目录进行更新。





