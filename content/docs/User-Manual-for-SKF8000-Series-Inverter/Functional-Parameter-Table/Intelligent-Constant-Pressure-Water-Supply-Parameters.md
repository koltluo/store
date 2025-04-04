---
title: 5.17 b0组：智能恒压供水参数
toc: true
weight: 17
next: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/parameter-monitoring/
prev: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/control-optimization-parameters/
---
{{< callout type="info" >}}
  变频器参数属性说明
{{< /callout >}}
✅：表示该参数的设定值在变频器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在变频器处于运行状态时，不可更改；  
❎：表示该参数的数值是实际检测记录值，不能更改；


## b0组：智能变频恒压供水参数

|  功能代码|    名称  | 设定范围 | 出厂值 |属性 | DEC地址 |
| :----: |    :----   | :----   | :----:   | :----:   | :----:   |
|  b0-00|    压力传感器量程  | 0~99.99Bar(kg) |10.00 | ✅ | 45056 |
|  b0-01|    目标压力数字给定</br>注：目标压力由PA-01选定  | 0~99.99Bar(kg) |5.00 | ✅ | 45057 |
|  b0-02|    休眠压力  | 0~100.0%(以目标压力比例联动) |100.0% | ✅ | 45058 |
|  b0-03|    唤醒压力  | 0~100.0%(以目标压力比例联动) |95.0% | ✅ | 45059 |
|  b0-04|    压力稳定偏差量  | 0~100.0%(以目标压力比例联动) |2.0% | ✅ | 45060 |
|  b0-05|    休眠延时  | 0~6553.5s（0：关闭休眠） |20.0s | ✅ | 45061 |
|  b0-06|    唤醒延时  | 0~6553.5s |0.0s | ✅ | 45062 |
|  b0-07|    压力上限保护值  | 0~100.0%(以目标压力比例联动) |10.0% | ✅ | 45063 |
|  b0-08|    压力上限保护停机延时  | 0~6553.5s（0：关闭检测） |0.3s | ✅ | 45064 |
|  b0-09|    下限频率超目标压力保护延时  | 0~6553.5s（0：关闭检测） |3.0s | ✅ | 45065 |
|  b0-10|    辅泵数量设定  | 0~4（0：关闭一拖多） |0 | ✅ | 45066 |
|  b0-11|    加辅泵压力容差  | 0~100.0%(以目标压力比例联动) |5.0% | ✅ | 45067 |
|  b0-12|    加辅泵延时  | 0~6553.5s |30.0s | ✅ | 45068 |
|  b0-13|    减辅泵压力容差  | 0~100.0%(以目标压力比例联动) |5.0% | ✅ | 45069 |
|  b0-14|    减辅泵延时  | 0~6553.5s |30.0s | ✅ | 45070 |
|  b0-15|    压力上限紧急减辅泵延时</br>（抢占b0-14的正常减泵时间）  | 0~6553.5s |3.0s | ✅ | 45071 |


探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}

  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
