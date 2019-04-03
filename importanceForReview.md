##  Java Question

##### 1, How does the java interpreter build link between variable name and memory box?

* The Java interpreter creates an entry in an internal table that maps each variable name to the location of the first bit in the memory box.
* Remember that primitive and reference type are installed in different way, really similar to the python under the hood.

##### 2, overriding of implementation inheritance and interface inheritance

* interface inherience should be overridden, and implementation inherience can also be overridden. Java choose the method call based on "dynamic method selection"—When Java runs a method that is overriden, it searches for the appropriate method signature in it's **dynamic type** and runs it.
* For overloaded method,  When Java checks to see which method to call, it checks the **static type** and calls the method with the parameter of the same type.

## C++ Question

##### 1, how to understand "const" in various way

<img src="/Users/yuanbaba/Documents/cs-material/snapshot/1.jpg" width="500px" />

##### 2, what is the difference between pointer and reference in C++

<img src="/Users/yuanbaba/Documents/cs-material/snapshot/ptr-ref.jpg" style="zoom: 40%">

* Examples of understanding reference variable and pass by reference

<img src="/Users/yuanbaba/Documents/cs-material/snapshot/reference.jpg" width="500px" />

<img src="/Users/yuanbaba/Documents/cs-material/snapshot/pass-by-reference.jpg" width="500px" />

Note: References in python are like pointers in C/C++ not C-style references. That is, in python, all variables are references that hold the memory address of objects.

##### 3, Interitance

* 1, virtual method, non-virtual method and their inheritance in C++
  * Virtual methods are methods been overridden, like implementation in java, completely virtual methods are similar to interface inherience, both apply dynamic method selection, aka, dynamic binding. For non-vritual methods, they are static binding. **Never override non-virtual method!**
* 2， Inheritance , Ctors and Dtors
  * Based class actor called first, folled by derived class ctor, if no explicit ctor is called for the base class, the default ctor is called.
  * Derived class dtor called first, followed by base class dtor, 
* 3, public, protected, and private inheritance
  * 公有继承（public）时，基类的公用成员和保护成员在派生类中保持原有的访问属性
  * 保护继承(protected)的特点是基类的所有公有成员和保护成员都成为派生类的保护成员，并且只能被它的派生类成员函数或友元访问，基类的私有成员仍然是私有的。
  * 私有继承(private)即所有基类成员均变成派生类的私有成员，基类的私有成员仍然不能在派生类中访问。

##### 4, IO stream

* [link](http://www.cplusplus.com/doc/tutorial/files/)



Does stack frame project to a continuous memory space in computer?

can a variable(memory box) appears in stack and heap simultaneously?

In multiple memory box simultaneously.



