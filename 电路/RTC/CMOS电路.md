# RTC/CMOS 电路。

一、RTC/CMOS 电路
作用：RTC 控制系统时间，CMOS 存储时间及 BIOS 设置。
RTC：实时时钟控制器。
CMOS：CMOS RAM 存储器。
CMOS/RTC 都是集成在南桥内部的模块。

1、电路核心
南桥(南桥内部 RTC/CMOS 模块)
2、主要电压及信号。
1、供电 VCCRTC: RTC/CMOS 的供电，大约 3V 左右。 2.时钟 32.768KHZ：由 32.768 晶振产生。 3.复位 RTCRST#、SRTCRST#,正常工作时必须为高电平(3V)，如果为低电平 RTC/CMOS 复位(初始化清零)。

![img](https://tuchuang-cw.oss-cn-shanghai.aliyuncs.com/img/20260617164746.png)

RC 延时电路一般用于复位电路中

- 台式机与笔记本 RTC/CMOS 电路不同点：
  1、台式机手动复位使用 CMOS 跳针，笔记本手动复位使用接地的焊点。
  2、台式机 CMOS 电池通常不能被充电，笔记本 CMOS 电池在某些主板上可以充电。
  3、笔记本某些内置电池型号取消小电池，直接大电池供电。

RTC/CMOS 在主板上赵线：
1、确定出发点目的地(搞清楚从哪里开始找，找到哪去？)
例如：RTC/CMOS 电路：出发点(电池正极)--目的地
