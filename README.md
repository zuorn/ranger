# Ranger 配置 

![](https://tva1.sinaimg.cn/large/008eGmZEly1gmy1m52qdfj31aq0u07ah.jpg)


## 安装

通过 brew 安装 ranger

```
brew install ranger
```

## 配置
生成配置文件（仅第一次使用）

```
ranger --copy-config=all
```

将会在~/.config/ranger目录输出以下文件

- rc.conf - 选项设置和快捷键
- commands.py - 可以通过 `：` 执行的命令
- rifle.conf - 指定不哦提给你类型的文件默认打开程序。


## 基本用法

在 终端 执行 `ranger` 来启动 ranger

- ？ 打开帮助手册或列出快捷键、命令以及设置项
- l ，renurn 打开文件
- j，k 上下选择当前目录中的文件
- h 切换到上层目录
- [] 上层目录上移和下移
- yy , dd 复制，粘贴

知道这些基本的操作就可以直接上手了，然后可根据官方文档及说明文档来配置适合自己的操作。

## 其他配置
- 启动图片预览  
在 ~/.config/ranger/rc.conf 添加(如果你用 iterm2 的话)
```
set preview_images true
set preview_images_method w3m
set preview_images_method iterm2
```

- 显示文件夹图标
在 ~/.config/ranger/rc.conf 添加以下内容：
```
default_linemode devicons
```

## 其他配置参考：
- 自定义键位绑定：https://github.com/ranger/ranger/wiki/Keybindings
- 自定义命令：https://github.com/ranger/ranger/wiki/Keybindings

### 其他参考官方文档： https://github.com/ranger/ranger/wiki/Official-User-Guide
