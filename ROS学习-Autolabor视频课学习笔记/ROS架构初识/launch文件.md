# launch文件  
## 使用背景
使用launch文件一次启动多个节点
## launch文件的添加
打开VSCode
* 在工程包下面新建launch文件夹
* 在launch文件夹下面新建launch文件，文件名任意，后缀为.launch
  launch文件就是把所有文件连接起来的，xml文件
  我们在里面根据自己需求写一下：  
```
<launch>
  <!-- 添加被执行的节点 -->
  <!-- 乌龟GUI -->
  <node pkg="turtlesim" type="turtlesim_node" name="turtle_GUI"/>
  <node pkg="turtlesim" type="turtle_teleop_key" name="turtle_key"/>
</launch>
```
有`<launch></launch>`就可以启动roscore  
先加一个跑小乌龟的，node节点例子，下面有3个属性pkg,type,name，  
- pkg对应跑小乌龟的包名turtlesim，  
- type对应被执行的节点turtlesim_node，  
- name就是给你的节点命一个名，如turtle_GUI，  
键盘控制也是如法炮制，`<node pkg="turtlesim" type="turtle_teleop_key" name="turtle_key"/>`
然后`ctrl + ~`进入命令窗口，先source一下，刷新  
```
source ./devel/setup.bash
``` 
 * launch命令使用：
   `roslaunch <工程包名称> <launch文件名称.launch>`  
launch启动就会出现小乌龟，然后鼠标点一下VSCode的命令行，就可以用键盘的上下左右控制小乌龟了  
之前写过一个用ros输出文本的C++程序，把它也可以加进来，那就是写成  
```
  <node pkg="hello_vscode" type="hello_vscode_c" name="hello"/>
```
