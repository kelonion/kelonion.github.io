---
title: "如何在macOS上安装matplotlib字体"
date: 2019-05-10
categories:
  - Tutorial
tags:
  - Matplotlib
---
## 1. 下载安装字体
由于matplotlib只支持.ttf格式的字体，所以需要先在网上下载相应格式的字体并安装。
我个人比较喜欢方正的字体，所以选择了[方正黑体](http://www.foundertype.com/index.php/FontInfo/index.html?id=131)（方正已支持个人非商业免费使用字体了）
下载完成后双击即可安装。
安装完成后会自动打开Font Book（或自行打开，点击左边栏中的User）, 记下该字体在Font Book中的名字。（注意不是字体文件的名字，比如兰亭黑体的字体文件名为`FZHTJW.TTF`，但字体在系统中的名字为`FZHei-B01S`）
## 2. 修改matplotlib配置
### 2.1 简单修改方案
```python
import matplotlib.pyplot as plt
plt.rcParams['font.sans-serif'] = ['FZHei-B01S'] # 填写该字体的名称
```
如果仍然没有效果可以尝试重置一下：
```python
from matplotlib.font_manager import _rebuild
_rebuild()
```
这个方法需要在每次运行matplotlib的时候都加上这段代码来更换字体，如果想要直接更换默认字体则可以选择另一种方案。
## 2.2 永久修改方案
首先找到matplotlib中管理默认配置的文件**matplotlibrc**，一般存放在：
`/Users/{你的用户名}/anaconda3/lib/python3.7/site-packages/matplotlib/mpl-data/`
双击打开后，找到`font.sans-serif`，删掉前面的`#`，并在后面添加字体的名词：
```
原配置文件中显示：
#font.sans-serif: DejaVu Sans, Bitstream Vera Sans

修改为：(把字体添加到最前面)
font.sans-serif: FZHei-B01S, DejaVu Sans, Bitstream Vera Sans
```