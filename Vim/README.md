**To use:** Move the `sayo.vim` file into your `{vim_runtime_dir}/colors` directory (by default, `~/.vim/colors` for vim and `~/.config/nvim/colors` for neovim), and ensure the following lines are present in your vimrc or init.vim:

```
syntax on
set termguicolors
colorscheme sayo
```

If this results in only black and white being displayed in your terminal, replace `set termguicolors` with the following (see `:h xterm-true-color` for more info):

```
let &t_8f = "\<Esc>[38:2:%lu:%lu:%lum"
let &t_8b = "\<Esc>[48:2:%lu:%lu:%lum"
```
