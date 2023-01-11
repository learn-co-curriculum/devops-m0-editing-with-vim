# Editing with Vim

## Learning goals

- Learn what modal editors are
- Understand the pros and cons of `vim` and `nano`
- Learn the basics of `vim`

## Introduction

As we briefly touched on earlier, **vim** is a CLI text editor that is widely used by programmers and system administrators. It was first released in the early nineties by *Bram Moolenaar*, and ever since has become a popular choice for exiting text due to its efficiency and flexibility.

As a beginner, you might find `vim` intimidating, but after a bit of practice you will see just how efficient and ergonomic editing text using just your keyboard can be!

## Standard usage

To open `vim`, like with nano, just run the `vim` or `vim <file>` command:

```bash
$ vim file.txt
```

Welcome to `vim`! You should see a mostly empty screen, and a blinking cursor. 

`vim` is what is known as a *modal* editor. A **modal editor** is simply an editor that revolves around *modes*, each mode having its own set of commands and capabilities.

The mode you find yourself in out-of-the-box is fittingly-enough known as **Normal mode**. You can use this mode to navigate through the text, execute commands, and perform some other actions. Since our file is currently empty, we're not doing anything here yet.

Press `i` to go into `insert` mode. **Insert mode** allows you to type and edit text in the document; this is essentially the same as `nano`, minus the shortcuts. You can type text in this mode as you would in any other text editor.

Write a few lines of text to get started, anything you want! Once you're done, press `Esc` to go back to `normal` mode.

> Note: You can tell what mode you're in by looking at the bottom left of the screen. If you see `-- INSERT --`, you know you are in `insert` mode. Otherwise, you are most likely in normal mode.

There are a lot of commands you can use in `normal` mode; for an extensive list, [check out this cheat sheet.](https://vim.rtorr.com/)

Generally, the commands you will find yourself using the most in `normal` mode are the following:

- `h`, `j`, `k`, `l`: These move the cursor left, down, up, and right, respectively. You can use the arrow keys as well, but it's encouraged to use these since they line up comfortably with the home row on the keyboard, making it faster to navigate.
- `w`: Takes you to the beginning of the next word.
- `b`: Takes you to the beginning of the previous word.
- `0` and `$`: Move the cursor to the beginning and end of the current line, respectively.
- `gg` and `G`: Move the cursor to the beginning and end of the document, respectively.
- `x`: Deletes the character under the cursor.
- `dd`: Deletes the entire current line.
- `yy`: Copies the current line.
- `p`: Pastes text currently in the clipboard.

There are a lot more shortcuts available, but these will get you through the door. Try moving around the text you typed earlier, using `w` and `b` to move between words, and getting used to switching between `insert` and `normal` mode to modify the text.

## Commands

In `normal` mode, you can also use various commands preceded by a `:` for actions that are unbounded by default to a shortcut/hotkey.

Here are some of the most common ones:

- `:w`: Saves the current document.
- `:q`: Quits `vim`.
- `:wq`: Writes the current document and quits.
- `:e <filename>`: Opens a new file with that name in `vim`. If the file doesn't exist, it will be created when you save.

After typing the command (you can see what you are typing at the bottom-left of the screen), hit `enter` to execute it. Alternatively, press `Esc` to cancel.

## Conclusion

While certainly daunting at first, learning `vim` can be a rewarding way to improve your efficiency editing text in the terminal (or in general). At the end of the day, it's up to you which editor you wish to use, but it's certainly worth giving modal editors a real chance before deciding to opt out.

Some other terminal editors worth checking out on your own time if you like `vim`:

- https://github.com/neovim/neovim
- https://github.com/helix-editor/helix
- https://github.com/zyedidia/micro