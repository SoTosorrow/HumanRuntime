* cpp的mem_fn

```cpp
struct Test{
    void test();
};
std::for_each(v.begin(), v.end(), [](Test& t){
        t.test();
    });
std::for_each(v.begin(), v.end(), std::mem_fn(&Test::test));
```