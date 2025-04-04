---
title: 5.2 P1组：电机参数
toc: true
weight: 2
next: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/vector-parameter/
prev: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/basic-parameters/
---
{{< callout type="info" >}}
  变频器参数属性说明
{{< /callout >}}

✅：表示该参数的设定值在变频器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在变频器处于运行状态时，不可更改；  
❎：表示该参数的数值是实际检测记录值，不能更改；

## P1组：电机参数

|  功能代码|    名称  | 设定范围 | 出厂值 |属性 | DEC地址 |
| :----: |    :----   | :----   | :----:   | :----:   | :----:   |
|  P1-00|    电机类型选择  | 0：普通异步电机</br>1：变频异步电机</br>2：永磁同步电机（另建说明书） |0| ✳️ | 61696 |
|  P1-01|    电机额定功率  | 0.1~1000KW |机型确定 | ✳️ | 61697 |
|  P1-02|    电机额定电压  | 1~380V |机型确定 | ✳️ | 61698 |
|  P1-03|    电机额定电流  | 0.01~100.00A |机型确定 | ✳️ | 61699 |
|  P1-04|    电机额定频率  | 0.01Hz~最大频率 |机型确定 | ✳️ | 61700 |
|  P1-05|    电机额定转速  | 1~65535rpm |机型确定 | ✳️ | 61701 |
|  P1-10|    异步电机空载电流  | 0.01~P1-03 |调谐参数 | ✳️ | 61706 |
|  P1-37|    调谐选择  | 0：无操作</br>1：异步机静止调谐</br>2：异步机完整调谐</br>3：静止调谐2 |0 | ✳️ | 61733 |



探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}

  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
