# Vim basics

**Resources:**

- run `vimtutor` in command line
- [Open Vim](https://www.openvim.com/tutorial.html)

## Modes

- `NORMAL` - navigate and manipulate text
- `INSERT` - write text like in other text editors
- `VISUAL` - select text and decide what to do with it

## Keys

### Navigation

- <kbd>h</kbd> <kbd>j</kbd> <kbd>k</kbd> <kbd>l</kbd> - left, down, up, right
- <kbd>w</kbd> - beginning of the next word
- <kbd>b</kbd> - beginning of the word
- <kbd>e</kbd> - end of the word
- <kbd>3</kbd> <kbd>w</kbd> - do a movement _x_ amount of times
- <kbd>f</kbd>, <kbd>F</kbd> + _char_ - find the next or previous occurrence of a character
- <kbd>%</kbd> - jump to the matching parenthesis/bracket
- <kbd>0</kbd>, <kbd>$</kbd>- reach the beginning or end of the line
- <kbd>*</kbd>, <kbd>#</kbd> - find the next or previous occurrence of the word under the cursor
- <kbd>g</kbd><kbd>g</kbd>, <kbd>G</kbd> - jump to the beginning or end of the file
- <kbd>5</kbd><kbd>G</kbd> - go to line 5

### Editing

- <kbd>i</kbd> - enter `INSERT` mode
    - <kbd>7</kbd> <kbd>i</kbd> <kbd>-</kbd> - insert `-` 7 times
- <kbd>a</kbd>, <kbd>A</kbd> - append here or at the end of the line
- <kbd>o</kbd>, <kbd>O</kbd> - insert a new line after or before current line
- <kbd>x</kbd>, <kbd>X</kbd> - delete a character or a character on the left
- <kbd>r</kbd> - replace a character
- <kbd>R</kbd> - replace a bunch of characters
- <kbd>d</kbd> - delete command
    - <kbd>d</kbd><kbd>w</kbd> - delete the next word
        - <kbd>d</kbd><kbd>2</kbd><kbd>e</kbd> - delete two words (to the end of the 2nd one)
    - <kbd>d</kbd><kbd>d</kbd> - delete current line
- <kbd>y</kbd> - copy (yank) into the buffer
    - <kbd>y</kbd> - copy current line
- <kbd>p</kbd> - paste the buffer
- <kbd>u</kbd> - undo
- <kbd>Ctrl</kbd> <kbd>r</kbd> - redo

### General

- <kbd>Esc</kbd> - enter `NORMAL` mode
- `/` - search for text
- <kbd>n</kbd>, <kbd>N</kbd> - search for the next or previous occurrence
- <kbd>.</kbd> - repeat the previous command

## Commands

- `:w` - save
- `:q` - quit
- `:wq` - quit and save
- `:q!` - quit without saving
- `:help` - self explanatory
