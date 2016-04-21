##  Smart -> plain -> smart

- almost all of `C` and `C++` APIs allow `void*` for user data
  - some allow larger data buffer at performance penalty
  - *Shared* pointer semantics is convenient for embedding scripting languages
    with GC
  - using a `std::shared_ptr` for that does not work
    - allocate the `shader_ptr` on the heap and pay double dereferencing
- It is possible for *copy* or *move*-heavy algorithms or data structures to go
  down to plain pointers

note:
    Put your speaker notes here.
    You can see them pressing 's'.
