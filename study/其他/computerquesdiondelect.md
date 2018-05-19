### 1.win10关机自动重启

1. 启动和故障恢复中关闭自动启动
2. 系统电源管里关闭快速启动
3. 关闭可唤醒电脑的USB设备
   1. win+r，输入cmd，回车。输入PowerCfg -DEVICEQUERY wake_armed 。查看可幻想电脑的USB设备。
   2. 进入资源管理器 - 右键此电脑 - 设备管理器。右击相应设备 - 属性 - 电源管理 - 允许此设备唤醒计算机（勾去） 
   3. *原因大概率是因为网卡,网卡驱动不兼容导致*  [参考资料](https://jingyan.baidu.com/article/19192ad8f8f923e53e57071e.html)

