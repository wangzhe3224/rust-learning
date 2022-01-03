# Rust Tips

这种方式处理异常更好：

`let mut f = File::Open(&mut fname).expect("这里放入失败的提示信息")`

因为，仅仅 `unwrap` 失败会直接 panic。

trait 用来做动态派发，generic 用来做静态派发。

## Topics

### trait 的原理和使用

### 小且给力的Rust库

- [evmap](https://github.com/jonhoo/evmap) - A lock-free, eventually consistent, concurrent multi-value map.
- [left-right](https://github.com/jonhoo/left-right) - A lock-free, read-optimized, concurrency primitive.
