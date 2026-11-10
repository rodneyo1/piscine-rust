# Piscine Rust

95 Rust exercises from the Zone01 Kisumu piscine. They go from the basics (variables, loops, strings) up to advanced topics: the borrow checker, lifetimes, traits, generics, iterators, smart pointers and error handling.

Each folder is its own Cargo crate with a small library and tests.

```bash
cd ownership
cargo test
```

## Concepts covered

### Basics: types, control flow, functions
Integer and float types, overflow, arithmetic, loops, recursion, tuples and arrays.

`scalar` · `temperature_conv` · `division_and_remainder` · `speed_transformation` · `looping` · `find_factorial` · `fibonacci2` · `logic_number` · `stars` · `diamond_creation` · `ordinal` · `talking` · `arrays` · `tuples_refs` · `tic_tac_toe`

### Ownership and the borrow checker
Moves vs copies, shared and mutable references, borrowing rules, and lifetimes.

`ownership` · `borrow` · `borrow_me_the_reference` · `copy` · `doubtful` · `changes` · `tuples_refs` · `lifetimes`

### Strings and text processing
`String` vs `&str`, slicing, UTF-8, case changes, ciphers and parsing.

`strings` · `string_literals` · `reverse_string` · `capitalizing` · `delete_prefix` · `name_initials` · `pig_latin` · `pangram` · `spelling` · `to_url` · `profanity_filter` · `arrange_it` · `expected_variable` · `string_permutation` · `edit_distance` · `rot` · `cipher` · `scytale_cipher` · `roman_numbers`

### Collections and data manipulation
`Vec`, `HashMap`, slices, sorting, searching, grouping and aggregating data.

`collect` · `hashing` · `simple_hash` · `slices_to_map` · `bigger` · `highest` · `scores` · `searching` · `get_products` · `groceries` · `sales` · `shopping_mall` · `mobs` · `commits_stats`

### Structs, enums and pattern matching
Modelling data with structs and enums, `impl` blocks, `match` and `Option`.

`circle` · `rgb_match` · `blood_types` · `card_deck` · `does_it_fit` · `events` · `middle_day` · `shopping_mall` · `mobs`

### Traits and generics
Defining and implementing traits, operator overloading, generic types, trait bounds and trait objects (`dyn`).

`traits` · `easy_traits` · `generics` · `generics_list` · `border_cross` · `vector_operations` · `lalgebra_scalar` · `lalgebra_vector` · `matrix` · `matrix_ops` · `matrix_mult` · `matrix_transposition`

### Closures and iterators
Closures that capture state, iterator adapters, and writing custom `Iterator` implementations.

`closures` · `adding` · `adding_twice` · `iterators` · `step_iterator` · `project_motion` · `roman_numbers_iter`

### Smart pointers: basic to advanced
`Box` for heap data and recursive types, `Rc` for shared ownership and reference counting, `RefCell` for interior mutability, and the `Drop` trait.

`box_it` · `borrow_box` · `box_recursion` · `boxing_todo` · `how_many_references` · `ref_cell` · `drop_the_thread`

### Error handling
`panic!`, `Result`, `Option`, the `?` operator, `unwrap`/`expect`, custom error types and reading files.

`panic` · `unwrap_or_expect` · `question_mark` · `error_types` · `handling` · `banner` · `boxing_todo`

### Crates and modules
Using external crates from crates.io, and local crates that depend on each other through path dependencies.

- `chrono`: dates and times (`events`, `middle_day`, `commits_stats`, `error_types`)
- `json` and `serde`: parsing and serialising data (`commits_stats`, `macro_calculator`, `boxing_todo`)
- `rand`: random card draws (`card_deck`)
- `colored`: coloured terminal output (`events`)
- `case`: case conversion (`expected_variable`)
- Local path crates: `lalgebra_vector` and the matrix exercises build on `lalgebra_scalar`, and `expected_variable` reuses `edit_distance`
