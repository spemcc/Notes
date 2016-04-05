# Templates

1. Declare template parameters with **_class_** if they can be only a user-defined type and with **_typename_** if they can also be a primitive type.
2. Member function templates cannot be declared virtual.  This constraint is imposed because the usual implementation
of the virtual function call mechanism uses a fixed-size table with one entry per virtual function. However, the number
of instantiations of a member function template is not fixed until the entire program has been translated. Hence,
supporting virtual member function templates would require support for a whole new kind of mechanism in C++
compilers and linkers.

