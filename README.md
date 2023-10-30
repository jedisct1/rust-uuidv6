UUIDv6 for Rust

A simple [UUIDv6](https://uuid6.github.io/uuid6-ietf-draft/) crate.

```rust
let node = uuidv6::Node::new();

let mut st = node.uuidv6().into_iter();

let uid_1 = st.next();
let uid_2 = st.next();
let uid_3 = st.next();
```

This returns standard UUIDv6 strings.

As an alternative, a 16-byte binary representation of these UUIDs can be produced:

```rust
let node = uuidv6::Node::new();

let mut st = node.uuidv6_raw().into_iter();

let uid_1 = st.next();
let uid_2 = st.next();
let uid_3 = st.next();
```