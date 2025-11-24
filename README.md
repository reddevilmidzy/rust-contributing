# 🗺🦀 rust contributing
> Let's contribute to [rust-lang](https://github.com/rust-lang)


## [rust](https://github.com/rust-lang/rust)

### PR
> Create Pull Requests

- **[#149258](https://github.com/rust-lang/rust/pull/149258)**: Fix None handling for simplify_type in for_each_relevant_impl 
- **[#149255](https://github.com/rust-lang/rust/pull/149255)**: Use `let...else` consistently in user-facing diagnostics
- **[#149179](https://github.com/rust-lang/rust/pull/149179)**: Add regression test for 128705
- **[#149101](https://github.com/rust-lang/rust/pull/149101)**: Improve mutable-binding suggestion to include name
- **[#149027](https://github.com/rust-lang/rust/pull/149027)**: Implement method signature suggestion for trait mismatches error
- **[#148785](https://github.com/rust-lang/rust/pull/148785)**: Replace master branch references with main
- **[#148775](https://github.com/rust-lang/rust/pull/148775)**: Fix a typo in the documentation for the strict_shr function
- **[#148526](https://github.com/rust-lang/rust/pull/148526)**: Expand pow docs with special-case tests
- **[#147845](https://github.com/rust-lang/rust/pull/147845)**: Add regression test for 134355
- **[#147438](https://github.com/rust-lang/rust/pull/147438)**: Rename "non-inline module" to "file module" in proc macro diagnostics
- **[#147395](https://github.com/rust-lang/rust/pull/147395)**: Improve diagnostics: update note and add help message
- **[#147269](https://github.com/rust-lang/rust/pull/147269)**: Add regression test for 123953
- **[#140819](https://github.com/rust-lang/rust/pull/140819)**: Add regression test for 125877
- **[#140574](https://github.com/rust-lang/rust/pull/140574)**: Add regression test for 133065
- **[#140205](https://github.com/rust-lang/rust/pull/140205)**: Tidying up UI tests [2/N]
- **[#140029](https://github.com/rust-lang/rust/pull/140029)**: Tidying up UI tests [1/N]
- **[#139893](https://github.com/rust-lang/rust/pull/139893)**: Add test for issue 125668
- **[#139778](https://github.com/rust-lang/rust/pull/139778)**: Add test for issue 34834
- **[#139607](https://github.com/rust-lang/rust/pull/139607)**: Add regression test for #127424
- **[#138509](https://github.com/rust-lang/rust/pull/138509)**: Add test to ensure no index out of bounds panic (#135474)
- **[#138105](https://github.com/rust-lang/rust/pull/138105)**: Fix broken link to Miri intrinsics in documentation

### Issue
> Create Issues

- **[#149181](https://github.com/rust-lang/rust/issues/149181)**: E0038 is emitted 2 or 3 times for the same line
- **[#140235](https://github.com/rust-lang/rust/issues/140235)**: Compiler misinterprets cast and comparison as generic syntax
- **[#137486](https://github.com/rust-lang/rust/issues/137486)**: fix suggestion for E0716 (temporary value dropped while borrowed)

### Participated in issue
> Add some code snippet, classify label and find duplicated issue
 
- **[#149155](https://github.com/rust-lang/rust/issues/149155)**: ICE: Option::unwrap() on a None value
- **[#149055](https://github.com/rust-lang/rust/issues/149055)**: panic at compiler/rustc_metadata/src/rmeta/def_path_hash_map.rs:18:54
- **[#148581](https://github.com/rust-lang/rust/issues/148581)**: thread 'rustc' panicked at compiler/rustc_metadata/src/rmeta/def_path_hash_map.rs:23:54: called `Option::unwrap()` on a None value
- **[#148809](https://github.com/rust-lang/rust/issues/148809)**: ICE: compiler paniced and panicked while processing panic, program terminated with signal: SIGSEGV
- **[#142482](https://github.com/rust-lang/rust/issues/142482)**: `this method is equivalent to` section of `Vec::extract_if` seems incorrect
- **[#141400](https://github.com/rust-lang/rust/issues/141400)**: ICE: layout_of: unexpected type
- **[#137588](https://github.com/rust-lang/rust/issues/137588)**: ICE: index out of bounds: the len is 0 but the index is `18446744073709551615`
- **[#128705](https://github.com/rust-lang/rust/issues/128705)**: E0038 emmitted twice

### Code review
> Add comments

- **[#149272](https://github.com/rust-lang/rust/pull/149272)**: Fix vec iter zst alignment 148682
- **[#149262](https://github.com/rust-lang/rust/pull/149262)**: build: update checkout action to v6
- **[#149144](https://github.com/rust-lang/rust/pull/149144)**: Reject async fn in const impl during AST validation
- **[#149045](https://github.com/rust-lang/rust/pull/149045)**: implement PartialEq<Vec<U>> for [T; N] and &[T; N]

---

## [rust-clippy](https://github.com/rust-lang/rust-clippy)

### PR

- **[#15448](https://github.com/rust-lang/rust-clippy/pull/15448)**: Update CONTRIBUTING.md to use RustRover instead of IntelliJ Rust

### Issue

- **[#15883](https://github.com/rust-lang/rust-clippy/issues/15883)**: `semicolon_if_nothing_returned` shows incorrect line number for method call with multi-line closure
- **[#15463](https://github.com/rust-lang/rust-clippy/issues/15463)**: Consider renaming `cargo dev setup intellij` to `cargo dev setup rustrover`
- **[#15406](https://github.com/rust-lang/rust-clippy/issues/15406)**: Update CONTRIBUTING.md to include RustRover instead of deprecated IntelliJ Rust

---

## [book](https://github.com/rust-lang/book)

### PR

- **[#4553](https://github.com/rust-lang/book/pull/4553)**: Fix incorrect link for chapter 16 reference

---

## [git2-rs](https://github.com/rust-lang/git2-rs)

### PR

- **[#1155](https://github.com/rust-lang/git2-rs/pull/1155)**: fix: add a backtick

---

## [blog.rust-lang.org](https://github.com/rust-lang/blog.rust-lang.org)

### PR

- **[#1738](https://github.com/rust-lang/blog.rust-lang.org/pull/1738)**: Fix link in `renaming-the-default-branch-of-rust-lang-rust.md`

---

## [rustc-dev-guide](https://github.com/rust-lang/rustc-dev-guide)

### PR

- **[#2654](https://github.com/rust-lang/rustc-dev-guide/pull/2654)**: Fix link to README in ui test documentation
