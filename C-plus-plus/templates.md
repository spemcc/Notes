# Templates

1. Declare template parameters with **_class_** if they can be only a user-defined type and with **_typename_** if they can also be a primitive type.
2. 
```c++

template<class Bar>
class Foo : public Bar
{
...
};
Foo<Baz<T>> foo;
    
//template template parameter
template<template <class Quz> class Bar>
class Foo : public Bar<T>
{
...
};
  
 Foo<Baz> foo;
```
