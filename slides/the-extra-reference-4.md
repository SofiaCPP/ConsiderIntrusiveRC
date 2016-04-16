##  The extra reference


The extra reference requires an extra allocation for the *control-block*.

- touching two different parts of the heap for each access to the block /
  resource
- small allocations are the worst
- `std::make_shared` solves this

