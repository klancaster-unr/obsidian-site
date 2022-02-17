# Smart Pointers
---
## Overview Videos on Smart Pointers
[The Cerno on Smart Pointers](https://youtu.be/UOB7-B2MfwA)

## `unique_ptr`

**Definition:** 
- `std::unique_ptr` is a smart pointer that owns and manages another object through a pointer and disposes of that object when the `unique_ptr` goes out of scope. 
- Reference: https://en.cppreference.com/w/cpp/memory/unique_ptr

## `shared_ptr`

**Definition:**
- `std::shared_ptr` is a smart pointer that retains shared ownership of an object through a pointer. Several `shared_ptr` objects may own the same object. The object is destroyed and its memory deallocated when either of the following happens:
	- the last remaining `shared_ptr` owning the object is destroyed;
	- the last remaining `shared_ptr` owning the object is assigned another pointer via [operator=](https://en.cppreference.com/w/cpp/memory/shared_ptr/operator%3D "cpp/memory/shared ptr/operator=") or [reset()](https://en.cppreference.com/w/cpp/memory/shared_ptr/reset "cpp/memory/shared ptr/reset").
- reference counting is a common technique for managing the count of references to the pointer
- Reference: [std::shared_ptr - cppreference.com](https://en.cppreference.com/w/cpp/memory/shared_ptr)

## `make_shared` 
- available in C++ 11 #todo

## `weak_ptr`
- `std::weak_ptr` is a smart pointer that holds a non-owning ("weak") reference to an object that is managed by [std::shared_ptr](https://en.cppreference.com/w/cpp/memory/shared_ptr "cpp/memory/shared ptr"). It must be converted to [std::shared_ptr](https://en.cppreference.com/w/cpp/memory/shared_ptr "cpp/memory/shared ptr") in order to access the referenced object.
- Use cases
	- circular / cyclical references that would be problematic with shared pointers
- Reference: [std::weak_ptr - cppreference.com](https://en.cppreference.com/w/cpp/memory/weak_ptr)

## C++  14 and Above
- `make_unique`


## Terminology

- *RAII* - "resource acquisition  is initialization"
	- Objects are allocated on the stack
	- They acquire some resource, such as a file or memory
	- *Is Initialization* means that the resource is allocated in the [[constructor]], and release in the destructor


