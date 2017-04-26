# open api [![Build Status](https://travis-ci.org/softprops/openapi.svg?branch=master)](https://travis-ci.org/softprops/openapi)

> Rust crate for serializing and deserializing [open api](http://swagger.io/specification/) documents

## install

add the following to your `Cargo.toml` file

```toml
[dependencies]
openapi = "0.1"
```

## usage

```rust
extern crate openapi;

fn main() {
  match openapi::from_path("path/to/openapi.yaml") {
    Ok(spec) => println!("spec: {:?}", spec),
    Err(err) => println!("error: {}", err)
  }
}
```

Doug Tangren (softprops) 2017
