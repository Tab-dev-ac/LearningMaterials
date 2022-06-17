# Vim Tutorial

Type `vimtutor` in the terminal to enter this tutorial.

## Movements:

Left `h` Down `j`  Up `k` Right `l`

Move to the start of a line `0`

Move to the end of a line `$`

Move to the end of the file `G`

Move to a line `[number]` + `G`

Move to the first line `gg`

`Ctrl` + `G` show the current location in file

Go back to where you came from `CTRL` + `O`

Go forward after you go back `CTRL` + `I`



## Enter & Quit:

Enter with `vim FILENAME`

Quit with `:q!` to not save changes, `:wq` to save changes.

Enter normal mode `ESC`

## Motion

`w` next start of a word

`e` next end of a word

`$` till the end of a line

## Operator

Delete one Character `x`



Insert text before cursor `i`

Insert text after cursor `a`

Insert text at the end of a line `A`



Undo `u`

Undo all changes in a line `U`

Redo `CTRL` + `R`



Put what's deleted last time `p`



Replace a character `r`+`[a character]`

Replace mode `R`

Change content `c`



`o` start a new line below

`O` start a new line above



visual Mode - select `v`

`y` copy

`p` paste

`V` select a line


## Search

Search forward `/` + `[word]`

Search backward `?` + `[word]`

Ignore cases `:set ic` cancel `:set noic`

Ignore case for one time `\c` (e.g. `/word\c`)

Hightlight search `:set hls` cancel `:set nohls` or `:nohlsearch`, highlight result

Incremental search `:set is` cancel `:set nois` , highlight while typing





`n` next result

`N` next result in another direction

`%` on the bracket to find its match ((,)[,]{,})

## Replace

`:s` substitute

`:#,#s` from line # to line # 

`:%s` within whole file



`/word/newword` old word and the substitution



`/g` globally in line `/c` ask for permission

`/gc`globally in line and ask for persmission



#### Grammar

`:s` + `/word/newword/` + `/g`

<hr/>

`:s/word/newword` substitute the first occurence of the word in a line with the new word

`:s/word/newword/g` substitute all matches with word with newword in the line (globally)

`:s/word/newword/c ` ask before change

(you can use `/gc` as globally and ask for permission)

`:#,#s/word/newworld/g` change from line# to line #

`:%s/word/newword/g` change in the whole file

## Formula

`operator`  `[number]`  `motion`

`2w` forward two words

Delete a word `dw`

Delete till the end of a line `d$`

Change till the end of the word `ce`

Change till the end of a line `c$`

## Other

Delete a whole line `dd`

Display your location in the document `CTRL` + `G`



`:help` get help

`:set nocp` set no compatible mode

`:!ls` or `:!dir` list files in current directory
 
