---
title: 5.5 P4组：输入端子参数
toc: true
weight: 5
next: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/output-terminal-parameters/
prev: /docs/user-manual-for-skf8000-series-inverter/functional-parameter-table/v-f-control-parameters/
---
{{< callout type="info" >}}
  变频器参数属性说明
{{< /callout >}}

✅：表示该参数的设定值在变频器处于停机、运行状态中，均可更改；  
✳️：表示该参数的设定值在变频器处于运行状态时，不可更改；  
❎：表示该参数的数值是实际检测记录值，不能更改；


## P4组：输入端子参数

|  功能代码|    名称  | 设定范围 | 出厂值 |属性 | DEC地址 |
| :----: |    :----   | :----   | :----:   | :----:   | :----:   |
|  P4-00|    X1端子功能选择  | 0：无功能</br>1：正转运行（FWD）</br>2：反转运行（REV）</br>3：三线式运行控制</br>4：正转点动（FJOG）</br>5：反转点动（RJOG）</br>6：端子UP</br>7：端子DOWN</br>8：自由停车</br>9：故障复位（RESET）</br>10：运行暂停</br>11：外部故障常开输入</br>12：多段指令端子1</br>13：多段指令端子2</br>14：多段指令端子3</br>15：多段指令端子4</br>16：加减速时间选择端子1</br>17：加减速时间选择端子2</br>18：频率切换</br>19：UP/DOWN设定清零（端子/键盘）</br>20：运行命令切换端子1</br>21：加减速禁止</br>22：PID暂停</br>23：PLC状态复位</br>24：摆频暂停</br>25：计数器输入</br>26：计数器复位</br>27：长度计数输入</br>28：长度复位</br>29：转矩控制禁止</br>30：HDI脉冲频率输入（X5）</br>31：保留</br>32：立即直流制动</br>33：外部故障常闭输入</br>34：频率修改使能</br>36：外部停车端子1</br>37：运行命令切换端子2</br>38：PID积分暂停</br>39：频率源X与预置频率切换</br>40：频率源Y与预置频率切换</br>43:PID参数切换</br>44：用户自定义故障1</br>45：用户自定义故障2</br>46：速度控制/转矩控制切换</br>47：紧急停车</br>48：外部停车端子2</br>49：减速直流制动</br>50：本次运行时间清零</br>51：两线式和三线式切换</br>52：禁止反转</br>53：单端子UP/DOWN使能，频率源切换（同功能18）</br>54：端子激活UP，不激活为DOWN |01 | ✳️ | 62464 |
|  P4-01|    X2端子功能选择  | 同P4-00 |02 | ✳️ | 62465 |
|  P4-02|    X3端子功能选择  | 同P4-00 |04 | ✳️ | 62466 |
|  P4-03|    X4端子功能选择  | 同P4-00 |09 | ✳️ | 62467 |
|  P4-04|    X5端子功能选择  | 同P4-00 |12 | ✳️ | 62468 |
|  P4-05|    X6端子功能选择  | 同P4-00 |00 | ✳️ | 62469 |
|  P4-06|    X7端子功能选择  | 同P4-00 |00 | ✳️ | 62470 |
|  P4-10|    X端子滤波时间  | 0.000s~1.000s |0.010s | ✅ | 62474 |
|  P4-11|    端子命令方式  | 0：两线式1</br>1：两线式2</br>2：三线式1</br>3：三线式2 |0 | ✳️ | 62475 |
|  P4-12|    端子UP/DOWN变化率  | 0.001Hz/s~65.535Hz/s |1.00Hz/s | ✅ | 62476 |
|  P4-13|    AI曲线1最小输入  | 0.00v~P4-15 |0.00V | ✅ | 62477 |
|  P4-14|    AI曲线1最小输入对应设定  | -100.0%~+100.0% |0.0% | ✅ | 62478 |
|  P4-15|    AI曲线1最大输入  | P4-13~+10.00V |10.00V | ✅ | 62479 |
|  P4-16|    AI曲线1最大输入对应设定 | -100.0%~+100.0% |100.0% | ✅ | 62480 |
|  P4-17|    AI滤波时间  | 0.00s~10.00s |0.10s | ✅ | 62481 |
|  P4-18|    AI曲线2最小输入  | 0.00V~P4-20 |0.00V | ✅ | 62482 |
|  P4-19|    AI曲线2最小输入对应设定  | -100.0%~+100.0% |0.0% | ✅ | 62483 |
|  P4-20|    AI曲线2最大输入  | P4-18~+10.00V |10.00V | ✅ | 62484 |
|  P4-21|    AI曲线2最大输入对应设定  | -100.O%~+100.0% |100.0% | ✅ | 62485 |
|  P4-22|    AI2滤波时间  | 0.00s~10.00s |0.10s | ✅ | 62486 |
|  P4-23|    AI曲线3最小输入  | 0.00V~P4-25 |0.00V | ✅ | 62487 |
|  P4-24|    AI曲线3最小输入对应设定  | -100.O%~+100.0% |0.0% | ✅ | 62488 |
|  P4-25|    AI曲线3最大输入  | P4-23~+10.00V |10.00V | ✅ | 62489 |
|  P4-26|    AI曲线3最大输入对应设定  | -100.O%~+100.0% |100.0% | ✅ | 62490|
|  P4-27|    AI3滤波时间  | 0.00s~10.00s |0.10s | ✅ | 62491 |
|  P4-28|    HDI脉冲最小输入  | 0.00kHz~P4-30 |0.00kHz | ✅ | 62492 |
|  P4-29|    HDI脉冲最小输入对应设定  | -100.O%~+100.0% |0.0% | ✅ | 62493 |
|  P4-30|    HDI脉冲最大输入  | P4-28~50.00kHz |50.00kHz | ✅ | 62494 |
|  P4-31|    HDI脉冲最大输入对应设定  | -100.O%~+100.0% |100.0% | ✅ | 62495 |
|  P4-32|    HDI脉冲滤波时间  | 0.00s~10.00s |0.10s | ✅ | 62496 |
|  P4-33|    AI曲线选择  | 个位：AI1曲线选择</br>1：曲线1（2点，P4-13~P4-16）</br>2：曲线2（2点，P4-18~P4-21）</br>3：曲线3（2点，P4-23~P4-26）</br>十位：AI2低于最小输入设定选择，同上</br>百位：AI3低于最小输入设定选择，同上 |321 | ✅ | 62497 |
|  P4-34|    AI低于最小输入设定选择  | 个位：AI1低于最小输入设定选择</br>0：对应最小输入设定</br>1：0.0%</br>十位：AI2低于最小输入设定选择，同上</br>百位：AI3低于最小输入设定选择，同上  |000 | ✅ | 62498 |
|  P4-35|    X端子有效模式选择1  | 0：高电平有效</br>1：低电平有效</br>个位：X1</br>十位：X2</br>百位：X3</br>千位：X4</br>万位：X5 |000 | ✅ | 62499 |
|  P4-37|    AI输入电压/电流选择  | 个位：AI1</br>十位：AI2</br>0：电压输入</br>1：电流输入 |000 | ✳️ | 62501 |
|  P4-38|    X1导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62502 |
|  P4-39|    X2导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62503 |
|  P4-40|    X3导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62504 |
|  P4-41|    X4导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62505 |
|  P4-42|    X5导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62506 |
|  P4-43|    X6导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62507 |
|  P4-44|    X7导通延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62508 |
|  P4-48|    X1断开延迟时间  | 0.0s~6553.5s |0.0s | ✳️ | 62512 |
|  P4-49|    X2断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62513 |
|  P4-50|    X3断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62514 |
|  P4-51|    X4断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62515 |
|  P4-52|    X5断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62516 |
|  P4-53|    X6断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62517 |
|  P4-54|    X7断开延迟时间   | 0.0s~6553.5s |0.0s | ✳️ | 62518 |



探索这些文档以便了解更多内容：

{{< cards >}}
  {{< card link="/products/vector-variable-frequency-driver/" title="立即购买高性能矢量变频器" icon="shopping-cart" >}}

  {{< card link="/blog/faq/" title="变频器常见问题解答" icon="newspaper" >}}
{{< /cards >}}	
