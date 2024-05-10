# Rust hooks for pre-commit

[Rust](https://www.rust-lang.org) tools package for [pre-commit](https://pre-commit.com), using nightly versions of Rust.

## Using rust tools with pre-commit

```yaml
- repo: https://github.com/pxeger/pre-commit-rust
  rev: master
  hooks:
  - id: fmt
  - id: cargo-check
```

## Passing arguments to rustfmt

```yaml
- repo: https://github.com/pxeger/pre-commit-rust
  rev: master
  hooks:
  - id: fmt
    args: ['--verbose', '--edition', '2018', '--']
```
