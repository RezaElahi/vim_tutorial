# vim_tutorial
Brief History: __ed__ is a line editor developed by the legendary Kemp Thomson in 1970. Later, Bill Joy developed the __vi__ (visual) editor, which was not free in the beginning. Bram Moolenaar wrote __vim__ (Vi IMproved) in 1991.<br>
Usually 10% of your time you are typing something, so the default mode of the vi is command mode.<br>
There are many jokes about the people who open the vi and don't know how to quit it, so they restart the computer :)
# First Part
These are what I have lernead from Jadi Tutorial for vim. 
## Command Description
	:q!	--> quit without saving
	:wq	--> write and quit
	ESC	--> quit any mode
	i	--> insert mode
	a,A	--> append mode
	x,X	--> delete character
	o,O	--> open a new line
	J	--> Join two lines
	G	--> Go to line (G, 1G, 10G)
	y	--> yank/copy (yy, yw, 2yy, ..)
	p,P	--> put/paste below or above
	r,R	--> replace a character or more, replace mode is like insert mode but every typed character will delete and existing one
	u,U	--> undo, return the whole line to original state!
	d	--> delete + motion (dd, dw, 3dw, 2dd), these are actually yanked!
	ce	--> change operator, delete the word and place you in insert mode
	/word	--> search for the word (n,N find the next match)
	?X	--> search backward for X (n,N finds the next match)
	$	--> end of line (from regex)
	^,0	--> start of the line (from rejex)
	. 	--> repeat the last command

<br>
VI can combine the previous commands! For example:

	3x	--> delete three characters!
	2u	--> two times undo
	d$	--> delete till end of line
	de	--> delete till end of the word
	dw	--> delete till begininng of next word.
	c	--> change operator work the same as d operator: c [number], it allows you to change from the cursor to where the motion takes you
	:![COMMAND]	--> Execute external command
	:!ls	--> smae as ls, print Enter to return
	:w TEST	--> write saved changes to TEXT
	ce	--> change operator, delete the word and place you in insert mode
	/:!rm TEST	--> remove TEST
	v	--> visual selector (:w TEST, yank, d, ...)
	v motion :w FILENAME	--> Write the selection to the file
	:r TEST	--> Retrieve (read) the content of TEST and paste it belo the cursor!	
	~/.vimrc	--> the startup scrip for doing configuration and setting!


<br>Here are some sample text to edit and work with. I need to add a break in the begining of this line so  how to do that?
# Second Part
This part is from vimtutor. It is build in guide for learning vim commands.

	%	--> search for matching ( { [, press it agian switch between those
	:s/old/new	--> substitude the first match in the line
	:s/old/new/g	--> substitude all  matches in the line
	:#,#s/old/new/gc	--> substitude all  matches between two lines with a prompt for each
	crtl+r	--> undo the undo's!
	ctrl+g	--> show the status of your location in the file
	gg	--> begininng of file
	10G	--> same as 10gg
	ctrl+I/O	--> to go back/forward where you came from. Useful for after search command!
	yw	--> You can also use yank as a operator, yw will yank a word
	set ic	--> set ignore case as TRUE, then you can serach for what you like
	set noic	--> prepend no to switch an option off
	:help w	--> shows the help fpr w command
	
			
