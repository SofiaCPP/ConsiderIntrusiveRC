##  intrusive_ptr

- No extra reference count
- from *smart* pointer to *plain* pointer and back to *smart* pointer
- Control over the type of the reference count
- Manually change the reference count
- Use existing reference counting in external APIs
  - Direct X
  - Almost every OS resource on Mac OS X and iOS
  - Embedding scripting languages GC
