# Emacs, Vi (Vim) and Git concepts
> Repository created to review concepts related with Emacs, Vi and Git <br>
Holberton Dev Bootcamp - Montevideo 2023
## Emacs
### Resources
- [x] [A Guided Tour of Emacs](https://www.gnu.org/software/emacs/tour/)
### Learning Objectives
* What is Emacs
	- Emacs is an extensible, customizable, self-documenting real-time display editor
* Who is Richard Stallman
	- Richard Matthew Stallman, also known by his initials, rms, is an American free software movement activist and programmer. He campaigns for software to be distributed in such a manner that its users have the freedom to use, study, distribute, and modify that software.
* How to open and save files
	- Use Ctrl-x f to open a file from within Emacs. Ctrl-x Ctrl-s to save the file.
* What is a buffer and how to switch from one to the other
	- For conveniently switching between a few buffers, use the commands C-x LEFT and C-x RIGHT
* How to use the mark and the point to set the region
	- To set the mark, type C- SPC ( set-mark-command ). This makes the mark active
* How to cut and paste lines and regions
	- To cut the text, press C-w.
	- To copy the text, press M-w.
	- To paste the text, press C-y.
* How to search forward and backward
	- C-s for forward search, and C-r for reverse search.
* How to invoke commands by name
	- Type M-x , then the name of the command, and finally hit RETURN (notice that all this happens in the echo area)
* How to undo
	- C-x u or C-_
* How to cancel half-entered commands
	- quitting with C-g , and aborting with C-] or M-x top-level
* How to quit Emacs
	- C-z and Emacs will be suspended. To get back into Emacs, type %emacs at the shell prompt. To quit Emacs permanently, type C-x C-c.
### Quiz answers
* Question #0
	- In Emacs’ documentation, what does C in a shortcut command stand for?
		- Ctrl
	- In Emacs’ documentation, what does M in a shortcut command stand for?
		- Alt
		- Meta
	- In Emacs, a buffer is an object that a file’s text is held in.
		- True
	- You can only have one buffer open in Emacs at a time.
		- False
## Vi
## Git
