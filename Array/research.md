# Array research

Use `CMD + Shift + V` to open this document as a preview in VSCode.
For each of the questions below, use the provided article and your own independent research to write an answer of 3-4 sentences. You don't need to go super deep into details and edge cases unless you have time, you just need the general gist.

[Starting point for research, read here first](https://lucasmagnum.medium.com/sidenotes-array-abstract-data-type-data-structure-b154140c8305)

## Questions(Write out you answers under separate headings)

0. What is an Abstract Data Type?
1. What is a Data Structure?
2. What is an array?
3. What is the difference between a dynamic and a static array?
4. What core operations can a dynamic array do?
5. What is the time complexity for the following operations in a dynamic array data structure?
   1. Searching(looking for something when you don't know an index)
   2. Updating(changing or adding a value) when you know the index
   3. Deleting like splice
   4. Accessing (retrieving a value) when you know an index

### What is an Abstract Data Type?

An abstract data type is a way of describing a data structure as basically an interface. It emphasizes behavior and NOT implementation. So it is inaccurate to say that an ADT has a specific time complexity for a specific operation.

### What is a Data Structure?

A data structure implements a data type. Data structures can implement ADTs in different ways, so the same functions can have different time and space complexities across different implementations.

### What is an array?

Arrays are defined as being a collection or body of elements that are accessed by an index. Any type can theoretically be stored in an array, though some languages that implement arrays may only allow one type to be stored in a slot at a time. Arrays need to be able to set and values at indices to be considered arrays.

### What core operations can an Array do?

#### Traversal

You can move over the indices in an array and read all of the values.

#### Search

During a traversal you can look at different values and seek out a particular value in the array.

#### Read and update

You can read change values at different indices in the array.

### What is the difference between a dynamic and static array?

Static arrays have a specific and unchangeable size. Dynamic arrays allow the size of the array to be changed if the final size of the array is unknown. This introduces time complexity ramifications to adding to an array. In JS, which uses dynamic arrays, pushing a new value can cause the original array to be copied and moved to a different, more free space in memory to accommodate the increased size.

### What is the time complexity for the following operations in a dynamic array data structure?

#### Searching(looking for something when you don't know an index)

O(n). If the array has no pattern to its ordering you have to look over every element.

#### Updating(changing or adding a value) when you know the index

O(1). You go to that place in memory and alter a value.

#### Deleting like splice

O(n). You have to reassign all of the other indices in the array to maintain the index order.

#### Accessing (retrieving a value) when you know an index

O(1). This is just going to an index location and grabbing the value.
