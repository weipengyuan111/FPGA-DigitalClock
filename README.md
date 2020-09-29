# FPGA-DigitalClock

## 一、介绍

### 选题原因

受到电脑开机长时间不操作会进入屏幕保护模式影响，并且会显示时间等信息，就打算做一个拥有屏幕保护多功能控制的数字钟。

### 主要功能

在VGA上显示时间/温度与湿度。具体的显示效果受声音传感器、板子上的开关与板子上显示时间的影响。

### 设计思路

采用自顶而下再自下而上的数字系统设计方法。首先划分子模块系统，数字钟模块，温湿度传感器模块，声音传感器控制模块，VGA显示模块，再根据每个模块的需要，向下一级划分。最后将它们同类归并整合，在顶层模块连接。

## 二、参考

[【接口时序】7、VGA接口原理与Verilog实现](https://www.cnblogs.com/liujinggang/p/9690504.html)(我确实是照着这篇博客才最终将VGA配置成功)

[[Verilog]实现数字钟(自动计时+手动校时+倒计时+设置闹钟)附完整源代码](https://blog.csdn.net/qq_41683065/article/details/94645628)

[字模提取软件的使用(pctolCD2002,基于FPGA的VGA显示汉字)](https://blog.csdn.net/cchulu/article/details/74923526)
