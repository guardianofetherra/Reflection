# Reflection
Using C++ Macros to do up a static library of Components

Can be used with smart enums also

Two type of libraries, 
First is the reflection library where you can get all the variables of the component using the name of the component that you desire
Second is the serialize library where you can create a component using the name of the component


To use it, you need to call REFLECT() in the header class file,
then at the end of the cpp, you need to call the REFLECT_VIRTUAL() if it is a pure virtual class
followed by REFLECT_PROPERTY(property_name)
after reflecting all the property, call REFLECT_END()

For non-pure virtual class, at the end of the cpp, you need to call the REFLECT_INIT()
followed by REFLECT_PROPERTY(property_name)
after reflecting all the property, call REFLECT_END()

N.B. This is only tested with a project that I am doing for my school assignment, and it is a work in progress so there might
be bugs
