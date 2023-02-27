# Accelerated C++ Solutions

## Chapter 0

### 00

```C++
#include <iostream>

int main(){
    std::cout << "Hello World!" << std::endl;
    return 0;
}
```

> 编译运行后

![image-20230227203427816](../../AppData/Roaming/Typora/typora-user-images/image-20230227203427816.png)



### 01

> 这个表达式将3与4相加，得到7，然后用分号终止了一切行为。总之，它进行了计算但没有保存结果，且没有任何的副作用。



### 02

```c++
#include <iostream>

int main(){
    std::cout << "This (\") is a quote , and this (\\) is a backslash." << std::endl;
}
```



### 03

> 尝试之后，发现“\t”表示一个tab键，即四个英文字符，两个中文字符



### 04

> ```c++
> #include <iostream>
> 
> int main(){
>     std::cout << "#include <iostream>"<< std::endl;
>     std::cout << std::endl;
>     std::cout << "int main(){" << std::endl;
>     std::cout << "    std::cout << \"Hello World!\" << std::endl;" << std::endl;
>     std::cout << "    return 0;" << std::endl;
>     std::cout << "}" << std::endl;
> }
> ```



### 05

> 显然不是，它缺少大括号表达函数的作用域
>
> 报错：expected initializer before 'std'



### 06

> 是，花括号可以任意地嵌套，只要是成对出现



### 07

> 不是，第一个注释号会找到离它最近的反注释号，使得最后一个\*/多余，所以在多行注释界定符之间不要随意地添加，最好的方式是使用多个单行注释，如08



### 08

> 是，只要行首有//这样的注释定界符，后面可以随意地写任何东西



### 09

> int main(){}  



### 10

> ```c++
> #include <iostream>
> 
> int
> main
> (
>         )
> {
>     std
>     ::
>     cout
>             <<
>             "Hello World!"
>             <<
>             std
>             ::
>             endl
>             ;
>     return
>     0
>     ;
> }
> 
> ```

> 可以说除了字符串字面量以外，其他均可拆分
