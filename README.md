### **AddrSearch**

*** 
#### **目录**
* [项目简介](#项目简介)
* [功能简介](#功能简介)
* [作者简介](#作者简介)
* [项目支持](#项目支持)

***
#### **项目简介** 

AddrSearch 旨在对32/64位进程进行 特征定位，并根据特征类型快速准确 计算 相关偏移 ，基址 ，CALL 。

#### **功能简介** 

1、根据目标进程和模块进行 特征码定位 并根据相应定义类型自动计算 相关 基址 CALL  偏移 数值；

2、x86/x64 进程支持；

3、模糊式特征码搜索（以 半角偶数个  ????????" 作为通配符）；

4、支持define 格式和 constexpr uint64_t  格式定义；

6、特殊码列表 保存 读取；

7、相对模块 地址方式 仅 地址 函数 指针内容 三个类型 使用相对地址 ，其他 4种取值方式均不使用相对地址；
#### **类型说明** 

1、地址:  就是搜索后的地址 加偏移修正值 。注：任何类型的偏移修正值请输入16进制；

2、函数:就是  取 CALL 0xXXXXXXXXX   （CALL头地址）  

3、[指针内容]_x64 取 x64指针内容，专门针对64位 取指针内容 设计  如 lea rdx,[1408A2B10]   mov rax,[1408A2B10] 

4、1 字节 2字节 4字节 8字节 地址内容四种类型 无需过多解释，即 地址处的值。

6、32进进程 指针内容 也使用 4字节 取值方式 如mov eax,[1408A2B10] ；
 
 
#### **作者简介** 
网名geekxiao y，QQ： 274351055 

开源项目圈（QQ群）
  x64编程交流群:775801853

