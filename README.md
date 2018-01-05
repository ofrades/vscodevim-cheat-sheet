# Vim Cheat Sheet
Vim cheat sheet, useful commands compatible with `vscodevim` for Microsoft Visual Studio Code.

## Commands

Vim commands are formed from a combination of verbs and targets.The targets could be objects (words, sentences, paragraphs, lines, the contents of parentheses) or movements (jump to end of word, jump to end of paragraph, jump forward until the letter ‘e’, etc). Forming objects generally involves the use of a modifier. You can also add a count to perform the action count times.

## Verbs

| Command | Use | 
| - | - | 
| i | insert - enter insert mode |
| a | append - enter insert mode after the carat | 
| I | enter insert mode at the beginning of the line | 
| A | append to line (enter insert mode at the end of the line) | 
| o | open a line after the current one and enter insert mode |
| O | open a line before the current one and enter insert mode |
| d[target] | delete (remove from the document and put in buffer) |
| y[target] | yank (copy) |
| p | paste the buffer after the cursor |
| P | paste the buffer before the cursor |
| c[target] | change (delete and then enter insert mode) |
| r[char] | replace the character under the cursor with [char] |
| x | delete the character under the cursor |
| u | undo the last command |
| Ctrl-R | redo the last undo (sidenote: in vim undo/redo forms a tree, changes aren’t lost) |
| / | enter regex search mode |
| n | find the next instance of the search term |
| N | find the previous instance of the search term |
| . | repeat last change (extremely powerful) |

## Nouns/Movements

Nouns or movements are commands for moving within the document or representing an area within a document.

| Command | Use | 
| - | - | 
| h, j, k, l | equivalent to the arrow keys left, down, up, right |
| 0 | move to the very beginning of the current line |
| ^ | move to the first non-whitespace character on the line |
| $ | move to the end of the line |
| w, b | move to the next/previous word |
| W, B | as w/b only Words are bigger |
| ), ( | move to the next/previous sentence |
| }, { | move to the next/previous paragraph |
| /[regexp] | like t but instead of finding a character it finds a regexp |
| % | jump to the matching parenthesis (vim understands nested parenthesis) |
| _ | move to the current line (useful for making commands line-based) |
| *[char] | jump to the next instance of the word under [char] |
| #[char] | jump to the previous instance of the word under [char] |