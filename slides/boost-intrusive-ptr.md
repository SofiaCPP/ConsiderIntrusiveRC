##  `boost::intrusive_ptr`

- A smart pointer class for intrusive RC classes
- the same as `shared_ptr`

```
class Document;

void intrusive_ptr_add_ref(Document* doc) {
    ++doc->RC;
}

void intrusive_ptr_release(Document* doc) {
    if (--doc->RC == 0)
        delete doc;
}
```
