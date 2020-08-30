# About

In `htop v3.0`, the `vim_mode` variable was added which toggles vim-like key mappings. This mode is very comfortable but some essential mappings are missing. Our patch introduces such shortcuts.

# Key Mappings

Our patch introduces the following key mappings.

- <kbd>Ctrl</kbd>+<kbd>u</kbd>: Scroll Up

- <kbd>Ctrl</kbd>+<kbd>d</kbd>: Scroll Down

- <kbd>Ctrl</kbd>+<kbd>k</kbd>: Send Signal

You can easily add or remove mappings by finding the keycodes (using for example [this code](https://stackoverflow.com/a/50443806/8776746)) and modifying the patch according to the result.

# Usage

```bash
patch < patch && ./autogen.sh && ./configure && make && sudo make install
```

<!-- vim: set spell: -->

