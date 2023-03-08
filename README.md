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
* Question #1
	- In Emacs’ documentation, what does M in a shortcut command stand for?
		- Alt
		- Meta
* Question #2
	- In Emacs, a buffer is an object that a file’s text is held in.
		- True
* Question #3
	- You can only have one buffer open in Emacs at a time.
		- False
## Vi
### Resources
- [x] [Basic Vi commands](https://www.cs.colostate.edu/helpdocs/vi.html)
### Learning Objectives
* What is vi
	- The default editor that comes with the UNIX operating system is called vi (visual editor).
* Who is Bill Joy
	- William Nelson Joy is an American computer engineer and venture capitalist. He co-founded Sun Microsystems in 1982.
* How to start and exit vi
	- Start: vi <filename>
	- Exit: :x (exit saving changes)
* What are the command and insert modes, and how to switch from one to the other
	- Insert mode: i
	- Command mode: <ESC>
* How to edit text
	- i (insert text before cursor, until <Esc> hit)
	- I (insert text at beginning of current line, until <Esc> hit)
* How to cut and paste lines
	- yy (copy (yank, cut) the current line into the buffer)
	- p (put (paste) the line(s) in the buffer into the text after the current line)
* How to search forward and backward
	- /string (search forward for occurrence of string in text)
	- ?string (search backward for occurrence of string in text)
* How to undo
	- u (UNDO WHATEVER YOU JUST DID; a simple toggle)
* How to quit vi
	- :q<Return> (quit (or exit) vi)
### Quiz answers
* Question #0
	- Vi is included with almost every Linux distribution.
		-True
* Question #1
	- How do you enter Command Mode in Vi?
		- <ESC>
* Question #2
	- How do you enter Insert Mode in Vi?
		- i
* Question #3
	- How do you quit Vi?
		- :q<Return>
## Git
### Resources
- [x] [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [x] [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [x] [How to write a Git commit message](https://cbea.ms/git-commit/)
**For Advanced Tasks**
- [x] [Learning Branching](https://learngitbranching.js.org/?locale=es_ES)
- [x] [Effective pull requests and other good practices for teams using GitHub](https://codeinthehole.com/tips/pull-requests-and-other-good-practices-for-teams-using-github/)
### Learning Objectives
* What is source code management
* What is Git
* What is GitHub
* What is the difference between Git and GitHub
* How to create a repository
* What is a README
* How to write good READMEs
* How to commit
* How to write helpful commit messages
* How to push code
* How to pull updates
* How to create a branch
* How to merge branches
* How to work as collaborators on a project
* Which files should and which files should not appear in your repo
### Additional info
#### Install git
If git is not already installed on your terminal:
```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```
#### Basic usage
```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```
#### Clone a repository using a personal Token
```
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository
```
### Quiz answers
* Question #0
	- You have the following files in your project directory:

```
julien@ubuntu:/tmp/git_project$ ls
0-test  0-test~ #0-test# file1  file2
```

	- You’ve edited 0-test and you want to add it to your GitHub repo. What is the correct command to add only 0-test?
		- git add 0-test
* Question #1
	- What command can you use to see what changes have been staged, which haven’t, and which files aren’t being tracked by Git?
		- git status
