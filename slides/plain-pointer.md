##  Smart -> plain -> smart

- `C` APIs
- 90% of `C++` APIs allow `void*` for user data
  - using a `std::shared_ptr` for that does not always work
- It is possible for *copy* or *move*-heavy algorithms or data structures to go
  down to plain pointers

note:
    Put your speaker notes here.
    You can see them pressing 's'.
