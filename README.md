# WCH-Link Debug Tool

&emsp;&emsp;这是一个修改自WCH-Link官方调试工具的WCH-Link项目。最主要的修改是将USB A口更换更加方便的USB C接口。此外WCH-LinkW-R0-1v1的MIFA重新进行了设计，提高了天线带宽，修改了谐振频率不需要Π型网络匹配。


![Link功能和性能对比](./Images/WCH-Link%20Diff%20Table.png)

&emsp;&emsp;WCH-LinkW-R0-1v1使用MIFA天线体积虽然小，但是性能不算好。为了减小体积，天线辐射臂线宽很小，导体损耗增加，辐射效率下降，且会导致天线Q值变大。

![WCH-LinkW-R0-1v1](./Images/WCH-Link.png)

&emsp;&emsp;下图是去掉匹配网络实测的原厂的S11的矩形图。天线谐振点距离2.44GHz有一定距离，需要额外匹配网络。但是其带宽仅有31MHz，比2.4GHz BlueTooth带宽要小不少。显然原厂的天线设计并不是是很好。本项目优化了原厂的天线设计，S11更好，带宽更大，且谐振点刚好在2.44GHz附近不要Π型网络匹配。

![WCH-LinkW-R0-1v1 S11图](./Images/plot_20261002_155505_568.png)

&emsp;&emsp;下图是项目天线的仿真结果。

![优化天线的S11图](./Images/Snipaste_2026-10-14_10-58-45.png)

![优化天线的方向图](./Images/Snipaste_2026-10-14_11-02-44.png)