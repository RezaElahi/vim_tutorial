# vim_tutorial
Brief History: __ed__ is a line editor developed by the legendary Kemp Thomson in 1970. Later, Bill Joy developed the __vi__ (visual) editor, which was not free in the beginning. Bram Moolenaar wrote __vim__ (Vi IMproved) in 1991.<br>
Usually 10% of your time you are typing something, so the default mode of the vi is command mode.<br>
There are many jokes about the people who open the vi and don't know how to quit it, so they restart the computer :)
## Command Description
	:q!	--> quit without saving
	:wq	--> write and quit
	ESC	--> quit any mode
	i	--> insert mode
	a	--> append mode
	x,X	--> delete character
	o,O	--> open a new line
	J	--> Join two lines
	G	--> Go to line (G, 1G, 10G)
	y	--> yank/copy (yy, yw, 2yy, ..)
	p,P	--> paste below or above
	r	--> replace a character
	u	--> undo
	d	--> delete + commmand (dd, dw, 3dw, 2dd), these are actually yanked!
	/word	--> search for the word (n,N find the next match)
	$	--> end of line (from regex)
	^	--> start of the line (from rejex)
	. 	--> repeat the last command
<br>
VI can mix the previous command! For example:
	3x	--> delete three characters!
	2u	--> two times undo
	d$	--> delete till end of line
