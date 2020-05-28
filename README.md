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
