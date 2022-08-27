# Random code snippets to help with rust

Read binary file to u8 vec
```rust
let bytes = std::fs::read("path").unwrap();
```

Convert bytes to string
```rust
str::from_utf8(&bytes[1073..1079]).unwrap();
```

List files in dir
```rust
let paths = fs::read_dir("./").unwrap();
```
Measure time
```rust
use std::time::Instant;

let now = Instant::now();

let elapsed = now.elapsed();
println!("Elapsed: {:.2?}", elapsed);
```