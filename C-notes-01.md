# C--notes--01

c++究极入门，10天能过二级我直接笑死

参考书籍C++ Primer Plus 中文版（第6版）

# 第一个代码文件

格式固定，注意`iostream`后面没有.h

```c++
#include <iostream>    //使用cin和cout进行输入输出的程序必须包含iostream
using namespace std;   //名称空间编译指令，用来区分不同文件的相同函数 p15

int main()             //int main 是函数头
{                      //大括号内是函数体
	cout << "hello xiaoxu"<< endl;   //cout表示输出,endl表示重起一行，光标移到下一行，类似c中\n p17
    system("pause");
	return 0;
} 
```

运行结果

```c++
hello xiaoxu
```

