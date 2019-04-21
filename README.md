color-backtrace
===============

[![Crates.io][crates-badge]][crates-url]
[![docs.rs][docs-badge]][docs-url]
[![MIT licensed][mit-badge]][mit-url]


[crates-badge]: https://img.shields.io/crates/v/color-backtrace.svg
[crates-url]: https://crates.io/crates/color-backtrace
[docs-badge]: https://docs.rs/color-backtrace/badge.svg
[docs-url]: https://docs.rs/color-backtrace/
[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
[mit-url]: LICENSE

A Rust library that makes panics a little less painful by nicely colorizing them
and printing the relevant source snippets.

```toml
[dependencies]
color-backtrace = { version = "0.1" }
```

To enable it, simply place this code somewhere in your app initialization code:
```rust
color_backtrace::install();
```

### Features
- Colorized backtraces in order to be easier on the eyes
- Show source snippets if source files are found on disk
- Print frames of application code in different color (red) than those of dependencies (green)
- Hide all the frames after the panic was already initiated

### Screenshot
![Screenshot](https://mainframe.pw/u/g5nrTt2w0wAwskFO.png)
