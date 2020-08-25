# C--notes--01

c++究极入门，10天能过二级我直接笑死

参考书籍C++ Primer Plus 中文版（第6版）

#### 第一个代码文件

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

#### 注释

```c++
//单行注释
/*多行
注释*/
```

#### 变量定义

c++中变量定义的风格是在第一次使用时定义，也可以在开头定义。

```c++
#include <iostream>
using namespace std;

int main()
{
	int carrots;
	carrots=25;
	cout << carrots;
	system("pause");
	return 0;
} 
//运行结果是25
```

#### 输入语句

用`cin`进行输入

```c++
#include <iostream>
using namespace std;

int main()
{
	int carrots;
	cout << "how many caaaots do you have?" << endl; 
	cin >> carrots;  //c++ input
	cout << carrots;
	system("pause");
	return 0;
} 
//输入25，输出25.
```

#### 输出的拼接

```c++
cout << "now you have " << carrots << "carrots."<< endl; 
//四行变一行
```

#### 函数

自定义函数的使用

```c++
#include <iostream>
using namespace std;
void simon(int); //注意分号
int main()
{
	cout << "please input m" << endl;
	int m;
	cin >> m;
    simon(m);
}
void simon (int n)
{
	cout << "its the " << n << " times i learn c++" << endl;
    //void类型不需要返回值
} 
```

