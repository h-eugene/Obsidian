**Material:**
# Part of the previous lecture about Pointers : 
![Pointer - The main type in C:](Static%20&%20Dynamic%20Typing.%20C%20Type%20System.%20Pointer%20Type..md#Pointer%20-%20The%20main%20type%20in%20C)
# Global, local & dynamic objects:
> [!abstract] Global & static objects
> - Stored in Global storage

> [!abstract] Local objects
> - Stored in Stack

> [!abstract] Dynamic objects
> - Stored in Heap
> - Dynamic objects are the ones that are created at any moment during program execution.
> - The lifetime of dynamic objects is not under the scoping rules
> - Created by function `malloc` 
> ```C
> malloc(memory size)
> ```
> ```C
> void* p = malloc(8);
> ```
> `void*` denotes a pointer to unknown type..
> ```C
> int* p = (int*)malloc(8);
> ```
> `(int*)` – change type of `malloc()` 