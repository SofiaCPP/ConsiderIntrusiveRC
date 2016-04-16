##  The extra reference

* `+` - single pointer dereferencing to get the resource
* `-` - `sizeof(shared_ptr<T>) == 2 * sizeof(T*)`
  Not a chance to use this `shared_ptr` with plain pointers *API*s, (more on
  that later).

