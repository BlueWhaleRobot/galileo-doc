# <a href="#" id="start"></a>常见问题与处理办法

## <a href="#" id="one"></a>4.1 遥控过程中突然失灵无法操纵

可能是底盘红外避障模块被触发激活了，请先检查机器人周围是否有障碍物，清空障碍物之后等待5秒，再次尝试控制。

## <a href="#" id="two"></a>4.2 图传画面卡顿、延时

请右键关闭图传后，重新打开图传，如果问题还是存在，请等待机器人驶离这段信号阻塞区域后再尝试

## <a href="#" id="three"></a>4.3 建图过程中视觉状态显示“丢失”，黑白图传画面中没有出现青绿色的特征点

分如下两种情况：
  a. 打开视觉后，视觉状态没有出现过“追踪中”
  b. 视觉状态之前出现过“追踪中”，遥控建图过程中突然变成了“丢失”

解决办法：
  a.尽量保证机器人为直线运动，前进一段时间后再后退一段时间，如此反复动作直到视觉状态变成“追踪中”
  b.将小车退回（保证小车朝向不变）到视觉状态出现“追踪中”的最近位置，使机器人视觉系统重新锁定。
  c.两个办法都尝试多次后，如果还是显示“丢失”，请关闭视觉然后重新开启视觉，从头开始扫描建图。

## <a href="#" id="four"></a>4.4 建立连接后，遥控图传正常，但是客户端不显示地图和巡检路径

地图和巡检路径的加载时间很长，请耐心等待5分钟左右，如果还是不显示，请关闭客户端软件后，再打开尝试。

## <a href="#" id="five"></a>4.5 开启自主巡检后，视觉状态一直显示“丢失”，机器人在原地摆动

这种情况说明机器人无法识别当前位置，有两种可能：
a.当前位置在建图扫描过程中没有被记录过，b.当前位置的光照强度或者物品分布发生了较大的变化。
对于第一种情况请将机器人遥控到建图扫描过的位置，保证机器人朝向和建图时的朝向一致，再重新开启自主巡检。
第二种情况，需要对环境进行重新扫描建图，巡检路径和站点也需要重新绘制。

## <a href="#" id="six"></a>4.6 无法关闭自主巡检

多尝试点击几次，如果还是无法关闭，请手动关闭机器人底盘电源开关后，再通过客户端软件使车载主机关机。

## <a href="#" id="seven"></a>4.7 规划巡检路径和轨迹时，加载的地图显示出一团乱糟糟的青色点、蓝色机器人轨迹点明显不像建图时的遥控路径

这说明视觉地图的建立失败了，请重新进行一次扫描建图，然后再尝试。

## <a href="#" id="eight"></a>4.8 机器人无法自主避障

检查kienct指示灯是否正常，kienct供电线是否连接完好，车载主机关机后再重新开机测试。

## <a href="#" id="nine"></a>4.9 客户端无法连接机器人

请登录局域网路由管理界面，检查客户端PC和机器人主机是否都已经连上网络，参考第二章的联网操作重新设置一下两者网络。
