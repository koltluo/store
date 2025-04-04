---
title: 5.11 PA组：PID功能参数
toc: true
weight: 11
next: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/pulse-frequency-and-counting/
prev: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/malfunction-and-protection/
---
{{< callout type="info" >}}
  变频器参数属性说明
{{< /callout >}}
✅：表示该参数的设定值在变频器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在变频器处于运行状态时，不可更改；  
❎：表示该参数的数值是实际检测记录值，不能更改；


## PA组：PID功能参数

|  功能代码|    名称  | 设定范围 | 出厂值 |属性 | DEC地址 |
| :----: |    :----   | :----   | :----:   | :----:   | :----:   |
|  PA-00|    PID给定源  | 0：PA-01设定</br>1：AI1 </br>2：AI2</br>3：AI3外引键盘电位器</br>4：HDI输入脉冲设定（X5）</br>5：通讯给定</br>6：多段指令给定</br>7：由供水组b0-01压力给定|0 | ✅ | 64000 |
|  PA-01|    PID数值给定  | 0.0~100.0% |50.0% | ✅ | 64001 |
|  PA-02|    PID反馈源  | 0：AI1</br>1：AI2 </br>2：AI3外引键盘电位器</br>3：AI1-AI2</br>4：HDI输入脉冲设定（X5）</br>5：通讯给定</br>6：AI1+AI2</br>7：MAX(AI1,AI2)</br>8：MIN(AI1,AI2) | 0 | ✅ | 64002 |
|  PA-03|    PID作用方向  | 0：正作用</br>1：反作用 |0 | ✅ | 64003 |
|  PA-04|    PID给定反馈量程  | 0~65535 |1000 | ✅ | 64004 |
|  PA-05|    比例增益KP1  | 0.0~100.0 |20.0 | ✅ | 64005 |
|  PA-06|    积分时间Ti1  | 0.01~10.00s |2.00s | ✅ | 64006 |
|  PA-07|    微分时间Td1  | 0.000~10.000s |0.000s | ✅ | 64007 |
|  PA-08|    PID反转截止频率  |0.00~最大频率 |2.00Hz | ✅ | 64008 |
|  PA-09|    PID偏差极限  | 0.0~100.0% |0.0% | ✅ | 64009 |
|  PA-10|    PID微分限幅  | 0.00~100.00% |0.1% | ✅ | 64010 |
|  PA-11|    PID给定变化时间  | 0.00~650.00s |0.00s | ✅ | 64011 |
|  PA-12|    PID反馈滤波时间  | 0.00~60.00s |0.00s | ✅ | 64012 |
|  PA-13|    PID输出滤波时间  | 0.00~60.00s |0.00s | ✅ | 64013 |
|  PA-15|    比例增益KP2  | 0.0~100.0 |20.0 | ✅ | 64015 |
|  PA-16|    积分时间Ti2  | 0.01~10.00s |2.00s | ✅ | 64015 |
|  PA-17|    微分时间Td2  | 0.000~10.000s |0.000s | ✅ | 64017 |
|  PA-18|    PID参数切换条件  | 0：不切换</br>1：通过X端子切换</br>2：根据偏差自动切换 |0 | ✅ | 64018 |
|  PA-19|    PID参数切换偏差1  | 0.0%~PA-20 |20.0% | ✅ | 64019 |
|  PA-20|    PID参数切换偏差2  | PA-19~100.0% |80.0% | ✅ | 64020 |
|  PA-21|    PID初值  | 0.0~100.0% |0.0% | ✅ | 64021 |
|  PA-22|    PID初值保持时间  | 0.00~650.00s |0.00s | ✅ | 64022 |
|  PA-23|    两次输出偏差正向最大值  | 0.00~100.00% |1.00% | ✅ | 64023 |
|  PA-24|    两次输出偏差反向最大值  | 0.00~100.00% |1.00% | ✅ | 64024 |
|  PA-25|    PID积分属性 | 个位：积分分离</br>0：无效</br>1：有效</br>十位：输出到限值后是否停止积分</br>0：继续积分</br>1：停止积分 |00 | ✅ | 64025 |
|  PA-26|    PID反馈丢失检测值  | 0.0%：不判断反馈丢失</br>0.1~100.0% |0.0% | ✅ | 64026 |
|  PA-27|    PID反馈丢失检测时间  | 0.0s~20.0s |0.0s | ✅ | 64027 |
|  PA-28|    PID停机运算  | 0：停机不运算</br>1：停机时运算 |1 | ✅ | 64028 |



探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}

  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
