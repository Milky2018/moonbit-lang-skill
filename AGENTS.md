## Common Pitfalls

- Use `func() |> ignore` not `let _ = func()`
- Use `!condition` not `not(condition)`
- Use `inspect(value)` not `inspect!(value)` (deprecated)
- Use `for i in 0..<n` not C-style `for i = 0; i < n; i = i + 1`
- Use `if opt is Some(v) { ... }` for single-branch matching
- Use `arr.clear()` not `while arr.length() > 0 { arr.pop() }`
- Use `s.code_unit_at(i)` not `s[i]` (deprecated)
- Use `pub(all) enum` not factory functions for simple enums
- Use `let mut` only for reassignment, not for mutable containers like Array
- Use `reinterpret_as_uint()` for unsigned ops, `to_int()` for numeric conversion
- Use `try! func() |> ignore` to ignore errors, `raise` to throw
- Use `func() catch { e => ... }` not `match (try? func()) { Ok(_) => ...; Err(_) => ...}`
