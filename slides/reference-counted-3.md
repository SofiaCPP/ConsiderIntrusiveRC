### Policies

```
template <typename Derived, typename RefCount>
struct RefCounted
{
    void add_ref() {
        RefCount::Increase(RC);
    }
    void release_ref() {
        if (RefCount::Decrease(RC)) {
            delete static_cast<Derived*>(this);
        }
    }
    RefCount::Type RC;
};
```

