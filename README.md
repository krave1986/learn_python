# learn_python

python 学习笔记

## 退出 python launcher

ctrl + z
或
quit()
或
exit()

## 列出虚拟环境中所安装的依赖
pip list --local

## 创建虚拟环境
py -3 -m venv .venv

## 激活虚拟环境
.venv\scripts\activate

## 退出虚拟环境
deactivate

## pip文档的阅读方式
在使用 vs code 的时候，帮我安装了 black 格式化工具，但是下载的命令里，用到了
pip install -U black
不明白 -U 是什么意思，就查询了一番，发现python的包管理工具 pip 隶属于 PyPA 。
https://www.pypa.io/en/latest/
而 pip 的文档又在它的子页面：
https://pip.pypa.io/en/stable/
如果要查命令的话，根据常识会去reference-guide
不过真正要找到 pip install 的 flag ，
还要去看 pip install 的参考页面：
https://pip.pypa.io/en/stable/reference/pip_install/

## black的缩进方式
black使用，且只使用 4个空格 的缩进方式。
所以，你在使用vscode的时候，需要勾选 editor.insertSpaces 选项。
不然你按tab的时候，会真实地插入一个 tab ，
而你的其它代码可能已经被 black 改成4个空格，如此，缩进对不上，就会导致看不见原因的报错。

但是，因为我这边同时要写 js 代码 和 python 。
在 js 测，使用 Prettier ，已经实现了代码的 tab 缩进。
如果又要写 python 的话，那么 editor.insertSpaces 选项就要频繁切换。
目前的一个解决方式是，依赖选项：editor.detectIndentation 来自动进行切换。

目前来看的话，这个选项还是相对可靠的。


