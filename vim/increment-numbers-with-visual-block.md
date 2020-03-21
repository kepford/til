# Increment numbers on multiple lines in visual block mode

Source: [Making a list of numbers | Vim Tips Wiki | Fandom](https://vim.fandom.com/wiki/Making_a_list_of_numbers#Incrementing_selected_numbers)

I commonly need to convert a list to a ordered markdown list.

Example:

```
First item
Another
And Another
Yet another
```

At the first letter of the of the first line enter visual block mode by pressing `Ctrl-v`. Press `3j` to select the block. Now press `Ctrl-I` and type `0. `.

```
0. First item
0. Another
0. And Another
0. Yet another
```

You now have `0. ` on each line. Now we need to increment each number by one. Press `gv` to select your previous block of text. Next press `g` and then `Ctrl-a` and your list will look like this.

```
1. First item
2. Another
3. And Another
4. Yet another
```

