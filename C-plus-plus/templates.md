# Templates

1. Declare template parameters with **_class_** if they can be only a user-defined type and with **_typename_** if they can also be a primitive type.
2. Member function templates cannot be declared virtual.  This constraint is imposed because the usual implementation
of the virtual function call mechanism uses a fixed-size table with one entry per virtual function. However, the number
of instantiations of a member function template is not fixed until the entire program has been translated. Hence,
supporting virtual member function templates would require support for a whole new kind of mechanism in C++
compilers and linkers.
3. There are three types of template types.
  * Type parameters 
    * Introduced with either the keyword typename or the keyword class, act as a typedef  
  * Non-Type parameters
    * Constant values that can be determined at compile or link time 
  * Template template parameters

4. **_typename_** keyword outside of template parameter: Tells compiler that it is a type. 
```c++
Foo<T>::x*y; // Is this a type or multiplication?
```
5.

