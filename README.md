# Macbook Setup Guide For Web Programmer

Setting up a new Macbook will be tough and cumbersome. Every time I am getting a new Macbook, I go over the same steps on how to set it up for my working experience.

I create a record of my setup, hoping it's helpful for others too!

## Immediate Frist Steps

### Enable Tap to Click

When setting up a new Macbook, one of the first changes we make is enabling the tap-to-click feature for the trackpad.

Go「**System Preference -> Trackpad -> Point & Click**」and enable 「**Tap to click**」 option.

![](./enable-tap-to-click.png)

### Enable Three Finger Dragging

In general, "tap to click" on your Macbook to avoid a force-click on the trackpad. But this doesn't work when it comes to dragging and repositioning windows.

Also, I'm big fan of tree finger dragging.

1. Go 「**System Preference -> Accessibility**」.
2. In the Accessibility sidebar, choose option 「**Pointer Control**」.
3. Click the button 「**Trackpad Options**」.
4. Enable dragging and select 「**three finger drag**」.

![](./enable-three-finger-drag.png)

### Change Wallpaper

Visit [wallhaven](https://wallhaven.cc/) to find a wonderful wallpaper and replace the default ones.

### Download Edge

After discovering [chrome are eating my old Mac's battery](https://twitter.com/xiaokedada/status/1495037432273596419), I turned to use [edge](https://www.microsoft.com/zh-cn/edge).

![](./chrome-eats-battery.png)

## Install Homebrew

[Homebrew](https://brew.sh/) is "The Missing Package Manager for macOS".

Simply follow their installation guide, copy `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` to terminal.

> For [GFW](https://en.wikipedia.org/wiki/Great_Firewall) reasons, the Chinese users will fail to connect to github.

> Just copy `/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"` to your terminal. It will do the same thing when installing homebrew.

## Setup Terminal

Use [iTerm2](https://iterm2.com/) as macOS terminal replacement.

1. **Use the Homebrew to install iTerm2**

```shell
$ brew install --cask iterm2
```

2. **Change a few settings of iterm2**

+ Go 「**iterm2 Preferences -> Profiles -> Default -> Window**」, add transparency and blur.

![](./iterm2-blur.png)

+ Go 「**iterm2 Preferences -> Profiles -> Default -> Keys -> Key Mappings**」, replace the standard ones with the preset "Natural Text Editing".

![](./iterm2-natural-text-editing.jepg)

3. **Install Oh My Zsh**

The great thing about this is that you can customize your shell and add plugins. Unlike the old Bash shell, which does not look attractive and can make it difficult for you to use.

```shell
$ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

4. ***Choose your favorite theme**

There are [multiple themes](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes) you can choose from. My favorite theme is [honukai](https://github.com/oskarkrawczyk/honukai-iterm-zsh) and it should look like in the screenshot:

![](./honukai-theme.png)

For compelete guide, dive into it's [docs](https://github.com/oskarkrawczyk/honukai-iterm-zsh).

5. **Add useful oh-my-zsh plugins**

Oh My Zsh is powered by plugins. I'll share my top 4 plugins.

```text
plugins=(
 git
 autojump
 colorize
 zsh-syntax-highlighting
)
```

1. the `git` plugin

The [git](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git) plugin is enabled by default. It provides many aliases and a few useful functions.



To 

