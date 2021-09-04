# 记录学习C++ Primer Plus的笔记
# 第2章

#### 2.1.3 C++预处理

##### **关于“[using namespace std](https://www.cnblogs.com/uniqueliu/archive/2011/07/10/2102238.html)”**

对于一个存在着标准输入输出的C++控制台程序，一般会在#include <iostream>的下一行发现一句话，using  namespace std。这句话其实就表示了所有的标准库函数都在标准命名空间std中进行了定义。其作用就在于避免发生重命名的问题。

直接使用“using namespace std”可能在大项目中有潜在的问题，可以根据使用的函数单独声明使用如：using std::cout; using std::endl;  using std::cin;



##### 头文件

可以使用iostream.h、math.h、iostream、cmath
  
##### 运算符也可以重载
插入运算符(<<)看上去像按位左移的运算符(<<),同样的&符号既可以表示地址运算符也可以表示AND运算符，*既表示乘法也可以表示指针引用

# 第3章
##### 初始化

初始化变量的两种方法
```c++
int owls = 101;
int wrens(432);
```

另外的初始化方法，这种方式用于数组和结构
```c++
int emus{7};	    // 设置emus为7
int rheas = {12};	// 设置rheas为12
int rocs = {};	    // 设置rocs为0
int psychics{};	    // 设置psychics为0
```  

整型表示方法
如果第一位为1~9，则表示为十进制
```  
如：1、93
```  
如果第一位为0，第二位为1~7则表示为八进制
```
如：042、01
```  
如果前两位为0x或0X，则表示为十六进制
```
如：0xF、0X15
```
  
转义字符
Ctrl+Z的ASCII码为26、032、0x1A，可以用转义序列来表示该字符:\032或\0x1A
```
如：'\032'、'\0x1A'、"hi\0x1A there"  
```  
