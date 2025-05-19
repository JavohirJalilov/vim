# 📝 Vim Full Cheat Sheet

## 🧭 Modes
- `i` — Insert before cursor
- `I` — Insert at beginning of line
- `a` — Append after cursor
- `A` — Append at end of line
- `o` — Open line below
- `O` — Open line above
- `Esc` — Return to Normal mode
- `v` — Visual mode (characterwise)
- `V` — Visual Line mode
- `Ctrl+v` — Visual Block mode
- `:` — Command-line mode

---

## 🎯 Cursor Movement
### Line & File
- `h`, `j`, `k`, `l` — Left, down, up, right
- `0` — Start of line
- `^` — First non-blank of line
- `$` — End of line
- `gg` — Start of file
- `G` — End of file
- `:n` — Go to line `n`

### Words
- `w` — Start of next word
- `W` — Next word (by whitespace)
- `b` — Start of previous word
- `B` — Previous word (by whitespace)
- `e` — End of current/next word
- `E` — End of word (by whitespace)

### Search
- `/text` — Search forward
- `?text` — Search backward
- `n` — Repeat search forward
- `N` — Repeat search backward

### Find Character
- `f<char>` — Find next `<char>` on line
- `F<char>` — Find previous `<char>`
- `t<char>` — To before next `<char>`
- `T<char>` — To before previous `<char>`
- `;` — Repeat last `f`, `t`, `F`, or `T`
- `,` — Reverse repeat

---

## ✂️ Editing
- `x` — Delete character under cursor
- `X` — Delete before cursor
- `r<char>` — Replace character
- `u` — Undo
- `Ctrl+r` — Redo
- `.` — Repeat last change

### Delete (with motions)
- `d{motion}` — Delete (e.g. `dw`, `d$`)
- `dd` — Delete line
- `D` — Delete to end of line

### Change
- `c{motion}` — Change (e.g. `cw`, `c$`)
- `cc` — Change whole line
- `C` — Change to end of line
- `S` — Change whole line (`cc`)
- `ci"` — Change inside quotes (replace `" "` content)
- `ca"` — Change around quotes (replace including `" "`)

### Copy & Paste
- `yy` — Yank (copy) line
- `y{motion}` — Yank motion
- `p` — Paste after cursor
- `P` — Paste before cursor

---

## 🔁 Repeating & Counts
- `{n}` before command — Repeat command `n` times (e.g. `3dw`)
- `.` — Repeat last command
- `@a` — Run macro `a`
- `@@` — Repeat last macro

---

## 🗃️ Buffers, Tabs, and Windows
### Buffers
- `:e filename` — Edit file
- `:bnext` / `:bn` — Next buffer
- `:bprev` / `:bp` — Previous buffer
- `:ls` or `:buffers` — List buffers
- `:bd` — Delete buffer

### Tabs
- `:tabnew filename` — Open in new tab
- `gt` — Next tab
- `gT` — Previous tab
- `:tabclose` — Close tab

### Windows (Splits)
- `:split filename` — Horizontal split
- `:vsplit filename` — Vertical split
- `Ctrl+w s` — Split current window horizontally
- `Ctrl+w v` — Split current window vertically
- `Ctrl+w w` — Switch window
- `Ctrl+w h/j/k/l` — Move between splits
- `Ctrl+w q` — Close current split

---

## 🔍 Search & Replace
- `:%s/old/new/g` — Replace all in file
- `:s/old/new/g` — Replace all in current line
- `:%s/old/new/gc` — Replace with confirmation
- `:noh` — Turn off highlight

---

## 🧠 Macros
- `q{a-z}` — Start recording into register
- Perform commands
- `q` — Stop recording
- `@a` — Play macro `a`
- `@@` — Repeat last macro

---

## 🔐 Registers
- `"ayy` — Yank line into register `a`
- `"ap` — Paste from register `a`
- `:reg` — Show registers

---

## 🛠️ Misc
- `:w` — Save
- `:q` — Quit
- `:wq` or `ZZ` — Save and quit
- `:q!` — Force quit
- `:x` — Save if changed and quit
- `:!cmd` — Run shell command
- `:set number` — Show line numbers
- `:set relativenumber` — Relative line numbers

---

## 🏁 Useful Command Combos
- `ci"` — Change content inside quotes
- `di(` — Delete inside parentheses
- `va{` — Select around curly braces (Visual mode)
- `:syntax on` — Enable syntax highlighting
- `:set paste` — Prevent auto-indent on paste

---

## 📚 Help
- `:help` — Open help
- `:help keyword` — Help for `keyword`
- `K` — Open man page for word under cursor

---

## ✅ Best Practices
- Use `hjkl` for movement
- Combine operators and motions: `d`, `c`, `y`, etc.
- Use Visual mode for block selection (`Ctrl+v`)
- Record macros for repetitive tasks
