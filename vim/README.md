[index]: https://github.com/rafaelrinaldi/cheatsheets
[abolish]: https://github.com/tpope/vim-abolish
[surround]: https://github.com/tpope/vim-surround
[unimpaired]: https://github.com/tpope/vim-unimpaired
[vimfiles]: https://github.com/rafaelrinaldi/vimfiles

# Vim

<img src=vim.png width=150>

1. [Defauts](#1.0)
2. [Plugins](#2.0)
  * [abolish.vim](#2.1)
  * [surround.vim](#2.2)
  * [unimpaired.vim](#2.3)

<small>My personal Vim configuration can be found [here][vimfiles].</small>

---

### <a name='1.0'></a>Defaults

| Command | Description |
| :--- | :--- |
| `gf` | Open file under cursor |
| `Ctrl+w gf` | Open file under cursor in a new tab |
| `:ccl` | Close quickfix window |
| `f[pattern]` | Jump to pattern |
| `xp` | Swap letters |
| `Ctrl+a` | Increase number under cursor |
| `Ctrl+x` | Decrease number under cursor |
| `:e!` | Read updated file content from disk to active buffer |
| `Ctrl+n` | Toggle omni completion |
| `Ctrl+r=[equation]` | Evaluate a math equation (insert mode only) |
| `:wa` | Save all buffers |
| `:xa` | Save all buffers and exit |
| `:r file.txt` | Print the contents of `file.txt` into the current buffer |
| `:r !ls` | Print the list of all files of current directory into the current buffer |
| `:% s/word//gn` | Count the number of occurrences of `word` |
| `:noh` | Remove highlighted search results |
| `:ls` | List active buffers |
| `:buf n` | Open buffer `n` into the current panel |
| `:only` | Close all panels but the current one |
| `z1=` | Fix word typos automatically |
| `dd2kp` | Send current line ↑ |
| `ddp` | Send current line one ↓ |
| `~` | Toggle character casing under the cursor |
| `guu` | Convert the whole line to lower case |
| `gUU` | Convert the whole line to upper case |
| `O` | Add new line above the cursor in insert mode |
| `o` | Add new line below the cursor in insert mode |
| `d$` or `D` | Delete from cursor until the end of line |
| `cc` | Change the contents of current line |
| `mq` | Create a marker named `q` |
| `` `q  `` | Move cursor to `q` marker position |
| `qq` | Start recording a macro named `q` |
| `q` | Stop recording macro |
| `@q` | Play macro `q` |
| `'.'` | Jump to last modified line |
| `` `. `` | Jump to exact position of last modification |
| `Ctrl+o` | Open previous file at previous cursor position |
| `Ctrl+i` | Open next file at previous cursor position |
| `I` | Start input mode at the beginning of line |
| `A` | Start input mode at the end of line |
| `L` | Move cursor to last visible line |
| `:nt.` | Copy the contents of line `n` to current line |
| `zf` | Create a fold |
| `za` | Unfold current fold |
| `gg` | Move cursor to the top of file |
| `G` | Move cursor to the bottom of file |
| `H` | Move cursor to the top of view port |
| `M` | Move cursor to the middle of view port |
| `L` | Move cursor to the bottom of view port |

## <a name='2.0'></a>Plugins

### <a name='2.1'></a>[abolish.vim][abolish]

| Command | Description |
| :--- | :--- |
| `crs` | Convert string to snake_case |
| `crm` | Convert string to MixedCase (aka PascalCase) |
| `crc` | Convert string to camelCase |
| `cru` | Convert string to UPPER_CASE |
| `:%Subvert/p{re,ost}processor{,s}//g` | Improved regex support for search and replace |

### <a name='2.2'></a>[surround.vim][surround]

| Command | Description |
| :--- | :--- |
| `cs"''` | Change double quotes to single quotes |
| `ysiw}` | Surround word under cursor with brackets |
| `ysiw<small>` | Surround word under cursor with `<small>` tag |
| `S<div class="wrapper">` | Wrap content of current selection with a `<div>` tag |
| `yss)` | Surround the whole line with parentheses |
| `ds]` | Remove square brackets from word under cursor |

### <a name='2.3'></a>[unimpaired.vim][unimpaired]

| Command | Description |
| :--- | :--- |
| `[b` | Next file on buffer list |
| `]b` | Previous file on buffer list |
| `[x` | Encode XML/HTML selection |
| `]x` | Decode XML/HTML selection |
| `[u` | Encode URL selection |
| `]u` | Decode URL selection |
| `[<Space>` | Add a new line above the cursor |
| `]<Space>` | Add a new line below the cursor |
| `[os` | Enable spelling |
| `]os` | Disable spelling |
| `[f` | Next file in the directory |
| `]f` | Previous file in the directory |
| `[n` | Next Git diff conflict marker |
| `]n` | Previous Git diff conflict marker |
| `[y` | Escape string (C String style) |
| `]y` | Unescape string (C String style) |

---

[← Back][index]
