# python 虚拟环境的下载及配置

## Windows  虚拟环境的下载及配置

1,在命令行工具中输入 pipv install virtualenv  下载python的虚拟环境

2,创建虚拟环境:  virtualenv  wanggang(虚拟环境名称)         ,virtualenv   是在当前文件下创建虚拟环境.

3,在命令行工具中输入:  cd wanggang (切换到wanggang)   再输入 cd Scripts(切换到Scripts)

4,执行启动文件,在命令行工具中输入: activate  (或者输入:activate.bat)

5退出虚拟环境:,在命令行工具中输入: deactivate(或者输入deactivate.bat)

6,查看虚拟环境名称,在命令行工具中输入: workon

7, 连接: https://blog.csdn.net/fcy8023/article/details/82764396





## 使用jupyter时的一些提前准备

1,打开命令行工具在你想要使用的地址安装虚拟环境: 可以在你的文件夹下打开cmd,  然后在里面输入:  virtualenv  wg(虚拟环境名)

2, 命令行工具中输入: cd/wg/Scripts

3,启动文件进入虚拟环境: 命令行工具中输入:activate

4, 安装需要用到的包: pip install numpy pandas matplotlib scipy pillow -i https://pypi.douban.com/simple

5,       -i https://pypi.douban.com/simple    豆瓣源

6,在当前的虚拟环境下输入: pip install jupyter -i https://pypi.douban.com/simple

7, 解决jupyter连接不上服务器的问题

安装完jupyter, 在虚拟环境中启动完,  打开文件时发现连接不上服务器,那是因为  prompt-toolkit 对应的版本不对  升级一下版本就可以了

(ERROR: jupyter-console 6.1.0 has requirement prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0, but you'll have prompt-toolkit 1.0.5 which is incompatible.
ERROR: ipython 7.13.0 has requirement prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0, but you'll have prompt-toolkit 1.0.5 which is incompatible.)

参考网站(https://blog.csdn.net/wushiqi11/article/details/101945085)

8,解决matplotlib画图显示汉字的问题:  输入代码;

```python
from pylab import mpl
mpl.rcParams['font.sans-serif'] = ['SimHei']
```



## Tableau安装

1, 网站: https://www.jianshu.com/p/763c10c4fdc0 