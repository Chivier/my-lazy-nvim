# ๐ค LazyVim

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## โจ Features

- ๐ฅ Transform your Neovim into a full-fledged IDE
- ๐ค Easily customize and extend your config with [lazy.nvim](https://github.com/folke/lazy.nvim)
- ๐ Blazingly fast
- ๐งน Sane default settings for options, autocmds, and keymaps
- ๐ฆ Comes with a wealth of plugins pre-configured and ready to use

## โก๏ธ Requirements

- Neovim >= **0.8.0** (needs to be built with **LuaJIT**)
- Git >= **2.19.0** (for partial clones support)
- a [Nerd Font](https://www.nerdfonts.com/) **_(optional)_**

## ๐ Getting Started

You can find a starter template for **LazyVim** [here](https://github.com/LazyVim/starter)


- Make a backup of your current Neovim files:

  ```sh
  mv ~/.config/nvim ~/.config/nvim.bak
  mv ~/.local/share/nvim ~/.local/share/nvim.bak
  ```

- Clone the starter

  ```sh
  git clone https://github.com/LazyVim/starter ~/.config/nvim
  ```

- Remove the `.git` folder, so you can add it to your own repo later

  ```sh
  rm -rf ~/.config/nvim/.git
  ```

- Start Neovim!

  ```sh
  nvim
  ```

  Refer to the comments in the files on how to customize **LazyVim**.


## ๐ File Structure

The files under config will be automatically loaded at the appropriate time,
so you don't need to require those files manually.
**LazyVim** comes with a set of default config files that will be loaded
**_before_** your own. See [here](https://github.com/LazyVim/LazyVim/tree/main/lua/lazyvim/config)

You can add your custom plugin specs under `lua/plugins/`. All files there
will be automatically loaded by [lazy.nvim](https://github.com/folke/lazy.nvim)

<pre>
~/.config/nvim
โโโ lua
โ   โโโ config
โ   โ   โโโ autocmds.lua
โ   โ   โโโ keymaps.lua
โ   โ   โโโ lazy.lua
โ   โ   โโโ options.lua
โ   โโโ plugins
โ       โโโ spec1.lua
โ       โโโ **
โ       โโโ spec2.lua
โโโ init.toml
</pre>

## โ๏ธ Configuration

Refer to the [docs](https://lazyvim.github.io)
