## Dynamic Memory Allocation

Dynamic memory management refers to dealing with objects that are stored on the [[heap]] rather than on the [[stack]]. We store objects on the heap 
- when we are wanting to keep them around for a while, or
- when the objects are very large or there are many of them (in an array, etc.)


Objects stored on the [[stack]] are destroyed when they go out of scope. Objects stored on the heap stick around until we explicitly delete them from memory.

## Creating Objects

Objects are created on the heap using either the `new` operator or using [[Smart Pointers|smart pointers]].

## Comparing Heap vs Stack Allocation
- Heap operations are slower by far, so prefer stack allocation when possible
- Stack memory is limited, whereas heap allocation is generally not
