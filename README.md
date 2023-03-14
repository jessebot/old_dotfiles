# OLD Dot Files for `onboardme`
These files are no longer maintained but may be of use to someone :) Checkout [jessebot/dot_files](https://github.com/jessebot/dot_files) for my current dot files :)

These directories/files are installed to your home directory and follow the [XDG Base Directory Spec] as closely as possible.

### Sections for each config directory/file

<details>
  <summary><code>.config</code></summary>

  <blockquote>

  <details>
  <summary><code>hyper</code></summary>

  <blockquote>

  File: [`~/.config/hyper/.hyper.js`](.config/hyper/.hyper.js)

  Sensible defaults for the [hyper](https://hyper.is) terminal emulator.

  </blockquote>

  </details>

  <details>
    <summary><code>iterm2</code></summary>

  <blockquote>

  [iterm2] is a terminal emulator for macOS.

  Symlinked File:  [`~/.config/iterm2/Profiles.json -> ~/Library/Application\ Support/iTerm2/DynamicProfiles/Profiles.json`](Library/Application\ Support/iTerm2/DynamicProfiles/Profiles.json)

  ### Profiles.json
  Sets some basic profiles:
  - default - profile with spacechalk colorscheme,
  - minimal - profile with basically nothing special and a plain `.bash_profile`.

  ###

  </blockquote>

  </details>

  <details>
    <summary><code>karabiner</code></summary>

  <blockquote>

  File: [`~/.config/karabiner/karabiner.json`](.config/karabiner/karabiner.json)

  Config file for [karabiner](https://karabiner-elements.pqrs.org/),
  which is used to map capslock to control on macOS and other key remapping that
  can be really useful.

  </blockquote>

  </details>

  <details>
    <summary><code>kitty</code></summary>

  <blockquote>

  Files:
  - [`~/.config/kitty/kitty.conf`](.config/kitty/kitty.conf)
  - [`~/.config/kitty/kitty-dark.png`](.config/kitty/kitty-dark.png)

  Config files related to [kitty], a terminal emulator. Cute open source
  kitty icon image by [DinkDonk], as well as a basic `kitty.conf` to
  use some [nerdfonts], and set up look and feel on macOS. I don't use this
  terminal emulator much anymore so I'm not sure how well this still works
  accross different OSes.

  </blockquote>

  </details>


  <details>
    <summary><code>lsimg</code></summary>

  <blockquote>

  File: [`~/.config/lsimg/config.yaml`](.config/lsimg/config.yaml)

  This is a local project that I'm working on to rewrite a bash script in python,
  to do basic checking of images in the terminal. I might remove it though,
  because after discovering [ranger], it might not be really needed :shrug:

  </blockquote>

  </details>

  <details>
    <summary><code>powerline</code></summary>

  <blockquote>

  Configuration files for [powerline], a status line for [BASH] and [tmux]. We enable a [spacechalk] color theme as well as:
  - local IP address
  - hostname
  - current working directory
  - git status info
  - unread mail count
  - kubernetes info
  - laptop battery information
  - the time
  - status of last run command (only appears if exit code is not 0)

  Currently working on getting mail notifications working.

  Files for colors:
  - [`~/.config/powerline/colors.json`](.config/powerline/colors.json)
  - [`~/.config/powerline/colorschemes/default.json`](.config/powerline/colorschemes/default.json)
  - [`~/.config/powerline/colorschemes/shell/default.json`](.config/powerline/colorschemes/shell/default.json)

  Files for configuring powerline for a login shell, and the console shell:
  - [`~/.config/powerline/themes/shell/default.json`](.config/powerline/themes/shell/default.json)
  - [`~/.config/powerline/themes/powerline.json`](.config/powerline/themes/powerline.json)
  - [`~/.config/powerline/themes/powerline_terminus.json`](.config/powerline/themes/powerline_terminus.json)
  - [`~/.config/powerline/themes/unicode_terminus.json`](.config/powerline/themes/unicode_terminus.json)

  File for configuring [tmux] status line:
  - [`~/.config/powerline/themes/tmux/default.json`](.config/powerline/)

  </blockquote>

  </details>

  <details>
    <summary><code>terminator</code></summary>

  <blockquote>

  File: [`~/.config/terminator`](.config/terminator)

  Default config for my favorite terminal from my starting days in tech, [terminator].
  We set some basic [spacechalk]-esk colors, transparency, and mononoki fonts.

  </blockquote>

  </details>


  <details>
    <summary><code>tmux</code></summary>

  <blockquote>

  File: [`~/.config/tmux/tmux.conf`](.config/tmux/tmux.conf)

  Config file for [tmux]. Currently, it will:
  - Sets 256 colors
  - enable the [powerline] tmux status line

  </blockquote>

  </details>

  <details>
    <summary><code>vim</code></summary>

  <blockquote>

  Configuration for [vim], a text editor, and it's plugins, installed via
  [vim-plug]. I am no longer actively using this vim configuration, and it will likely be archived soonish.

  [`~/.config/vim/vimrc`](.config/vim/vimrc) is the main file for the global vim configuration.
  We set a lot of defaults, including:
  - making vim use the [XDG Base Directory Spec]
  - setting window width to 82 characters
  - enabling line numbers
  - enabling highlighting of column cursor is on
  - add a colored column on column 80 for tidy python
  - sets a nerd font for vim
  - enable syntax highlighting
  - use [spacechalk] colorscheme
  - configure icons for VimDevicons, and NERDTree
  - ale icons changed, ale linters and fixers set for python
  - gitgutter icons
  - folding defaults
  - sets backups to XDG standard
  - allow backspace in insert mode
  - default tabbing
  - set search history
  - installs all the plugins [here](https://github.com/jessebot/dot_files/blob/main/.vimrc#L452)
  - uses template files below

  Auto-install vim-plug:
  - [`~/.vim/autoload/plug.vim`](.vim/autoload/plug.vim)

  Files for syntax highlighting for python, ssh_known_hosts, and .toml files:
  - [`~/.vim/syntax/python.vim`](.vim/syntax/python.vim)
  - [`~/.vim/syntax/ssh_known_hosts.vim`](.vim/syntax/ssh_known_hosts.vim)
  - [`~/.vim/syntax/toml.vim`](.vim/syntax/toml.vim)

  Files for default values in a python or markdown file:
  - [`~/.vim/templates/template.md`](.vim/templates/template.md)
  - [`~/.vim/templates/template.py`](.vim/templates/template.py)


  Since we install the [NERDTree](https://github.com/preservim/nerdtree) plugin,
  `:NERDTreeToggle` enables a directory tree of your current directory on the left hand side of your current vim window.
  </blockquote>

  </details>

</details>

<details>
  <summary><code>.cron</code></summary>

   <blockquote>
  local cron jobs for alarms, and package manager updates
    </blockquote>

</details>

<details>
  <summary><code>.local</code></summary>

  <blockquote>

  Directories:

  <details>
    <summary><code>bin</code></summary>

  <blockquote>

  Files:
  - [`~/.local/bin/utc`](.local/bin/utc)
  - [`~/.local/bin/w3msplits`](.local/bin/w3m-splits)

  This is just where we throw a few really simple scripts like:

  | Command         | Description                                                 |
  |-----------------|-------------------------------------------------------------|
  | `utc`           | for ease of use printing the time in UTC                    |
  | `w3m-splits`    | open split in iterm2 and send a website or HTML file to w3m |

  `w3m-splits` is mostly useful for [NeoMutt], but anything is possible :shrug:

  Directories:

  <details>
    <summary><code>iterm2</code></summary>

  <blockquote>

  Directory:
  - [`~/.local/bin/iterm2`](.local/bin/iterm2)

  Everything in there are files written and provided by iTerm2 for integrating iterm2 magic into your terminal. The only custom one is the following:

  | Command         | Description                                    |
  |:---------------:|:-----------------------------------------------|
  | `it2split`      | Open split in iterm2 with your default profile |

  </blockquote>

  </details>

  </blockquote>

  </details>

  <details>
    <summary><code>share</code></summary>

  <blockquote>

  Mostly READMEs to generate directory structure, but also some fastfetch preset configs.

  </blockquote>

  </details>

  <details>
    <summary><code>state</code></summary>

  <blockquote>

  This directory and the director[y/ies]/file(s) within it are specifically to auto-generate directory structure so that XDG spec is enforced with tools that only loosely enforce it.

  </blockquote>

  </details>

</details>

<details>
  <summary><code>.gitignore</code></summary>

  <blockquote>

  Git ignore file for all sorts of things in your home directory that should
  never get committed if this repo is used as your home directory dot files.

  </blockquote>

</details>

<details>
  <summary><code>.hushlogin</code></summary>

  <blockquote>

  This just silences the last login message of shells.

  </blockquote>

</details>

<details>
  <summary><code>.zshrc</code></summary>

  <blockquote>

  Recently started giving this some TLC, but still in it's infancy to be match the .bash configs. Currently we:
  - set some useful aliases
  - set the same powerline prompt as bash

  </blockquote>

</details>


Please feel free to fork this repo and make it your own.
You can still use `onboardme`, but you'll want to pass in _your_ git URL and branch. Example:

```bash
# this uses your personal git URL and makes sure to always pull from main
# if you want to overwrite your existing dot files, you can also add --overwrite to this command
onboardme --git_url https://github.com/your_username/dot_files --git_branch main
```

<!-- ♡  ♡  ♡  ♡  ♡  ♡  ♡  ♡  ♡  Link References ♡  ♡  ♡  ♡  ♡  ♡  ♡  ♡  ♡ -->

<!-- general -->
[bw]: https://bitwarden.com/help/cli "bitwarden CLI"
[powerline]: https://github.com/powerline/powerline "powerline"
[sixel]: https://en.wikipedia.org/wiki/Sixel "sixel"
[tmux]: https://github.com/tmux/tmux "tmux"
[TUI]: https://en.wikipedia.org/wiki/Text-based_user_interface "TUI"
[XDG Base Directory Spec]: https://wiki.archlinux.org/title/XDG_Base_Directory#User_directories

<!-- ------------------------ Fonts and Colors -------------------------- -->
[nerdfonts]: https://www.nerdfonts.com/ "nerdfonts"
[powerline fonts]: https://github.com/powerline/fonts "powerline fonts"
[spacechalk]: https://github.com/space-chalk/spacechalk.vim "spacechalk colorscheme for vim"

<!-- ------------------------------- Kubernetes --------------------------- -->
[krew]: https://krew.sigs.k8s.io/ "krew, plugin manager for kubectl"
[kubectl]: https://kubernetes.io/docs/reference/kubectl/kubectl/ "cli for kubernetes"

<!-- ---------------------- Terminal emulators ---------------------- -->
[iterm2]: https://iterm2.com/ "iterm2"
[kitty]: https://sw.kovidgoyal.net/kitty/ "kitty, a terminal emulator"
[DinkDonk]: https://github.com/DinkDonk/kitty-icon "kitty-icon"

<!-- ------------------------- Vim ---------------------------- -->
[airline]: https://github.com/vim-airline/vim-airline "airline"
[ale]: https://github.com/dense-analysis/ale "ale: asynchonous linting engine"
[vim]: https://www.vim.org/ "vim, a text editor"
[vim-plug]: https://github.com/junegunn/vim-plug "plugin manager for vim"
