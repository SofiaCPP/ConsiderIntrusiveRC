##  Lack of Control

- `std::shared_ptr` is thread-safe. The reference count is *atomic* or has a
  mutex!
  - using a `shared_ptr` in a single thread is more popular than it seems
- can not change the reference count manually.  May be the standard does not
  require reference counting.


note:
  - using a `shared_ptr` in a single thread is more popular than it seems
    - modifying some objects in multiple threads with locking doesn't make
      sense
    - game logic in a game
    - executing JavaScript in a browser
