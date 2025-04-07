---
title: 2.7 变频器选型指导
toc: true
weight: 7
next: /docs/user-manual-for-skf8000-series-inverter/Mounting/
prev: /docs/user-manual-for-skf8000-series-inverter/product-information/product-selection-specification-table/
---

[变频器](/products/vector-variable-frequency-driver/)可提供三种控制方式：普通V/F、SVC、VC。  
选用变频器时首先必须明确系统对变频调速的技术要求、变频器的应用场合及负载特性的具体情况，并从适配电机、输出电压、额定输出电流等方面因素进行综合考虑，进而选择满足要求的机型及确定运行方式。

基本原则为：电机额定负载电流不能超过变频器的额定电流。一般情况下按[变频器说明书](/zh-cn/docs/user-manual-for-skf8000-series-inverter/ "变频器说明书")所规定的配用电机容量进行选择，注意比较电机和变频器的额定电流。变频器的过载能力对于起动和制动过程才有意义。凡是在运行过程中有短时过载的情况，会引起负载速度的变化。如果对速度精度要求比较高时，请考虑放大一个档次。

风机和水泵类型：在过载能力方面要求较低，由于负载转矩与速度的平方成正比，所以低速运行时负载较轻（罗茨风机除外）又因为这类负载对转速精度没有特殊要求，故选择平方转矩V/F。

恒转矩负载：多数负载具有恒转矩特性，但在转速精度及动态性能等方面要求一般不高。例如挤压机、搅拌机、传送带、厂内运输电车、吊车的平移机构等。选型时可选多段V/F运行方式。

被控对象有一定的动、静态指标要求：这类负载一般要求低速时有较硬的机械特性，才能满足生产工艺对控制系统的动、静态指标要求。选型时可选择SVC控制方式。

被控对象有较高的动、静态指标要求：对于调速精度和动态性能指标都有较高要求及高精度同步控制的场合，可采用VC控制方式。例如，电梯、造纸，塑料薄膜加工生产线。

探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}
  {{< card link="/docs/user-manual-for-skf8000-series-inverter/table-of-contents/" title="变频器使用说明书目录" icon="newspaper"  >}}
  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
