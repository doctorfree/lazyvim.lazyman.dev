---
layout: post
title: LazyVim Configurations
toc: true
post_style: page
---

<h2>Lazyman Supported LazyVim Neovim Configurations</h2>

The following are [Lazyman](https://lazyman.dev) supported
[LazyVim](https://lazyvim.org){:target="_blank"}{:rel="noopener noreferrer"}
based Neovim configurations:

| LazyVim |        |        | Configurations |
| :------ | :----: | :----: | -------------: |
| [LazyVim](https://lazyvim.lazyman.dev/posts/LazyVim) | [Barebones](https://lazyvim.lazyman.dev/posts/Barebones) | [CatNvim](https://lazyvim.lazyman.dev/posts/CatNvim) | [Elijah](https://lazyvim.lazyman.dev/posts/Elijah) |
| [JustinNvim](https://lazyvim.lazyman.dev/posts/JustinNvim) | [JustinOhMy](https://lazyvim.lazyman.dev/posts/JustinOhMy) | [LazyIde](https://lazyvim.lazyman.dev/posts/LazyIde) | [Nv](https://lazyvim.lazyman.dev/posts/Nv) |
| [Penguin](https://lazyvim.lazyman.dev/posts/Penguin) | [Traap](https://lazyvim.lazyman.dev/posts/Traap) | [Webdev](https://lazyvim.lazyman.dev/posts/Webdev) | |

Install all Lazyman supported LazyVim configurations with the command `lazyman -i lazyvim`.

## 📦 What is LazyVim

[LazyVim](https://lazyvim.org){:target="_blank"}{:rel="noopener noreferrer"}
is one of the most popular Neovim "distributions"
along with [AstroNvim](https://astronvim.lazyman.dev),
[LunarVim](https://lunarvim.lazyman.dev), and
[NvChad](https://nvchad.lazyman.dev). These aren't really distributions,
they do not include Neovim, but that is what they are called. They are more
accurately described as "Neovim configuration frameworks". In most cases they
provide some pre-configuration of plugins as well as an easy way to extend
the base configuration.

A Neovim configuration framework can be of considerable assistance in managing
the exploding Neovim plugin ecosystem, quickly and easily incorporating
advanced features, and maintaining an up-to-date Neovim configuration.

Features that distinguish LazyVim include:

- Very well maintained by the author of `lazy.nvim`
- Nice architecture, it's a plugin with which you can `import` preconfigured plugins
- Good documentation

Read our overview and comparison of
[Neovim configuration distributions](https://lazyman.dev/posts/Configuration-Distributions).

## 🌟 Overview

LazyVim is a Neovim setup powered by
[💤 lazy.nvim](https://github.com/folke/lazy.nvim){:target="_blank"}{:rel="noopener noreferrer"}
to make it easy to customize and extend your config.
Rather than having to choose between starting from scratch or using a
pre-made distro, LazyVim offers the best of both worlds - the flexibility
to tweak your config as needed, along with the convenience of a pre-configured setup.

![image](https://user-images.githubusercontent.com/292349/211285846-0b7bb3bf-0462-4029-b64c-4ee1d037fc1c.png)

![image](https://user-images.githubusercontent.com/292349/213447056-92290767-ea16-430c-8727-ce994c93e9cc.png)

## ✨ Features

- 🔥 Transform your Neovim into a full-fledged IDE
- 💤 Easily customize and extend your config with [lazy.nvim](https://github.com/folke/lazy.nvim){:target="_blank"}{:rel="noopener noreferrer"}
- 🚀 Blazingly fast
- 🧹 Sane default settings for options, autocmds, and keymaps
- 📦 Comes with a wealth of plugins pre-configured and ready to use

## ⚡️ Requirements

- Neovim >= **0.8.0** (needs to be built with **LuaJIT**)
- Git >= **2.19.0** (for partial clones support)
- a [Nerd Font](https://www.nerdfonts.com/){:target="_blank"}{:rel="noopener noreferrer"} **_(optional)_**
- a **C** compiler for `nvim-treesitter`. See [here](https://github.com/nvim-treesitter/nvim-treesitter#requirements){:target="_blank"}{:rel="noopener noreferrer"}

## 🚀 Getting Started

After installing and initializing [lazyman](https://lazyman.dev),
install the Lazyman Base LazyVim configuration with the command:

```shell
lazyman -l
```

Open the newly installed and initialized LazyVim configuration with

```shell
NVIM_APPNAME="lazyman/LazyVim" nvim
```

There's a great video created by
[@elijahmanor](https://github.com/elijahmanor){:target="_blank"}{:rel="noopener noreferrer"}
with a walkthrough to get started.

[![Watch the video](https://img.youtube.com/vi/N93cTbtLCIM/hqdefault.jpg){:target="_blank"}{:rel="noopener noreferrer"}](https://www.youtube.com/watch?v=N93cTbtLCIM)

## 📂 File Structure

The files under config will be automatically loaded at the appropriate time,
so you don't need to require those files manually.
**LazyVim** comes with a set of default config files that will be loaded
**_before_** your own. See [here](https://github.com/LazyVim/LazyVim/tree/main/lua/lazyvim/config){:target="_blank"}{:rel="noopener noreferrer"}

You can add your custom plugin specs under `lua/plugins/`. All files there
will be automatically loaded by [lazy.nvim](https://github.com/folke/lazy.nvim){:target="_blank"}{:rel="noopener noreferrer"}

<pre>
~/.config/nvim
├── lua
│   ├── config
│   │   ├── autocmds.lua
│   │   ├── keymaps.lua
│   │   ├── lazy.lua
│   │   └── options.lua
│   └── plugins
│       ├── spec1.lua
│       ├── **
│       └── spec2.lua
└── init.lua
</pre>

## ⚙️  Configuration

Refer to the [docs](https://lazyvim.github.io){:target="_blank"}{:rel="noopener noreferrer"}

<div align="center">
  <p align="center">
    <a href="https://ronrecord.com" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="domain"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/domain.png"
    /></a>
    <a href="https://www.reddit.com/user/No-Blackberry-3160" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="reddit"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/reddit.png"
    /></a>
    <a href="https://github.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="github"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/github.png"
    /></a>
    <a href="https://gitlab.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="gitlab"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/gitlab.png"
    /></a>
    <a href="https://twitter.com/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="twitter"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/twitter.png"
    /></a>
    <a href="https://youtube.com/c/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="youtube"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/youtube.png"
    /></a>
    <a href="https://linkedin.com/in/ronrecord" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="linkedin"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/linkedin.png"
    /></a>
    <a href="https://instagram.com/doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="instagram"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/instagram.png"
    /></a>
    <a href="https://noc.social/@doctorwhen" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="mastodon"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/mastodon.png"
    /></a>
    <a href="https://en.wikipedia.org/wiki/User:Doctorfree" target="_blank" rel="noopener">
      <img align="center"
      style="width:40px;height:40px"
      alt="wikipedia"
      src="https://raw.githubusercontent.com/doctorfree/doctorfree/master/icons/wikipedia.png"
    /></a>
  </p>
</div>
