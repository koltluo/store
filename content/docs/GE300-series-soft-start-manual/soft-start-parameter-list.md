---
linktitle: 软启动参数明细表
title: 软启动参数一览表
weight: 9
math: true
---
## A基本参数表


| 序号    |  参数名称   |  参数范围   |  默认值   |  备注   | 属性    |
| --- | --- | --- | --- | --- | --- |
|  1   |  控制方式   |  0：禁止启停</br>1：键盘单独控制 </br>2：外控单独控制</br> 3：键盘+外控</br> 4：通讯单独控制 </br>5：键盘+通讯 </br>6：外控+通讯</br>7：键盘+外控+通讯    |  3：键盘+外控   |     |  ✅   |
|  2   |   起动方式  |  0：限流起动</br>1：电压斜坡起动 </br>2：保留</br>3：突跳电压斜坡起动   |   0：限流起动   |     |  ✅   |
|  3   |  起动限流百分比   |  50%~600%   |  300%    |     |  ✅   |
|  4   |   起始电压百分比  |   10%~80%   |   35%   |     |   ✅  |
|  5   |  电压斜坡起动时间   |   1s~120s    |  15s   |     |  ✅   |
|  6   |  突跳电压   |  10%~95%   |   80%   |     |  ✅   |
|  7   |  突跳时间   |   10ms~2000ms  |   500ms   |     |  ✅   |
|  8   |  停止模式   |   0：自由停车</br>1：软停车   |  0：自由停车   |     |  ✅   |
|  9   |   软停时间  |    1s~60s  |   5s   |     |  ✅   |
|  10   |  软起动器类型   |   0:在线型 </br>1:旁路型   |   1:旁路型  |     |  ✅   |


✅：表示该参数的设定值在软启动器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在软启动器处于运行状态时，不可更改；   
❎：表示该参数的数值是实际检测记录值，不能更改；  


## B保护参数一览表

| 序号    |  参数名称   |  参数范围   |  默认值   |  备注   | 属性    |
| --- | --- | --- | --- | --- | --- |
|  1   |  起动过载等级   |  0~30  |  10   | 0：关闭  |  ✅   |
|  2   |   运行过载等级 |  0~30   |   10  |  0：关闭   |  ✅   |
|  3   |  运行过流倍数   |  0%-600%   |  0%    |  0：关闭   |  ✅   |
|  4   |   运行过流保护时间  |   0s-6000s   |   5s    |     |   ✅  |
|  5   |  过压保护值   |    100%~140%   |  120%   |  100：关闭   |  ✅   |
|  6   |  过压保护时间  |   1s~60s  |   5s   |     |  ✅   |
|  7   |  欠压保护值   |   60%-100%  |   80%   |  100：关闭   |  ✅   |
|  8   |  欠压保护时间   |   1s~60s   |  5s   |     |  ✅   |
|  9   |   三相不平衡度  |    20%~100%  |   40%   |  100：关闭   |  ✅   |
|  10   |  三相不平衡时间   |    0.1s~60.0s   |    10.0s  |     |  ✅   |
|  11   |  起动超时时间   |    0s~150s |   60s   |   0：关闭   |  ✅   |
|  12   |  点动超时时间   |    0s~150s   |  Os   |   0：关闭   |  ✅   |
|  13   |   欠载保护值  |     0%~100%  |   0%   |   0：关闭   |  ✅   |
|  14   |  欠载保护时间   |    1s~60s   |   10s  |     |  ✅   |

✅：表示该参数的设定值在软启动器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在软启动器处于运行状态时，不可更改；   
❎：表示该参数的数值是实际检测记录值，不能更改；  






## C高级功能一览表


| 序号    |  参数名称   |  参数范围   |  默认值   |  备注   | 属性    |
| --- | --- | --- | --- | --- | --- |
|  1   |  可编程继电器1   |  功能：</br>0：不动作 </br>1：上电动作</br>2：软起中动作 </br>3：旁路动作 </br>4：软停中动作 </br>5：点动中动作 </br>6：运行时动作 </br>7：待机动作 </br>8：故障动作</br>9：晶闸管击穿动作    |  8：故障动作   |     |  ✳️   |
|  2   |   可编程输出延时1  |  0-600s   |   0s   |     |  ✳️   |
|  3   |  可编程继电器2   |  功能：</br>0：不动作 </br>1：上电动作</br>2：软起中动作 </br>3：旁路动作 </br>4：软停中动作 </br>5：点动中动作 </br>6：运行时动作 </br>7：待机动作 </br>8：故障动作</br>9：晶闸管击穿动作    |  6：运行时动作   |     |  ✳️   |
|  4   |   可编程输出延时2  |   0-600s   |   0s   |     |   ✳️  |
|  5   |  通讯地址   |   1-127    |  1   |     |  ✳️   |
|  6   |  通讯波特率   |   0:2400</br> 1:4800</br> 2:9600</br> 3:19200  |   2:9600  |     |  ✳️  |
|  7   |  A相电流校准值   |   10%~1000%  |   100%   |     |  ✳️  |
|  8   |  B相电流校准值   |   10%~1000%  |  100%   |  ✳️   |
|  9   |   C相电流校准值  |    10%~1000% |   100%   |     |  ✳️   |
|  10   |  输入电压校准值   |   10%~1000%   |   100%  |     |  ✳️   |
|  11   |  4-20mA下限校准   |   0%~150.0%  |   20.0%  |     |  ✳️   |
|  12   |  4-20mA上限校准   |   0%~150.0%   |  100%    |     |  ✳️   |
|  13   |   4-20mA上限电流  |    50%~500% |   200%   |     |  ✳️   |


✅：表示该参数的设定值在软启动器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在软启动器处于运行状态时，不可更改；   
❎：表示该参数的数值是实际检测记录值，不能更改；  


  


     





## D状态信息一览表



| 序号    |  参数名称   |  参数范围   |  默认值   |  备注   | 属性    |
| --- | --- | --- | --- | --- | --- |
|  1   |  软起额定电流   |      |     |     |  ❎   |
|  2   |   软起额定电压  |     |     |     |  ❎   |
|  3   |  电机额定电流   |  10-1600A   |     |     |  ✳️   |
|  4   |   软起起动次数  |      |     |     |   ❎  |
|  5   |  累计运行小时   |       |     |     |  ❎   |
|  6   |  主控软件版本   |    |      |     |  ❎   |


✅：表示该参数的设定值在软启动器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在软启动器处于运行状态时，不可更改；   
❎：表示该参数的数值是实际检测记录值，不能更改；  





## E显示参数一览表

| 序号    |  参数名称   |  参数范围   |  默认值   |  备注   | 属性    |
| --- | --- | --- | --- | --- | --- |
|  1   | 待机显示模式| 0：模式0 </br>1：模式1    |   0：模式0  |     |  ✳️   |
|  2   |   运行显示模式  | 0：模式0 </br>1：模式1   |    0：模式0   |     |  ✳️   |
|  3   |  操作语言选择  |  0：英语  </br>1：中文   |  1：中文     |     |  ✳️  |
|  4   |   屏幕保护时间  |   0s~1800s |   120s   |  0：不保护   |   ✳️  |
|  5   |  键盘软件版本   |       |     |     |  ❎   |
|  6   |  屏幕对比度   |    |      |     |  ❎  |


✅：表示该参数的设定值在软启动器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在软启动器处于运行状态时，不可更改；   
❎：表示该参数的数值是实际检测记录值，不能更改；  


