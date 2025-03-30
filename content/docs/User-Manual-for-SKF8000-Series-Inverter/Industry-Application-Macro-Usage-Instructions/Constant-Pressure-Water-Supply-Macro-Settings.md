---
title: 6.2 恒压供水宏
toc: true
weight: 2
next: /docs/user-manual-for-skf8000-series-inverter/industry-application-macro-usage-instructions/machine-tool-macro-settings/
prev: /docs/user-manual-for-skf8000-series-inverter/industry-application-macro-usage-instructions/restore-to-factory-settings/
---

{{< callout type="info" >}}
  小提示：1bar=1kg=0.1MPa=10米汞柱
{{< /callout >}}

本恒压力供水宏特点：直接选择供水宏，再输入传感器量程值和目标压力，其它参数基本上不动就能直接实现高效的恒压供水控制，调压能力强大，反应迅速灵敏，因此比传统的PID控制频率方式的供水控制更优秀，压力更稳定，更节能等优点。同时对有压力罐的现场有更好的恒压保压效果。以及主板双继电器直接实现一拖三，或配合Y1和HDO端子外接继电器控制最多可实现一拖五供水，有独立的加泵和减泵压力以及延时控制，还可以实现超压力时，备用紧急的减泵专用时间控制，只要适当减小(b0-15压力上限紧急减辅泵延时)的时间值，即可快速减泵并停机，合理避免水压上升太快的难题。另外，键盘可以通过移位键切换直接监视压力设定目标值，或压力反馈值。掉电后重新上电后运行时，监视内容不变。同时本机还直接支持双显键盘监视压力设定值以及反馈值。

## 单泵变频恒压力供水宏
P0-29=1时，其自动初始化参数如下：（默认面板电位器给定目标压力值）  
P0-01=2，P0-02=1，P0-03=8，P0-14=20.00Hz，P4-18=2.00，P7-03=8015，P7-04=0001，P7-05=3003，P7-17=15，P7-18=16，PA-00=3，PA-05=50.0，PA-06=0.10，PA-28=0（如果加快反应速度，可以增大PA-05和减小PA-06的值；减慢反应速度，这两参数反之），AI1默认为0~10V输入作为PID压力反馈源，如果需要改为4~20mA输入，请补充参数：P4-13=2.00V，P4-37=11(个位设1为电流输入型)。变频器本身出厂AI2默认为0~20MA输入，如果使用AI2作为PID压力反馈源，对应补充参数：P4-18=2.00V，P4-37=10即可。AI1和AI2改为电流输入时，需要串接端子24V为传感器供电。  
b0组为恒压力供水参数组，其中b0-00为压力传感器的量程，需要如实输入。例如：传感器最大值标记为1.6MPa，则b0-00=16.00kg。   
PA-00用于选定目标压力给定源默认是3键盘模拟电位器，如果选为8即由b0-01为供水现场的目标压力值设定，默认为5.00kg，可按需求更改。休眠和唤醒压力以及相关的延时可以调整，休眠，唤醒以及各种压力偏差量，都是自动跟随着目标压力的百分比值联动自动适应调整，基本上不需要调节就能稳定工作。  
注意：关于恒压供水的变频器相关接线，请点[这里](/docs/user-manual-for-skf8000-series-inverter/panel-display-and-operation/terminal-application-wiring-diagram/ "变频恒压供水接线图")，不在此叙述。  
## 一拖三变频恒压力供水宏
P0-29=2，即可实现1变频泵拖2工频泵的恒压供水模式。此模式基于上面的**单泵变频恒压力供水宏**的初始化默认参数条件下，增加如下默认参数：  
P5-02=50(RLY1为辅助泵1)，P5-03=51(RLY2为辅助泵2)，P5-25=0.3s，P5-26=0.3s，b0-10=2(两个辅助泵)，更多控制参数请看[恒压供水参数b0组](/docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/intelligent-constant-pressure-water-supply-parameters/ "变频恒压供水参数设置")   
## 一拖五变频恒压力供水宏
P0-29=3，即可实现1变频泵拖4工频泵的恒压供水模式。此模式基于上面的**一拖三变频恒压力供水宏**的初始化默认参数条件下，增加如下默认参数：  
P5-04=52（Y1为辅助泵3），P5-01=53(HDO为辅助泵4)，P5-00=1，P5-24=0.3s，P5-27=0.3s，b0-10=4(四个辅助泵)，更多控制参数请看[恒压供水参数b0组](/docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/intelligent-constant-pressure-water-supply-parameters/ "变频恒压供水参数设置")    
## 消防供水巡检柜专用宏
P0-29=7，些模式默认参数如下：  
P0-02=1，P0-03=0，P0-08=10.00Hz，P0-12=15.00Hz，P4-00=1，P4-03=9，P6-10=1

探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}

  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
