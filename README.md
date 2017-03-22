# 基于按键的OLED显示控制

本项目是采用Ti公司的TMS320F28027板为基础实现基于按键的LED显示控制

> 关于TMS320F28027芯片板的介绍请查看  *tms320f28027介绍.pdf*

## 概述

项目的核心设计在于按键与*OLED*的设计，F28027只有一个按键可以控制，设计实现按键单击与长按的判断，扩展按键功能，*OLED*控制通过相应的函数显示汉字与字符。通过长按实现*LED*灯的流水灯与呼吸灯（***PWM***产生）的控制，通过单击实现时钟，计时器，***MCU***温度监控的功能的切换。通过***SCI***实时将温度通过串口传输得到PC。
   计时模块可通过单击启动，再次单击暂停，再次单击复位。温度监控模块可显示当前MCU实时温度。还有自***MCU***运行后的历史最高温度与最低温度。*LED*模式可实现两种不同形式流水灯与呼吸灯之间的切换。

## 结构

![QQ截图20170322221753](C:\Users\kejie\Pictures\截图\git素材\QQ截图20170322221753.png)
