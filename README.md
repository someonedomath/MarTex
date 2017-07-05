# MarTex简介

若要使用 MarTex, 你需要准备如下的工具:

- 一台 Mac 电脑. 
- 在 Mac 上安装好 [Pandoc](http://pandoc.org) 和 [Mactex](https://www.tug.org/mactex/).
- 用 MarkDown 写好一篇学术文章. 这里安利下 [Typora](https://typora.io), 是一款很好用的 MarkDown 编辑器.

如果你从没有用过 MarTex, 可以先下载 [example.md](https://raw.githubusercontent.com/someonedomath/MarTex/master/example.md), 作为第一次使用的实验对象. 
你可以在 .md 文件的任意部位插入 latex 指令, 方法是使用 "[MarkDown 代码块](http://xianbai.me/learn-md/article/extension/code-blocks-and-highlighting.html)".
这是因为 MarTex 在转换你的 .md 文件时候, 会把所有代码块中的文本, 识别为 latex 指令.

接下来可以使用 MarTex 了! 

先使用下面的指令来初始化程序

```bash
source <(curl -s https://raw.githubusercontent.com/someonedomath/MarTex/master/init.sh)
```

使用下面的指令将一个 markdown 文件转化为一个 tex 文件

```bash
MarTex YourMardkdownFile
```

使用下面的指令将一个  tex 文件编译为 pdf 文件

```tex
TexPdf YourTexFile
```

使用下面的指令将一个 markdown 文件先运行 MarTex 再运行 TexPdf

```bash
MarPdf YourTexFile
```

