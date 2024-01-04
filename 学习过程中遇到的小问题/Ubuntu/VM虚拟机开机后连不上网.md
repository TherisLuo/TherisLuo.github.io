# VM虚拟机连不上网
> 解决方法来源 [解决VM虚拟机中ubuntu系统上不了网的问题](http://t.csdnimg.cn/JhadZ)
## 方法一 虚拟网络编辑器还原默认
* 参考链接 [VMware虚拟机Ubuntu16.04联网问题解决方案 - SegmentFault 思否](https://link.csdn.net/?target=https%3A%2F%2Fsegmentfault.com%2Fa%2F1190000022982425)
* 首先关闭ubuntu系统
* 点击编辑，虚拟网络编辑器
  ![1](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20155241.png?raw=true)
* 点击编辑，选中VMnet8的Nat模式，点击还原默认设置，就会卸载先前的所有虚拟网卡，重新配置新的虚拟网卡
  ![2](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20164917.png?raw=true)
*  ubuntu 虚拟机选着 NAT模式不变  
  ![3](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20165227.png?raw=true)
