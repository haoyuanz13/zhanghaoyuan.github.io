---
layout: post
comments: true
categories: tools
---
[TOC]

# 步骤

## 0.前提准备

* 装好了lua

## 1. 安装NppExec插件

(1)菜单栏->插件->Plugin Manager->Show Plugin Manager

(2)按键盘NppExec，会检索到这个插件

(3)安装重启





## 2. 配置命令

(1)按F6

(2)拷贝下面命令到对话框中，修改lua.exe为自己的安装路径，注意：lua.exe的路径有空格要用双引号括起来


	"D:\Program Files (x86)\lua-5.1.5_Win32_bin\lua.exe" "$(FULL_CURRENT_PATH)" & PAUSE & EXIT

(3)点击save...，存一个名字，例如：run_lua
(4)测试：点击运行，看一下下方有没有lua执行的输出，如果有就表示命令配置ok了

## 3. 添加命令

菜单栏->插件->NppExec->Advanced Options
![参考图片](http://o856moet9.bkt.clouddn.com/lua_config.jpg)

(1)Associated script选择刚才保存的脚本名字，run_lua

(2)可省略。在Item name下面输入一个名字，也可以直接用现有的名字run_lua

(3)点击Add/Modify按钮，这个时候可以看到最上方里面多了一个run_lua::run_lua

## 4. 修改快捷键：菜单栏->运行->管理快捷键

（1）删除现有的F5快捷键，标签页Main menu中找一下

（2）在标签页Plugin commands中找到cmd_lua，把快捷键修改为F5

## 5. 运行：按F5可以看到下方有输出结果，大功告成！