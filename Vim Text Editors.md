# Vim text editors 

Vim, like its predecessor Vi, follows a modal editing paradigm. Modal editing means that Vim has different modes, and each mode has a specific purpose and set of commands. Here are the main modes in Vim.

**Normal Mode**	:- This is the default mode when you launch Vim. In normal mode, you can navigate the file, issue commands, and perform various editing operations. Some common commands in normal mode include.
           
| Key | Description |
| --- | --- |
| h, j, k, l | These keys allow you to move the cursor left, down, up, and right, respectively. |
| x | Deletes the character under the cursor. |
| dd | Deletes the entire line. |
| yy | Yanks (copies) the current line. |
| p | Pastes the yanked or deleted text. |
| u | Undo. |
| dw | Deletes the word under the cursor. |
| D | Delete from the current cursor position to the end of the current line. |
| cw | Change from the current cursor position to the end of the current word. |
| C | Change from the current cursor position to the end of the current line. |
| o | The o is used to open a new line below the current line and enter insert mode. |
| O | The O command is similar to the o command, but it opens a new line above the current line and enters insert mode. |
| J | The J command is used to join the current line with the line below it by removing the line break. |

**Insert Mode(i)** :- In insert mode, you can directly type and edit text. To enter insert mode from normal mode, press i (for insert) or any other insert mode command, such as a (append) or o (open a new line below and start inserting). In insert mode, you can freely type and edit text as you would in a traditional text editor.

**Visual Mode(v,V)** :- Visual mode allows you to select and manipulate blocks of text. You can enter visual mode by pressing v in normal mode. From there, you can move the cursor to select text character by character, line by line, or in rectangular blocks. Once you have selected the desired text, you can perform various operations on it, such as copying, cutting, or deleting.

**Command-Line Mode(:)** :- Command-line mode is used for entering commands and performing specific actions. To enter command-line mode from normal mode, press : (colon). Once in command-line mode, you can enter commands, such as saving the file, searching for text, or executing macros. Some commonly used commands include.

| key   | Description                                                   |
| ---------- | ------------------------------------------------------------- |
| w          | Saves the file.                                               |
| q          | Exits Vim.                                                    |
| set nu     | The `set nu` command is used to enable line numbering in the editor. |
| /          | The `/` command is used to initiate a forward search within the file. |
| s/old/new/g | Searches for "old" and replaces it with "new" globally in the file. |
| q!         | The `q!` command is used to forcefully quit the editor without saving any changes. |
| help       | Opens the built-in Vim help documentation.                     |
