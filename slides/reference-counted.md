## Embedding the RC

- it will be tedious to manually add the RC to every resource class
- inheritance and templates - [CRTP]() can help

```
class Document : public RefCounted<Document>
{
};
```
