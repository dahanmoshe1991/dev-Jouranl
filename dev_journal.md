self Notes of different topics

## JS
let/const vs var:
  var has a function scope while let/const has block scope

## c vs C++:
malloc() vs new(): 

- malloc(): It is a C library function that can also be used in C++, while the “new” operator is specific for C++ only. 
- Both malloc() and new are used to allocate the memory dynamically in heap. But “new” does call the *constructor* of a class whereas “malloc()” does not.

free() vs delete: 

- free() is a C library function that can also be used in C++, while “delete” is a C++ keyword.
- free() frees memory but doesn’t call Destructor of a class whereas “delete” frees the memory and also calls the Destructor of the class.
