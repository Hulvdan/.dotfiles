# ideavimconfig

## 0. Personally Overridden

| shortcut    | action    |
| ----------- | --------- |
| `<leader>w` | save file |

## 1. Insert mode                                          *insert-index*

| tag               | char                     | action                                                                        |
| ----------------- | ------------------------ | ----------------------------------------------------------------------------- |
| `i_CTRL-@`        | `CTRL-@`                 | insert previously inserted text and stop insert                               |
| `i_CTRL-A`        | `CTRL-A`                 | insert previously inserted text                                               |
|                   | `CTRL-B`                 | not used                                                                      |
| `i_CTRL-C`        | `CTRL-C`                 | quit insert mode, without checking for abbreviation, unless 'insertmode' set. |
| `i_CTRL-D`        | `CTRL-D`                 | delete one shiftwidth of indent in the current line                           |
| `i_CTRL-E`        | `CTRL-E`                 | insert the character which is below the cursor                                |
|                   | `CTRL-F`                 | not used (but by default it's in 'cinkeys' to re-indent the current line)     |
| `i_<BS>`          | `<BS>`                   | delete character before the cursor                                            |
| `i_digraph`       | `{char1}<BS>{char2}`     | enter digraph (only when 'digraph' option set)                                |
| `i_CTRL-H`        | `CTRL-H`                 | same as <BS>                                                                  |
| `i_<Tab>`         | `<Tab>`                  | insert a <Tab> character                                                      |
| `i_CTRL-I`        | `CTRL-I`                 | same as <Tab>                                                                 |
| `i_<NL>`          | `<NL>`                   | same as <CR>                                                                  |
| `i_CTRL-J`        | `CTRL-J`                 | same as <CR>                                                                  |
| `i_CTRL-K`        | `CTRL-K {char1} {char2}` | enter digraph                                                                 |
| `i_<CR>`          | `<CR>`                   | begin new line                                                                |
| `i_CTRL-M`        | `CTRL-M`                 | same as <CR>                                                                  |
| `i_CTRL-O`        | `CTRL-O`                 | execute a single command and return to insert mode                            |
| `i_CTRL-R`        | `CTRL-R {0-9a-z"%#*:=}`  | insert the contents of a register                                             |
| `i_CTRL-T`        | `CTRL-T`                 | insert one shiftwidth of indent in currentline                                |
| `i_CTRL-U`        | `CTRL-U`                 | delete all entered characters in the current line                             |
| `i_CTRL-V_digit`  | `CTRL-V {number}`        | insert three digit decimal number as a single byte.                           |
| `i_CTRL-W`        | `CTRL-W`                 | delete word before the cursor                                                 |
| `i_CTRL-Y`        | `CTRL-Y`                 | insert the character which is above the cursor                                |
| `i_<Esc>`         | `<Esc>`                  | end insert mode (unless 'insertmode' set)                                     |
| `i_CTRL-[`        | `CTRL-[`                 | same as <Esc>                                                                 |
| `i_CTRL-\_CTRL-N` | `CTRL-\ CTRL-N`          | go to Normal mode                                                             |
|                   | `CTRL-\ a - z`           | reserved for extensions                                                       |
|                   | `CTRL-\ others`          | not used                                                                      |
| `i_0_CTRL-D`      | `0 CTRL-D`               | delete all indent in the current line                                         |
| `i_<Del>`         | `<Del>`                  | delete character under the cursor                                             |
| `i_<Left>`        | `<Left>`                 | cursor one character left                                                     |
| `i_<S-Left>`      | `<S-Left>`               | cursor one word left                                                          |
| `i_<C-Left>`      | `<C-Left>`               | cursor one word left                                                          |
| `i_<Right>`       | `<Right>`                | cursor one character right                                                    |
| `i_<S-Right>`     | `<S-Right>`              | cursor one word right                                                         |
| `i_<C-Right>`     | `<C-Right>`              | cursor one word right                                                         |
| `i_<Up>`          | `<Up>`                   | cursor one line up                                                            |
| `i_<S-Up>`        | `<S-Up>`                 | same as <PageUp>                                                              |
| `i_<Down>`        | `<Down>`                 | cursor one line down                                                          |
| `i_<S-Down>`      | `<S-Down>`               | same as <PageDown>                                                            |
| `i_<Home>`        | `<Home>`                 | cursor to start of line                                                       |
| `i_<C-Home>`      | `<C-Home>`               | cursor to start of file                                                       |
| `i_<End>`         | `<End>`                  | cursor past end of line                                                       |
| `i_<C-End>`       | `<C-End>`                | cursor past end of file                                                       |
| `i_<PageUp>`      | `<PageUp>`               | one screenfull backward                                                       |
| `i_<PageDown>`    | `<PageDown>`             | one screenfull forward                                                        |
| `i_<F1>`          | `<F1>`                   | same as <Help>                                                                |
| `i_<Help>`        | `<Help>`                 | stop insert mode and display help window                                      |
| `i_<Insert>`      | `<Insert>`               | toggle Insert/Replace mode                                                    |
| `i_<LeftMouse>`   | `<LeftMouse>`            | cursor at mouse click                                                         |

## 2. Normal mode                                          *normal-index*

CHAR     any non-blank character
WORD     a sequence of non-blank characters
N        a number entered before the command
{motion} a cursor movement command
Nmove    the text that is moved over with a {motion}
SECTION  a section that possibly starts with '}' instead of '{'

note: 1 = cursor movement command; 2 = can be undone/redone

| tag             | char                 | note | action in Normal mode                                                                                                                               |
| --------------- | -------------------- | ---- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
|                 | `CTRL-@`             |      | not used                                                                                                                                            |
| `CTRL-A`        | `CTRL-A`             | 2    | add N to number at/after cursor                                                                                                                     |
| `CTRL-B`        | `CTRL-B`             | 1    | scroll N screens Backwards                                                                                                                          |
| `CTRL-D`        | `CTRL-D`             |      | scroll Down N lines (default: half a screen)                                                                                                        |
| `CTRL-E`        | `CTRL-E`             |      | scroll N lines upwards (N lines Extra)                                                                                                              |
| `CTRL-F`        | `CTRL-F`             | 1    | scroll N screens Forward                                                                                                                            |
| `CTRL-G`        | `CTRL-G`             |      | display current file name and position                                                                                                              |
| `<BS>`          | `<BS>`               | 1    | same as "h"                                                                                                                                         |
| `CTRL-H`        | `CTRL-H`             | 1    | same as "h"                                                                                                                                         |
| `<Tab>`         | `<Tab>`              | 1    | go to N newer entry in jump list                                                                                                                    |
| `CTRL-I`        | `CTRL-I`             | 1    | same as <Tab>                                                                                                                                       |
| `<NL>`          | `<NL>`               | 1    | same as "j"                                                                                                                                         |
| `CTRL-J`        | `CTRL-J`             | 1    | same as "j"                                                                                                                                         |
|                 | `CTRL-K`             |      | not used                                                                                                                                            |
| `<CR>`          | `<CR>`               | 1    | cursor to the first CHAR N lines lower                                                                                                              |
| `CTRL-M`        | `CTRL-M>`            | 1    | same as <CR>                                                                                                                                        |
| `CTRL-N`        | `CTRL-N`             | 1    | same as "j"                                                                                                                                         |
| `CTRL-O`        | `CTRL-O`             | 1    | go to N older entry in jump list                                                                                                                    |
| `CTRL-P`        | `CTRL-P`             | 1    | cursor N lines upward                                                                                                                               |
|                 | `CTRL-Q`             |      | (used for terminal control flow)                                                                                                                    |
| `CTRL-R`        | `CTRL-R`             | 2    | redo changes which were undone with 'u'                                                                                                             |
|                 | `CTRL-S`             |      | not used                                                                                                                                            |
| `CTRL-U`        | `CTRL-U`             |      | scroll N lines Upwards (default: half a screen)                                                                                                     |
| `CTRL-V`        | `CTRL-V`             |      | start blockwise Visual mode                                                                                                                         |
| `CTRL-X`        | `CTRL-X`             | 2    | subtract N from number at/after cursor                                                                                                              |
| `CTRL-Y`        | `CTRL-Y`             |      | scroll N lines downwards                                                                                                                            |
|                 | `CTRL-[ <Esc>`       |      | not used                                                                                                                                            |
| `CTRL-\_CTRL-N` | `CTRL-\ CTRL-N`      |      | go to Normal mode (no-op)                                                                                                                           |
|                 | `CTRL-\ a - z`       |      | reserved for extensions                                                                                                                             |
|                 | `CTRL-\ others`      |      | not used                                                                                                                                            |
| `CTRL-^`        | `CTRL-^`             |      | edit Nth alternate file (equivalent to                                                                                                              |
|                 | `                    | `    | ":e #N")                                                                                                                                            |
|                 | `CTRL-_`             |      | not used                                                                                                                                            |
| `<Space>`       | `<Space>`            | 1    | same as "l"                                                                                                                                         |
| `!!`            | `!!{filter}`         | 2    | filter N lines through the {filter} command                                                                                                         |
| `quote`         | `"{a-zA-Z0-9.%#:-"}` |      | use buffer {a-zA-Z0-9.%#:-"} for next delete, yank or put (uppercase to append) ({.%#:} only work with put)                                         |
| `#`             | `#`                  | 1    | search backward for the Nth occurrence of the ident under the cursor                                                                                |
| `$`             | `$`                  | 1    | cursor to the end of Nth next line                                                                                                                  |
| `%`             | `%`                  | 1    | find the next (curly/square) bracket on this line and go to its match, or go to matching comment bracket, or go to matching preprocessor directive. |
| `N%`            | `{count}%`           | 1    | go to N percentage in the file                                                                                                                      |
| `&`             | `&`                  | 2    | repeat last :s                                                                                                                                      |
| `'`             | `'{a-zA-Z0-9}`       | 1    | cursor to the first CHAR on the line with mark {a-zA-Z0-9}                                                                                          |
| `''`            | `''`                 | 1    | cursor to the first CHAR of the line where the cursor was before the latest jump.                                                                   |
| `'(`            | `'(`                 | 1    | cursor to the first CHAR on the line of the start of the current sentence                                                                           |
| `')`            | `')`                 | 1    | cursor to the first CHAR on the line of the end of the current sentence                                                                             |
| `'<`            | `'<`                 | 1    | cursor to the first CHAR of the line where highlighted area starts/started in the current buffer.                                                   |
| `'>`            | `'>`                 | 1    | cursor to the first CHAR of the line where highlighted area ends/ended in the current buffer.                                                       |
| `'[`            | `'[`                 | 1    | cursor to the first CHAR on the line of the start of last operated text or start of putted text                                                     |
| `']`            | `']`                 | 1    | cursor to the first CHAR on the line of the end of last operated text or end of putted text                                                         |
| `'{`            | `'{`                 | 1    | cursor to the first CHAR on the line of the start of the current paragraph                                                                          |
| `'}`            | `'}`                 | 1    | cursor to the first CHAR on the line of the end of the current paragraph                                                                            |
| `(`             | `(`                  | 1    | cursor N sentences backward                                                                                                                         |
| `)`             | `)`                  | 1    | cursor N sentences forward                                                                                                                          |
| `star`          | `*`                  | 1    | search forward for the Nth occurrence of the ident under the cursor                                                                                 |
| `+`             | `+`                  | 1    | cursor to the first CHAR N lines lower                                                                                                              |
| `,`             | `,`                  | 1    | repeat latest f, t, F or T in opposite direction N times                                                                                            |
| `-`             | `-`                  | 1    | cursor to the first CHAR N lines higher                                                                                                             |
| `.`             | `.`                  | 2    | repeat last change with count replaced with N                                                                                                       |
| `/`             | `/{pattern}<CR>`     | 1    | search forward for the Nth occurrence of {pattern}                                                                                                  |
| `/<CR>`         | `/<CR>`              | 1    | search forward for {pattern} of last search                                                                                                         |
| `count`         | `0`                  | 1    | cursor to the first char of the line                                                                                                                |
| `count`         | `1`                  |      | prepend to command to give a count                                                                                                                  |
| `count`         | `2`                  |      | "                                                                                                                                                   |
| `count`         | `3`                  |      | "                                                                                                                                                   |
| `count`         | `4`                  |      | "                                                                                                                                                   |
| `count`         | `5`                  |      | "                                                                                                                                                   |
| `count`         | `6`                  |      | "                                                                                                                                                   |
| `count`         | `7`                  |      | "                                                                                                                                                   |
| `count`         | `8`                  |      | "                                                                                                                                                   |
| `count`         | `9`                  |      | "                                                                                                                                                   |
| `:`             | `:`                  | 1    | start entering an Ex command                                                                                                                        |
| `N:`            | `{count}:`           |      | start entering an Ex command with range from current line to N lines down                                                                           |
| `;`             | `;`                  | 1    | repeat latest f, t, F or T N times                                                                                                                  |
| `<`             | `<{motion}`          | 2    | shift Nmove lines one 'shiftwidth' leftwards                                                                                                        |
| `<<`            | `<<`                 | 2    | shift N lines one 'shiftwidth' leftwards                                                                                                            |
| `==`            | `==`                 | 2    | filter N lines through "indent"                                                                                                                     |
| `>`             | `>{motion}`          | 2    | shift Nmove lines one 'shiftwidth' rightwards                                                                                                       |
| `>>`            | `>>`                 | 2    | shift N lines one 'shiftwidth' rightwards                                                                                                           |
| `?`             | `?{pattern}<CR>`     | 1    | search backward for the Nth previous occurrence of {pattern}                                                                                        |
| `?<CR>`         | `?<CR>`              | 1    | search backward for {pattern} of last search                                                                                                        |
| `@`             | `@{a-z}`             | 2    | execute the contents of named buffer {a-z} N times                                                                                                  |
| `@:`            | `@:`                 |      | repeat the previous ":" command N times                                                                                                             |
| `@@`            | `@@`                 | 2    | repeat the previous @{a-z} N times                                                                                                                  |
| `A`             | `A`                  | 2    | append text after the end of the line N times                                                                                                       |
| `B`             | `B`                  | 1    | cursor N WORDS backward                                                                                                                             |
| `C`             | `["x]C`              | 2    | change from the cursor position to the end of the line, and N-1 more lines [into buffer x]; synonym for "c$"                                        |
| `D`             | `["x]D`              | 2    | delete the characters under the cursor until the end of the line and N-1 more lines [into buffer x]; synonym for "d$"                               |
| `E`             | `E`                  | 1    | cursor forward to the end of WORD N                                                                                                                 |
| `F`             | `F{char}`            | 1    | cursor to the Nth occurrence of {char} to the left                                                                                                  |
| `G`             | `G`                  | 1    | cursor to line N, default last line                                                                                                                 |
| `H`             | `H`                  | 1    | cursor to line N from top of screen                                                                                                                 |
| `I`             | `I`                  | 2    | insert text before the first CHAR on the line N times                                                                                               |
| `J`             | `J`                  | 2    | Join N lines; default is 2                                                                                                                          |
| `K`             | `K`                  |      | lookup Keyword under the cursor with 'keywordprg'                                                                                                   |
| `L`             | `L`                  | 1    | cursor to line N from bottom of screen                                                                                                              |
| `M`             | `M`                  | 1    | cursor to middle line of screen                                                                                                                     |
| `N`             | `N`                  | 1    | repeat the latest '/' or '?' N times in opposite direction                                                                                          |
| `O`             | `O`                  | 2    | begin a new line above the cursor and insert text, repeat N times                                                                                   |
| `P`             | `["x]P`              | 2    | put the text [from buffer x] before the cursor N times                                                                                              |
| `R`             | `R`                  | 2    | enter replace mode: overtype existing characters, repeat the entered text N-1 times                                                                 |
| `S`             | `["x]S`              | 2    | delete N lines [into buffer x] and start insert; synonym for "^cc" or "0cc", depending on autoindent                                                |
| `T`             | `T{char}`            | 1    | cursor till after Nth occurrence of {char} to the left                                                                                              |
| `V`             | `V`                  |      | start linewise Visual mode                                                                                                                          |
| `W`             | `W`                  | 1    | cursor N WORDS forward                                                                                                                              |
| `X`             | `["x]X`              | 2    | delete N characters before the cursor [into buffer x]                                                                                               |
| `Y`             | `["x]Y`              |      | yank N lines [into buffer x]; synonym for "yy"                                                                                                      |
| `ZZ`            | `ZZ`                 |      | store current file if modified, and exit                                                                                                            |
| `ZQ`            | `ZQ`                 |      | exit current file always                                                                                                                            |
| `[`             | `[{char}`            |      | square bracket command (see below)                                                                                                                  |
|                 | `\`                  |      | not used                                                                                                                                            |
| `]`             | `]{char}`            |      | square bracket command (see below)                                                                                                                  |
| `^`             | `^`                  | 1    | cursor to the first CHAR of the line                                                                                                                |
| `_`             | `_`                  | 1    | cursor to the first CHAR N - 1 lines lower                                                                                                          |
| `` ` ``         | `` `{a-zA-Z0-9} ``   | 1    | cursor to the mark {a-zA-Z0-9}                                                                                                                      |
| `` `( ``        | `` `( ``             | 1    | cursor to the start of the current sentence                                                                                                         |
| `` `) ``        | `` `) ``             | 1    | cursor to the end of the current sentence                                                                                                           |
| `` `< ``        | `` `< ``             | 1    | cursor to the start of the highlighted area                                                                                                         |
| `` `> ``        | `` `> ``             | 1    | cursor to the end of the highlighted area                                                                                                           |
| `` `[ ``        | `` `[ ``             | 1    | cursor to the start of last operated text or start of putted text                                                                                   |
| `` `] ``        | `` `] ``             | 1    | cursor to the end of last operated text or end of putted text                                                                                       |
| `` ` ``         | `` ` ``              | 1    | cursor to the position before latest jump                                                                                                           |
| `` `{ ``        | `` `{ ``             | 1    | cursor to the start of the current paragraph                                                                                                        |
| `` `} ``        | `` `} ``             | 1    | cursor to the end of the current paragraph                                                                                                          |
| `a`             | `a`                  | 2    | append text after the cursor N times                                                                                                                |
| `b`             | `b`                  | 1    | cursor N words backward                                                                                                                             |
| `c`             | `["x]c{motion}`      | 2    | delete Nmove text [into buffer x] and start insert                                                                                                  |
| `cc`            | `["x]cc`             | 2    | delete N lines [into buffer x] and start insert                                                                                                     |
| `d`             | `["x]d{motion}`      | 2    | delete Nmove text [into buffer x]                                                                                                                   |
| `dd`            | `["x]dd`             | 2    | delete N lines [into buffer x]                                                                                                                      |
| `e`             | `e`                  | 1    | cursor forward to the end of word N                                                                                                                 |
| `f`             | `f{char}`            | 1    | cursor to Nth occurrence of {char} to the right                                                                                                     |
| `g`             | `g{char}`            |      | extended commands, see below                                                                                                                        |
| `h`             | `h`                  | 1    | cursor N chars to the left                                                                                                                          |
| `i`             | `i`                  | 2    | insert text before the cursor N times                                                                                                               |
| `j`             | `j`                  | 1    | cursor N lines downward                                                                                                                             |
| `k`             | `k`                  | 1    | cursor N lines upward                                                                                                                               |
| `l`             | `l`                  | 1    | cursor N chars to the right                                                                                                                         |
| `m`             | `m{A-Za-z}`          |      | set mark {A-Za-z} at cursor position                                                                                                                |
| `n`             | `n`                  | 1    | repeat the latest '/' or '?' N times                                                                                                                |
| `o`             | `o`                  | 2    | begin a new line below the cursor and insert text, repeat N times                                                                                   |
| `p`             | `["x]p`              | 2    | put the text [from register x] after the cursor N times                                                                                             |
| `q`             | `q{0-9a-zA-Z"}`      |      | record typed characters into named register {0-9a-zA-Z"} (uppercase to append)                                                                      |
| `q`             | `q`                  |      | (while recording) stops recording                                                                                                                   |
| `r`             | `r{char}`            | 2    | replace N chars with {char}                                                                                                                         |
| `s`             | `["x]s`              | 2    | (substitute) delete N characters [into buffer x] and start insert                                                                                   |
| `t`             | `t{char}`            | 1    | cursor till before Nth occurrence of {char} to the right                                                                                            |
| `u`             | `u`                  | 2    | undo changes                                                                                                                                        |
| `v`             | `v`                  |      | start characterwise Visual mode                                                                                                                     |
| `w`             | `w`                  | 1    | cursor N words forward                                                                                                                              |
| `x`             | `["x]x`              | 2    | delete N characters under and after the cursor [into buffer x]                                                                                      |
| `y`             | `["x]y{motion}`      |      | yank Nmove text [into buffer x]                                                                                                                     |
| `yy`            | `["x]yy`             |      | yank N lines [into buffer x]                                                                                                                        |
| `z`             | `z{char}`            |      | commands starting with 'z', see below                                                                                                               |
| `{`             | `{`                  | 1    | cursor N paragraphs backward                                                                                                                        |
| `bar`           | `                    | `    | 1                                                                                                                                                   | cursor to column N |
| `}`             | `}`                  | 1    | cursor N paragraphs forward                                                                                                                         |
| `~`             | `~`                  | 2    | switch case of N characters under cursor and move the cursor characters to the right                                                                |
| `<C-End>`       | `<C-End>`            | 1    | same as "G"                                                                                                                                         |
| `<C-Home>`      | `<C-Home>`           | 1    | same as "gg"                                                                                                                                        |
| `<C-Left>`      | `<C-Left>`           | 1    | same as "b"                                                                                                                                         |
| `<C-Right>`     | `<C-Right>`          | 1    | same as "w"                                                                                                                                         |
| `<Del>`         | `["x]<Del>`          | 2    | same as "x"                                                                                                                                         |
| `N<Del>`        | `{count}<Del>`       |      | remove the last digit from {count}                                                                                                                  |
| `<Down>`        | `<Down>`             | 1    | same as "j"                                                                                                                                         |
| `<End>`         | `<End>`              | 1    | same as "$"                                                                                                                                         |
| `<F1>`          | `<F1>`               |      | same as <Help>                                                                                                                                      |
| `<Help>`        | `<Help>`             |      | open a help window                                                                                                                                  |
| `<Home>`        | `<Home>`             | 1    | same as "0"                                                                                                                                         |
| `<Insert>`      | `<Insert>`           | 2    | same as "i"                                                                                                                                         |
| `<Left>`        | `<Left>`             | 1    | same as "h"                                                                                                                                         |
| `<LeftMouse>`   | `<LeftMouse>`        | 1    | move cursor to the mouse click position                                                                                                             |
| `<PageDown>`    | `<PageDown>`         |      | same as CTRL-F                                                                                                                                      |
| `<PageUp>`      | `<PageUp>`           |      | same as CTRL-B                                                                                                                                      |
| `<Right>`       | `<Right>`            | 1    | same as "l"                                                                                                                                         |
| `<S-Down>`      | `<S-Down>`           | 1    | same as CTRL-F                                                                                                                                      |
| `<S-Left>`      | `<S-Left>`           | 1    | same as "b"                                                                                                                                         |
| `<S-Right>`     | `<S-Right>`          | 1    | same as "w"                                                                                                                                         |
| `<S-Up>`        | `<S-Up>`             | 1    | same as CTRL-B                                                                                                                                      |
| `<Undo>`        | `<Undo>`             | 2    | same as "u"                                                                                                                                         |
| `<Up>`          | `<Up>`               | 1    | same as "k"                                                                                                                                         |

### 2.1 Text objects                                                *objects*

These can be used after an operator or in Visual mode to select an object.

| tag    | command | action in Normal mode                       |
| ------ | ------- | ------------------------------------------- |
| `v_a(` | `a(`    | same as ab                                  |
| `v_a)` | `a)`    | same as ab                                  |
| `v_a<` | `a<`    | "a <>" from '<' to the matching '>'         |
| `v_a>` | `a>`    | same as a<                                  |
| `v_aB` | `aB`    | "a Block" from "[{" to "]}" (with brackets) |
| `v_aW` | `aW`    | "a WORD" (with white space)                 |
| `v_a[` | `a[`    | "a []" from '[' to the matching ']'         |
| `v_a]` | `a]`    | same as a[                                  |
| `v_ab` | `ab`    | "a block" from "[(" to "])" (with braces)   |
| `v_ap` | `ap`    | "a paragraph" (with white space)            |
| `v_as` | `as`    | "a sentence" (with white space)             |
| `v_aw` | `aw`    | "a word" (with white space)                 |
| `v_a{` | `a{`    | same as aB                                  |
| `v_a}` | `a}`    | same as aB                                  |
| `v_i(` | `i(`    | same as ib                                  |
| `v_i)` | `i)`    | same as ib                                  |
| `v_i<` | `i<`    | "inner <>" from '<' to the matching '>'     |
| `v_i>` | `i>`    | same as i<                                  |
| `v_iB` | `iB`    | "inner Block" from "[{" and "]}"            |
| `v_iW` | `iW`    | "inner WORD"                                |
| `v_i[` | `i[`    | "inner []" from '[' to the matching ']'     |
| `v_i]` | `i]`    | same as i[                                  |
| `v_ib` | `ib`    | "inner block" from "[(" to "])"             |
| `v_ip` | `ip`    | "inner paragraph"                           |
| `v_is` | `is`    | "inner sentence"                            |
| `v_iw` | `iw`    | "inner word"                                |
| `v_i{` | `i{`    | same as iB                                  |
| `v_i}` | `i}`    | same as iB                                  |
`
2.2 Window commands                                             *CTRL-W*

tag             command            action in Normal mode

2.3 Square bracket commands                                     *[* *]*

| tag  | char | note | action in Normal mode                            |
| ---- | ---- | ---- | ------------------------------------------------ |
| `[(` | `[(` | 1    | cursor N times back to unmatched '('             |
| `[P` | `[P` | 2    | same as "[p"                                     |
| `[[` | `[[` | 1    | cursor N sections backward                       |
| `[]` | `[]` | 1    | cursor N SECTIONS backward                       |
| `[b` | `[b` | 1    | cursor N camel words backward                    |
| `[p` | `[p` | 2    | like "P", but adjust indent to current line      |
| `[m` | `[m` | 1    | cursor N times back to start of member function  |
| `[w` | `[w` | 1    | cursor N camel words forward                     |
| `[{` | `[{` | 1    | cursor N times back to unmatched '{'             |
| `])` | `])` | 1    | cursor N times forward to unmatched ')'          |
| `]P` | `]P` | 2    | same as "[p"                                     |
| `][` | `][` | 1    | cursor N SECTIONS forward                        |
| `]]` | `]]` | 1    | cursor N sections forward                        |
| `]b` | `]b` | 1    | cursor backward to the end of camel word N       |
| `]p` | `]p` | 2    | like "p", but adjust indent to current line      |
| `]m` | `]m` | 1    | cursor N times forward to end of member function |
| `]w` | `]w` | 1    | cursor forward to the end of camel word N        |
| `]}` | `]}` | 1    | cursor N times forward to unmatched '}'          |

2.4 Commands starting with 'g'                                          *g*

| tag        | char           | note | action in Normal mode                                                                                                                                                          |
| ---------- | -------------- | ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `g_CTRL-G` | `g_CTRL-G`     |      | show information about current cursor position                                                                                                                                 |
| `g#`       | `g#`           | 1    | like "#", but without using "\<" and "\>"                                                                                                                                      |
| `g$`       | `g$`           | 1    | when 'wrap' off go to rightmost character of the current line that is on the screen; when 'wrap' on go to the rightmost character of the current screen line                   |
| `g&`       | `g&`           | 2    | repeat last ":s" on all lines                                                                                                                                                  |
| `g'`       | `g'{mark}`     | 1    | like                                                                                                                                                                           | '  | but without changing the jumplist |
| `` g` ``   | `` g`{mark} `` | 1    | like                                                                                                                                                                           | `  | but without changing the jumplist |
| `g(`       | `g(`           | 1    | cursor N sentence ends backward                                                                                                                                                |
| `g)`       | `g)`           | 1    | cursor N sentence ends forward                                                                                                                                                 |
| `gstar`    | `g*`           | 1    | like "*", but without using "\<" and "\>"                                                                                                                                      |
| `g0`       | `g0`           | 1    | when 'wrap' off go to leftmost character of the current line that is on the screen; when 'wrap' on go to the leftmost character of the current screen line                     |
| `g8`       | `g8`           |      | print hex value of bytes used in UTF-8 character under the cursor                                                                                                              |
| `gD`       | `gD`           | 1    | go to definition of word under the cursor in current file                                                                                                                      |
| `gE`       | `gE`           | 1    | go backwards to the end of the previous WORD                                                                                                                                   |
| `gI`       | `gI`           | 2    | like "I", but always start in column 1                                                                                                                                         |
| `gJ`       | `gJ`           | 2    | join lines without inserting space                                                                                                                                             |
| `gP`       | `["x]gP`       | 2    | put the text [from register x] before the cursor N times, leave the cursor after it                                                                                            |
| `gU`       | `gU{motion}`   | 2    | make Nmove text uppercase                                                                                                                                                      |
| `g^`       | `g^`           | 1    | when 'wrap' off go to leftmost non-white character of the current line that is on the screen; when 'wrap' on go to the leftmost non-white character of the current screen line |
| `ga`       | `ga`           |      | print ascii value of character under the cursor                                                                                                                                |
| `gd`       | `gd`           | 1    | go to definition of word under the cursor in current function                                                                                                                  |
| `ge`       | `ge`           | 1    | go backwards to the end of the previous word                                                                                                                                   |
| `gg`       | `gg`           | 1    | cursor to line N, default first line                                                                                                                                           |
| `gi`       | `gi`           | 2    | like "i", but first move to the                                                                                                                                                | '^ | mark                              |
| `gj`       | `gj`           | 1    | like "j", but when 'wrap' on go N screen lines down                                                                                                                            |
| `gk`       | `gk`           | 1    | like "k", but when 'wrap' on go N screen lines up                                                                                                                              |
| `gm`       | `gm`           | 1    | go to character at middle of the screenline                                                                                                                                    |
| `go`       | `go`           | 1    | cursor to byte N in the buffer                                                                                                                                                 |
| `gp`       | `["x]gp`       | 2    | put the text [from register x] after the cursor N times, leave the cursor after it                                                                                             |
| `gu`       | `gu{motion}`   | 2    | make Nmove text lowercase                                                                                                                                                      |
| `gv`       | `gv`           |      | reselect the previous Visual area                                                                                                                                              |
| `g~`       | `g~{motion}`   | 2    | swap case for Nmove text                                                                                                                                                       |
| `g<Down>`  | `g<Down>`      | 1    | same as "gj"                                                                                                                                                                   |
| `g<End>`   | `g<End>`       | 1    | same as "g$"                                                                                                                                                                   |
| `g<Home>`  | `g<Home>`      | 1    | same as "g0"                                                                                                                                                                   |
| `g<Up>`    | `g<Up>`        | 1    | same as "gk"                                                                                                                                                                   |

2.5 Commands starting with 'z'                                          *z*

| tag        | char       | note                                                                                              | action in Normal mode |
| ---------- | ---------- | ------------------------------------------------------------------------------------------------- | --------------------- |
| `z<CR>`    | `z<CR>`    | redraw, cursor line to top of window, cursor on first non-blank                                   |
| `z+`       | `z+`       | cursor on line N (default line below window), otherwise like "z<CR>"                              |
| `z-`       | `z-`       | redraw, cursor line at bottom of window, cursor on first non-blank                                |
| `z.`       | `z.`       | redraw, cursor line to center of window, cursor on first non-blank                                |
| `zM`       | `zM`       | set 'foldlevel' to zero                                                                           |
| `zR`       | `zR`       | set 'foldlevel' to the deepest fold                                                               |
| `z^`       | `z^`       | cursor on line N (default line above window), otherwise like "z-"                                 |
| `zb`       | `zb`       | redraw, cursor line at bottom of window                                                           |
| `zc`       | `zc`       | close a fold                                                                                      |
| `ze`       | `ze`       | when 'wrap' off scroll horizontally to position the cursor at the end (right side) of the screen  |
| `zh`       | `zh`       | when 'wrap' off scroll screen N characters to the right                                           |
| `zl`       | `zl`       | when 'wrap' off scroll screen N characters to the left                                            |
| `zo`       | `zo`       | open fold                                                                                         |
| `zs`       | `zs`       | when 'wrap' off scroll horizontally to position the cursor at the start (left side) of the screen |
| `zt`       | `zt`       | redraw, cursor line at top of window                                                              |
| `zz`       | `zz`       | redraw, cursor line at center of window                                                           |
| `z<Left>`  | `z<Left>`  | same as "zh"                                                                                      |
| `z<Right>` | `z<Right>` | same as "zl"                                                                                      |

## 3. Visual mode                                          *visual-index*

Most commands in Visual mode are the same as in Normal mode. The ones listed
here are those that are different.

| tag               | command         | note | action in Visual mode                                                                      |
| ----------------- | --------------- | ---- | ------------------------------------------------------------------------------------------ |
| `v_CTRL-\_CTRL-N` | `CTRL-\ CTRL-N` |      | stop Visual mode                                                                           |
| `v_CTRL-Q`        | `CTRL-Q`        |      | same a CTRL-V                                                                              |
| `v_CTRL-V`        | `CTRL-V`        |      | make Visual mode blockwise or stop Visual mode                                             |
| `v_!`             | `!{filter}`     | 2    | filter the highlighted lines through the external command {filter}                         |
| `v_:`             | `:`             |      | start a command-line with the highlighted lines as a range                                 |
| `v_<`             | `<`             | 2    | shift the highlighted lines one 'shiftwidth' left                                          |
| `v_=`             | `=`             | 2    | filter the highlighted lines through the external program given with the 'equalprg' option |
| `v_>`             | `>`             | 2    | shift the highlighted lines one 'shiftwidth' right                                         |
| `v_b_A`           | `A`             | 2    | block mode: append same text in all lines, after the highlighted area                      |
| `v_C`             | `C`             | 2    | delete the highlighted lines and start insert                                              |
| `v_D`             | `D`             | 2    | delete the highlighted lines                                                               |
| `v_b_I`           | `I`             | 2    | block mode: insert same text in all lines, before the highlighted area                     |
| `v_J`             | `J`             | 2    | join the highlighted lines                                                                 |
| `v_O`             | `O`             |      | Move horizontally to other corner of area.  Q                  does not start Ex mode      |
| `v_R`             | `R`             | 2    | delete the highlighted lines and start insert                                              |
| `v_S`             | `S`             | 2    | delete the highlighted lines and start insert                                              |
| `v_U`             | `U`             | 2    | make highlighted area uppercase                                                            |
| `v_V`             | `V`             |      | make Visual mode linewise or stop Visual mode                                              |
| `v_X`             | `X`             | 2    | delete the highlighted lines                                                               |
| `v_Y`             | `Y`             |      | yank the highlighted lines                                                                 |
| `v_a(`            | `a(`            |      | same as ab                                                                                 |
| `v_a)`            | `a)`            |      | same as ab                                                                                 |
| `v_a<`            | `a<`            |      | extend highlighted area with a <> block                                                    |
| `v_a>`            | `a>`            |      | same as a<                                                                                 |
| `v_aB`            | `aB`            |      | extend highlighted area with a {} block                                                    |
| `v_aW`            | `aW`            |      | extend highlighted area with "a WORD"                                                      |
| `v_a[`            | `a[`            |      | extend highlighted area with a [] block                                                    |
| `v_a]`            | `a]`            |      | same as a[                                                                                 |
| `v_ab`            | `ab`            |      | extend highlighted area with a () block                                                    |
| `v_ap`            | `ap`            |      | extend highlighted area with a paragraph                                                   |
| `v_as`            | `as`            |      | extend highlighted area with a sentence                                                    |
| `v_aw`            | `aw`            |      | extend highlighted area with "a word"                                                      |
| `v_a{`            | `a{`            |      | same as aB                                                                                 |
| `v_a}`            | `a}`            |      | same as aB                                                                                 |
| `v_c`             | `c`             | 2    | delete highlighted area and start insert                                                   |
| `v_d`             | `d`             | 2    | delete highlighted area                                                                    |
| `v_gJ`            | `gJ`            | 2    | join the highlighted lines without inserting spaces                                        |
| `v_gq`            | `gq`            | 2    | format the highlighted lines                                                               |
| `v_gv`            | `gv`            |      | exchange current and previous highlighted area                                             |
| `v_i(`            | `i(`            |      | same as ib                                                                                 |
| `v_i)`            | `i)`            |      | same as ib                                                                                 |
| `v_i<`            | `i<`            |      | extend highlighted area with inner <> block                                                |
| `v_i>`            | `i>`            |      | same as i<                                                                                 |
| `v_iB`            | `iB`            |      | extend highlighted area with inner {} block                                                |
| `v_iW`            | `iW`            |      | extend highlighted area with "inner WORD"                                                  |
| `v_i[`            | `i[`            |      | extend highlighted area with inner [] block                                                |
| `v_i]`            | `i]`            |      | same as i[                                                                                 |
| `v_ib`            | `ib`            |      | extend highlighted area with inner () block                                                |
| `v_ip`            | `ip`            |      | extend highlighted area with inner paragraph                                               |
| `v_is`            | `is`            |      | extend highlighted area with inner sentence                                                |
| `v_iw`            | `iw`            |      | extend highlighted area with "inner word"                                                  |
| `v_i{`            | `i{`            |      | same as iB                                                                                 |
| `v_i}`            | `i}`            |      | same as iB                                                                                 |
| `v_o`             | `o`             |      | move cursor to other corner of area                                                        |
| `v_r`             | `r`             | 2    | delete highlighted area and start insert                                                   |
| `v_s`             | `s`             | 2    | delete highlighted area and start insert                                                   |
| `v_u`             | `u`             | 2    | make highlighted area lowercase                                                            |
| `v_v`             | `v`             |      | make Visual mode characterwise or stop Visual mode                                         |
| `v_x`             | `x`             | 2    | delete the highlighted area                                                                |
| `v_y`             | `y`             |      | yank the highlighted area                                                                  |
| `v_~`             | `~`             | 2    | swap case for the highlighted area                                                         |

## 4. Command-line editing                                 *ex-edit-index*

Get to the command-line with the ':', '!', '/' or '?' commands.
Normal characters are inserted at the current cursor position.

| tag             | command            | action                                                                                |
| --------------- | ------------------ | ------------------------------------------------------------------------------------- |
|                 | `CTRL-@`           | not used                                                                              |
| `c_CTRL-B`      | `CTRL-B`           | cursor to begin of command-line                                                       |
| `c_CTRL-C`      | `CTRL-C`           | same as <ESC>                                                                         |
| `c_CTRL-E`      | `CTRL-E`           | cursor to end of command-line                                                         |
|                 | `CTRL-G`           | not used                                                                              |
| `c_<BS>`        | `<BS>`             | delete the character in front of the cursor                                           |
| `c_CTRL-H`      | `CTRL-H`           | same as <BS>                                                                          |
| `c_<NL>`        | `<NL>`             | same as <CR>                                                                          |
| `c_CTRL-J`      | `CTRL-J`           | same as <CR>                                                                          |
| `c_CTRL-K`      | `CTRL-K {char1} {` | char2} enter digraph                                                                  |
| `c_<CR>`        | `<CR>`             | execute entered command                                                               |
| `c_<CR>`        | `CTRL-M`           | same as <CR>                                                                          |
| `c_CTRL-Q`      | `CTRL-Q`           | same as CTRL-V, unless it's used for terminal control flow                            |
| `c_CTRL-U`      | `CTRL-U`           | remove all characters                                                                 |
| `c_CTRL-V`      | `CTRL-V`           | insert next non-digit literally, insert three digit decimal number as a single byte.  |
| `c_CTRL-W`      | `CTRL-W`           | delete the word in front of the cursor                                                |
|                 | `CTRL-X`           | not used (reserved for completion)                                                    |
|                 | `CTRL-Z`           | not used (reserved for suspend)                                                       |
| `c_<Esc>`       | `<Esc>`            | abandon command-line without executing it                                             |
| `c_<Esc>`       | `CTRL-[`           | same as <Esc>                                                                         |
|                 | `CTRL-\ a - z`     | reserved for extensions                                                               |
|                 | `CTRL-\ others`    | not used                                                                              |
|                 | `CTRL-]`           | not used                                                                              |
| `c_<Del>`       | `<Del>`            | delete the character under the cursor                                                 |
| `c_<Left>`      | `<Left>`           | cursor left                                                                           |
| `c_<S-Left>`    | `<S-Left>`         | cursor one word left                                                                  |
| `c_<C-Left>`    | `<C-Left>`         | cursor one word left                                                                  |
| `c_<Right>`     | `<Right>`          | cursor right                                                                          |
| `c_<S-Right>`   | `<S-Right>`        | cursor one word right                                                                 |
| `c_<C-Right>`   | `<C-Right>`        | cursor one word right                                                                 |
| `c_<Up>`        | `<Up>`             | recall previous command-line from history that matches pattern in front of the cursor |
| `c_<S-Up>`      | `<S-Up>`           | recall previous command-line from history                                             |
| `c_<Down>`      | `<Down>`           | recall next command-line from history that matches pattern in front of the cursor     |
| `c_<S-Down>`    | `<S-Down>`         | recall next command-line from history                                                 |
| `c_<Home>`      | `<Home>`           | cursor to start of command-line                                                       |
| `c_<End>`       | `<End>`            | cursor to end of command-line                                                         |
| `c_<PageDown>`  | `<PageDown>`       | same as <S-Down>                                                                      |
| `c_<PageUp>`    | `<PageUp>`         | same as <S-Up>                                                                        |
| `c_<Insert>`    | `<Insert>`         | toggle insert/overstrike mode                                                         |
| `c_<LeftMouse>` | `<LeftMouse>`      | cursor at mouse click                                                                 |

## 5. EX commands                                  *ex-cmd-index* *:index*

This is a brief but complete listing of all the ":" commands, without
mentioning any arguments.  The optional part of the command name is inside [].
The commands are sorted on the non-optional part of their name.

| command       | short           | action                                                   |
| ------------- | --------------- | -------------------------------------------------------- |
| `:!`          | `:!`            | filter lines or execute an external command              |
| `:!!`         | `:!!`           | repeat last ":!" command                                 |
| `:&`          | `:&`            | repeat last ":substitute"                                |
| `:<`          | `:<`            | shift lines one 'shiftwidth' left                        |
| `:>`          | `:>`            | shift lines one 'shiftwidth' right                       |
| `:@`          | `:@`            | execute contents of a register                           |
| `:@@`         | `:@@`           | repeat the previous ":@"                                 |
| `:Next`       | `:N[ext]`       | go to previous file in the argument list                 |
| `:argument`   | `:argu[ment]`   | go to specific file in the argument list                 |
| `:ascii`      | `:as[cii]`      | print ascii value of character under the cursor          |
| `:browse`     | `:bro[wse]`     | use file selection dialog                                |
| `:class`      | `:cla[ss]`      | find class in project and edit it (not in Vim)           |
| `:close`      | `:clo[se]`      | close current window                                     |
| `:copy`       | `:co[py]`       | copy lines                                               |
| `:delete`     | `:d[elete]`     | delete lines                                             |
| `:display`    | `:di[splay]`    | display registers                                        |
| `:digraphs`   | `:dig[raphs]`   | show or enter digraphs                                   |
| `:edit`       | `:e[dit]`       | edit a file                                              |
| `:exit`       | `:exi[t]`       | same as ":xit"                                           |
| `:find`       | `:fin[d]`       | find file in 'path' and edit it                          |
| `:first`      | `:fir[st]`      | go to the first file in the argument list                |
| `:goto`       | `:go[to]`       | go to byte in the buffer                                 |
| `:help`       | `:h[elp]`       | open a help window                                       |
| `:hide`       | `:hid[e]`       | close current editor                                     |
| `:history`    | `:his[tory]`    | print a history list                                     |
| `:join`       | `:j[oin]`       | join lines                                               |
| `:jumps`      | `:ju[mps]`      | print the jump list                                      |
| `:k`          | `:k`            | set a mark                                               |
| `:last`       | `:la[st]`       | go to the last file in the argument list                 |
| `:move`       | `:m[ove]`       | move lines                                               |
| `:mark`       | `:ma[rk]`       | set a mark                                               |
| `:marks`      | `:marks`        | list all marks                                           |
| `:next`       | `:n[ext]`       | go to next file in the argument list                     |
| `:nohlsearch` | `:noh[lsearch]` | suspend 'hlsearch' highlighting                          |
| `:only`       | `:on[ly]`       | close all windows except current one                     |
| `:previous`   | `:prev[ious]`   | go to previous file in argument list                     |
| `:promptfind` | `:pro[mptfind]` | Search dialog                                            |
| `:promptrepl` | `:promptr[epl]` | Search/Replace dialog                                    |
| `:put`        | `:pu[t]`        | insert contents of register in the text                  |
| `:quit`       | `:q[uit]`       | quit current window (when one window quit Vim)           |
| `:quitall`    | `:quita[ll]`    | quit Vim                                                 |
| `:qall`       | `:qa[ll]`       | quit Vim                                                 |
| `:redo`       | `:red[o]`       | redo one undone change                                   |
| `:registers`  | `:reg[isters]`  | display the contents of registers                        |
| `:rewind`     | `:rew[ind]`     | go to the first file in the argument list                |
| `:substitute` | `:s[ubstitute]` | find and replace text                                    |
| `:set`        | `:se[t]`        | show or set options                                      |
| `:t`          | `:t`            | same as ":copy"                                          |
| `:undo`       | `:u[ndo]`       | undo last change(s)                                      |
| `:write`      | `:w[rite]`      | write to a file                                          |
| `:wNext`      | `:wN[ext]`      | write to a file and go to previous file in argument list |
| `:wall`       | `:wa[ll]`       | write all (changed) buffers                              |
| `:wnext`      | `:wn[ext]`      | write to a file and go to next file in argument list     |
| `:wprevious`  | `:wp[revious]`  | write to a file and go to previous file in argument list |
| `:wq`         | `:wq`           | write to a file and quit window or Vim                   |
| `:wqall`      | `:wqa[ll]`      | write all changed buffers and quit Vim                   |
| `:xit`        | `:x[it]`        | write if buffer changed and quit window or Vim           |
| `:xall`       | `:xa[ll]`       | same as ":wqall"                                         |
| `:yank`       | `:y[ank]`       | yank lines into a register                               |
| `:~`          | `:~`            | repeat last ":substitute"                                |
