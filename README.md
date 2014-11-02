#####这是在arch中用的fvwm的配置文件

### 参考
http://box-look.org/content/show.php/Lethe?content=91022

### 软件列表
1. habak 用于改变桌面背景
2. tint2 任务管理器
3. conky 资源监视器
4. fcitx 小企鹅
5. xcompmgr 这个还没搞清楚怎么用，参照着留下来
6. xterm + roxterm + rxvt + rxvt-unicode终端安装的比较
7. pacmanfm 文件管理
8. firefox 默认浏览器
9. fvwm 2.6.5

### 安装
1. 把文件全部下载到~/.fvwm目录中
2. .xinitrc中设置XIM环境变量和启动fvwm

		export XMODIFIERS=@im=fcitx
		export XIM=fcitx
		export GTK_IM_MODULE=fcitx
		export QT_IM_MODULE=fcitx
		export XMODIFIERS=@im=fcitx
		export XIM_PROGRAM=fcitx
		exec fvwm

3. 安装字体
因为在conky中用到openlogo的字体，需要
	
		cp openlogos.ttf /usr/share/fonts/TTF/
		cd /usr/share/fonts/TTF/
		mkfontdir
		mkfontscale

### 快捷键
1. Alt + t 打开roxterm
2. Alt + f 打开firefox
3. Alt + c 打开FvwmConsle
