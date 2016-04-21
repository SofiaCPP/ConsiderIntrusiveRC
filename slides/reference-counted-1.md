```
template <typename Derived>
struct RefCounted
{
    void add_ref() {
        ++RC;
    }
    void release_ref() {
        if (--RC == 0) {
            // We have to delete the derived class
            // otherwise we'll need to have virtual dtor
            delete static_cast<Derived*>(this);
        }
    }
    int RC;
};
```
