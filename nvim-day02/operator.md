# Operator & Motion in Neovim

## The core idea

An operator waits for a motion:

    [operator] + [motion] = action

Example: `dw` = delete to the next word. `c$` = change to end of line.

## Main operators

- `d` — delete.
- `c` — change (delete + enter insert mode).
- `y` — yank (copy).
- `p` / `P` — paste after / before the cursor.

## Line shortcuts

- `dd` — delete one line.
- `cc` — change one line.
- `yy` — yank one line.
- `D` — delete from cursor to end of line.
- `C` — change from cursor to end of line.
- `x` — delete one character.
- `s` — delete one character and enter insert mode.
- `S` — same as `cc`.
- `r` — replace one character (stays in normal mode).
- `R` — enter replace mode.

## Counts

- `3dd` — delete 3 lines.
- `2dw` — delete 2 words.
- `d2w` — delete 2 words (motion with count).
- `5j` — move down 5 lines.
- `3p` — paste 3 times.

## Change with text objects

- `ciw` — change inner word.
- `cw` — change to end of word.
- `ci"` — change inside double quotes.
- `ci(` — change inside parentheses.

## Undo and redo

- `u` — undo.
- `Ctrl+r` — redo.
- `U` — undo the whole line (built-in).

## Common traps

- `p` overwrites the default register. After `y` then `d`, `p` pastes the deleted text. Use `"0p` for the last yank.
- `dw` in the middle of a word does not delete the whole word. Use `diw` for that.
- `x` deletes, `s` deletes and enters insert.
- `r` replaces one character, `R` enters replace mode.
