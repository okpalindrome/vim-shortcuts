# vim-shortcuts
Personal note/reference

```
**Mode**
command/normal mode - ESC
visual mode - ESC + v
insert mode - i

**remove ^I for spaces and $ signs at the end of each line**
:set nolist

**or add to ~/.vimrc**
set nolist
set number - to show line numbers
:<line-number> - to jump to a specific line


**save changes as a root user**
:w !sudo tee %


**Quick usage**
start of the line - 0
start of the line and switch to insert mode - I
end of the line - $
end of the line and switch to insert mode - A
delete a line - dd
move forward by word start position - w
move forward by word end position - e
move to the first line of file - g
move to the last line the file - G + with append mode A


**cut, copy and paste - system clipboard**
register + or *
cut - visual mode + "+d or "+dd or "+2dd
copy - visual mode + "+y or "+yy or "+2yy
paste - visual mode + "+p - Mostly the system commands like CMD+v or CTRL+v works on insert mode


**cut, copy and paste withing vim**
copy a line - yy
copy 2 or more lines - 2yy
copy till the end of the line - y$

paste after the cursor - p
paste before the cursor - P

cut the line - dd
cut 2 or more lines - 2dd
cut till end of the line - D


**search and vimgrep**
search forward - /keyword
search backward - ?keyword
next found from the search - n
previous found from the search - N
find and replace all - :%s/old/new/g - remove g for one occurance


**tabs and split views**
new tab creation - :tabnew filename
close the current tab - :tabclose
close all other tab except opened one - :tabonly
list all tabs - :tabs
create or open a file in a another file from different directory - :cd /path/to/directory + :tabnew filename

switch to next tab - ESC + gt or :tabnext
switch to previous tab - ESC gT or :tabprevious


**split within a tab. Splitting won't create a new file. Its just for modifying or viewing existing filey**
horizontal split - :sp filename or :split filename
vertical split - :vsp filename or :vsplit filename
switch between splits using CRTL + w (twice)
quit the split just like a file - :q :wq or forcibly
```
