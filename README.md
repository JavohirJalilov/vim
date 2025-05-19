# Vim Context-Aware Actions Cheat Sheet

## Basic Modes

- `i`, `I` — Enter insert mode (insert at cursor / beginning of line)

## Cursor Movement

- `h`, `j`, `k`, `l` — Move left, down, up, right
- `w` — Move to the beginning of the next word
- `b` — Move to the beginning of the previous word
- `e` — Move to the end of the current/next word
- `ge` — Move to the end of the previous word
- `[n][movement]` — Repeat movement `n` times (e.g., `3w` moves 3 words forward)
- `f<char>` — Move to next occurrence of `<char>` in line
- `F<char>` — Move to previous occurrence of `<char>` in line
- `;`, `,` — Repeat last `f` or `F` (forward / backward)
- `0` — Move to beginning of the line
- `$` — Move to end of the line
- `%` — Go to matching parenthesis, bracket, or brace
- `gg` — Go to the beginning of the file
- `G` — Go to the end of the file

## Editing Text

- `x`, `X` — Delete character under (x) / before (X) the cursor
- `a`, `A` — Append after cursor / end of line
- `o`, `O` — Open new line below / above and enter insert mode
- `d[movement]` — Delete text covered by movement (e.g., `dw` deletes to next word)
- `D` — Delete to end of the line
- `r<char>` — Replace character under cursor with `<char>`
- `ci[movement]` — Change inside specified movement (e.g., `ci"` changes inside quotes)
- `S` — Delete line and enter insert mode

## Copy and Paste

- `yy` — Yank (copy) current line
- `p` — Paste yanked text after the cursor

## Searching

- `/yourtext` — Search for “yourtext”
  - `n` — Repeat search forward
  - `N` — Repeat search backward
