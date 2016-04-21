### Using `RefCounted` with `boost::intrusive_ptr`

- catch all classes inheriting `RefCounted`

```
template <typename T>
void intrusive_ptr_add_ref(RefCounted<T>* p) {
    p->add_ref();
}

template <typename T>
void intrusive_ptr_release(RefCounted<T>* p) {
    p->release_ref();
}
```
