```
namespace boost {

  struct thread_unsafe_counter;
  struct thread_safe_counter;

  template<class DerivedT, class CounterPolicyT = thread_safe_counter>
  class intrusive_ref_counter
  {
  public:
      // ctors and assignments

      unsigned int use_count() const noexcept;

  protected:
      ~intrusive_ref_counter() = default;
  };
}
```
