# 记录学习C++ Primer Plus的笔记
# 第2章

#### 2.1.3 C++预处理

##### **关于“[using namespace std](https://www.cnblogs.com/uniqueliu/archive/2011/07/10/2102238.html)”**

对于一个存在着标准输入输出的C++控制台程序，一般会在#include <iostream>的下一行发现一句话，using  namespace std。这句话其实就表示了所有的标准库函数都在标准命名空间std中进行了定义。其作用就在于避免发生重命名的问题。

直接使用“using namespace std”可能在大项目中有潜在的问题，可以根据使用的函数单独声明使用如：using std::cout; using std::endl;  using std::cin;



##### 头文件

可以使用iostream.h、math.h、iostream、cmath
