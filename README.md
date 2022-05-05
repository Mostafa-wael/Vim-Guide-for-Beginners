# Vim-Guide-for-Beginners
A lot of people are afraid of Vim and a lot of them have seen the nightmare of entering Vim and not being able to exit it. In this tutorial, we will go through the most important and basic commands in Vim and believe me, you will be able to use Vim as your primary editor if you have moved with the tutorial and applied what you read step by step. So, let's go!
![image](https://user-images.githubusercontent.com/56788883/167031824-97ed4847-53df-4d7c-9691-d7b86e6e8be3.png)


1. Before start, consider downloading this repository. As we will train on the examples on the **tutorial** file.
2. First thing to learn is how to open a file using Vim, to start Vim from the shell prompt type: `vim FILENAME <ENTER>`
3. Try moving the cursor using the `hjkl` keys -recommended- or the arrow keys -not recommended-
`h (left) j (down) k (up) l (right) `
4. Now, try to overcome your nightmare and exit vim by typing:

`<ESC> :q! <ENTER> to trash all changes.`
OR type: `<ESC> :wq <ENTER> to save the changes.`

5. Now, we will play with the text and try adding and removing some text:

- Insert new text before the cursor: `i <type inserted text> <ESC>`
- Append new text after the cursor: `a <type appended text> <ESC>`
- Append new text at the end of the line: `A <type appended text> <ESC>`
- Delete the character at the cursor: `x`
- Delete from the cursor to the end of a line: `d$`
- Delete a whole line: `dd`
- To put back text that has just been deleted: `p`. This puts the deleted text AFTER the cursor (if a line was deleted it will go on the line below the cursor).
- To open a line BELOW the cursor and start Insert mode: o`
- To open a line ABOVE the cursor: `O`
  
6. Now, you may ask why did we type `<ESC>` after every command? The answer is that Vim has two modes, the command mode and the insert mode. By default, we are in the command mode in which letters will map to its equivalent Vim command. But, for using Vim as a text editor we should enter the Insert mode, like what we did when we used `i` , `a` and `A` . Then, we typed `<ESC>` to return back to our command mode, it is that easy!

>> Note: You should try those commands and practice them as much as you can. Don’t move to the next point unless you are comfortable with the previous ones.

7. Now, after you have modified the file content try saving it using `:w FILENAME` which writes the current Vim file to disk with name FILENAME.

8. One of the things that makes Vim powerful, is its easy way to navigate through out the whole file, here are some of those commands:

- To move to the start of the line use a zero: `0`
- To display your location in the file and the file status: `CTRL-G`
- To move to the end of the file: `G`
- To move to a specific line: `<number> G`
- To move to the first line in the file: `gg`
- To move to the end of the word: `e`
  
9. Oops! you have made a typo?

- To undo previous actions: `u`(lowercase u)
- To undo the undo’s (Redo): `CTRL-R`
  
10. You are a developer and got bored of searching and matching brackets?

- Typing `% `while the cursor is on a (,),[,],{, or } goes to its match.
  
11. What about search & replacements? :

- Typing `/` followed by a phrase searches FORWARD for the phrase. Type `n` to get the next occurrence or `N` to return to the previous one.
- To substitute all occurrences in the file type: `%s/<old>/<new>/g`
- To ask for confirmation each time add c: `%s/<old>/<new>/gc`

12. What about copy & paste?

- Visually select text: `v <motion, either number or hjkl>`
- Yank (copy) text: `y`
- Put (paste) text: `p`
13. Don’t forget that we are still in the terminal, Vim allows you to execute some commands on the terminal without closing it, you can do it as follows:

- To execute a `<command>`: `:!<command>`
- Some useful examples -on (Unix)- are:
  - `:!ls` shows a directory listing.
  - `:!rm FILENAME` removes file FILENAME.

14. We have done so much until now! and this commands are more than enough for you to start with. However, if you want to learn more, you can always use the help window:

- Open a help window, type `:help` or press `<F1>` or `<HELP>`
- Jump to another window, type `CTRL-W CTRL-W`
- Close the help window, type `:q`

15. Vim will not leave you alone, it supports intellisense when typing a `:command`:

- press `CTRL-D` to see possible completions.
- Press `<TAB>` to use one completion.
  
##### Hope this tutorial was a good starting point to kick start your journey with Vim. Don’t forget to follow me to get more of this tutorials and articles.
