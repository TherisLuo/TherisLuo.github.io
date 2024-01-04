# VSCode C++ 输出乱码问题
## 问题描述
如题，在ros入门过程中第一个用ros跑的cpp程序，编译没问题，启动roscore，新建终端然后rosrun，输出中文时乱码  
![1](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20165647.png?raw=true)  
![2](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20170231.png?raw=true)
## 问题解决
* 调用函数：  
```setlocale(LC_ALL,"")```  
通过这条语句我们可以解决乱码问题。
![3](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20171018.png?raw=true)  
问题就解决了。
![4](https://github.com/RisingsunLuo/Pictures/blob/main/Screenshots/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-12-18%20171055.png?raw=true)
