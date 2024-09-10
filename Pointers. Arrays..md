**Material:**
# Part of the previous lecture about Pointers : 
![Pointer - The main type in C:](Static%20&%20Dynamic%20Typing.%20C%20Type%20System.%20Pointer%20Type..md#Pointer%20-%20The%20main%20type%20in%20C)
# Global, local & dynamic objects:
> [!abstract] Global & static objects
> - Stores in the Global storage

> [!abstract] Local objects
> - Stores in the Stack

> [!abstract] Dynamic objects
> - Stores in the Heap
> - Dynamic objects are the ones that are created at any moment during program execution.
> - The lifetime of dynamic objects is not under the scoping rules
> - Created by function ``malloc`` from `<stdlib.h>` direction of processor 
> ```C
> malloc(memory size)
> ```
> `void*` denotes a pointer to unknown type..
> ```C
> void* p = malloc(8);
> ```
> `(int*)` – change type of `malloc()`
> ```C
> int* p = (int*)malloc(8);
> ```
> - `free` – destroys *the Dynamic objects*, it needs to avoid *the memory leak*
> ```C
> #include <stdlib.h>
> struct S {int a, b;};
> 
> void* ptr = malloc(sizeof(struct S));
> struct S* s = 
> ```

