---
layout: post
title:  "Supercharging VIM"
date:   2018-04-03
description: A quickstart description of how to set up VIM for code development.
---


I decided that I want to set up `vim` as my developer environment. This is mostly because I love `vim`, but also for the smaller projects that I work on some of the available IDEs feel too heavy and unnecessary. In general, the tools described below are useful even if you are not doing code development. Things like being able to navigate through the file tree and see syntax highlighting, search for other files etc are nice in any scenario. This setup should take 20 - 30 minutes.

So let's go from:

<figure>
	<img src="{{ '/assets/images/basic_vim.png' | prepend: site.baseurl }}" alt="" width="750"> 
	<figcaption>Vim before. </figcaption>
</figure>

To:


<figure>
	<img src="{{ '/assets/images/nice_vim.png' | prepend: site.baseurl }}" alt="" width="750"> 
	<figcaption>Vim after. </figcaption>
</figure>

in a few easy steps.

## Package manager

This takes all the pain out of installing new plugins.

* `vundle` seems like a good option.
* [A very thorough guide](https://www.digitalocean.com/community/tutorials/how-to-use-vundle-to-manage-vim-plugins-on-a-linux-vps) on how to set up `vundle`.
* A quick-start guide for the impatient:
	* Clone the repo `git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle`.
	* Edit your `~/.vimrc`:

```bash
"""" START Vundle Configuration
"""" Vundle is a VIM package manager - all plugins go in here
 
set nocompatible              " be iMproved, required
filetype off                  " required
 
" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()

" " let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'
 
```

 Plugins go here

```bash
" All of your Plugins must be added before the following line
call vundle#end()            " required
filetype plugin indent on    " required
 
"""" END Vundle Configuration
```

## A file tree navigator

This lets you see where you are in the filesystem. It also lets you browse through and look for other files that could be of interest.

* `NERDTree` is the clear choice.
* Allows you to open a file tree from vim and navigate through.
* I suggest enabling the mouse, add `set mouse=r` to `~/.vimrc`.
* Note, you can use `ctrl`+`w` to toggle between the tabs.
* To open up the tree from `vim`, just type `:NERDTree`.
* Standard `vim` commands can close the tree `:q`.

## A Tagbar

Tagbars are used for navigating code. A tag bar shows the tags of the current file. The tags are things like classes, functions and variables in a code file. 

* OSX - get exuberant ctags `brew install ctags`.
* Open up `vim` and use `vundle` to search for packages Tagbar.

```bash
:PluginSearch Tagbar
```

* Navigate to the `Tagbar` package and hit `i`.
* Now simply add `Plugin 'Tagbar'` line to your `~.vimrc` in the `Plugins go here section`.
* To use `:TagbarToggle` turns it on/off.

## Tab completion

Because of course you want tab completion. `Supertab` is a good option.

* Open `vim`.
* `:PluginSearch supertab`.
* Navigate to `supertab` and hit `i`.
* Now simply add `Plugin 'supertab'` line to your `~.vimrc` in the `Plugins go here section`.
* To use, just hit tab while typing.

## A fuzzy finder

<figure>
	<img src="{{ '/assets/images/fuzzy_finder.png' | prepend: site.baseurl }}" alt="" width="500"> 
	<figcaption>An example of what the search function looks like. </figcaption>
</figure>

Just like Google or Mac spotlight search, `fzf` gives you autocomplete finding (allowing for spelling mistakes etc) from the command line! And, you can plugin to `vim` to allow for fuzzy searching of your file system from your favourite text editor! See [this video](https://www.youtube.com/watch?v=1a5NiMhqAR0) of examples of how useful it can be.

* Download `fzf`:

```bash
brew install fzf
```

* Add the following to your `.vimrc`:

```bash
Plugin 'junegunn/fzf'
Plugin 'junegunn/fzf.vim'
```

* Open `vi` and run:

```bash
:PluginInstall
```

* To use:
	* `:Files <path>` searches in `<path>` for files.
	* `:Buffers` open buffers.
	* `:History` command history.
	* `:Commits` Git commits.
	* [Many more](https://github.com/junegunn/fzf.vim).

## Airbar

<figure>
	<img src="{{ '/assets/images/airbar.png' | prepend: site.baseurl }}" alt="" width="750"> 
	<figcaption>This airbar looks the business. </figcaption>
</figure>

I'm not going to lie, although airbars are useful, this one is more about the look than the utility. It just sits at the bottom of the screen making you look like a pro. Although it does give useful information like the file format, the mode you are in.

* Add the following to your `.vimrc`:

```bash
Plugin 'vim-airline/vim-airline'
```

* Open `vi` and run:

```bash
:PluginInstall
```
