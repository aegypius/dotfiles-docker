# Dotfiles: Docker

This is my docker dotfiles storage

## Installation

### 1. Get the code

You can install this repository using either one of these method:

#### Using bootstrap script
    bash <(curl -sL https://raw.githubusercontent.com/aegypius/dotfiles-docker/master/bootstrap.bash)

#### Using homeshick

```shell
homesick clone aegypius/dotfiles-docker
```

### 2. Inject it in your environment

Then you need to update your `.bashrc` with the following code:

```shell
# Source everything in ~/bashrc.d {{{
if [ -d ~/.bashrc.d ]; then
  for script in ~/.bashrc.d/*; do
    test -f $script && source $script;
  done;
fi
# }}}
```

### See Also

  - [aegypius/dotfiles](https://github.com/aegypius/dotfiles-docker): My personal dotfiles canonical repository
  - [aegypius/dotfiles-wrapped](https://github.com/aegypius/dotfiles-wrapped): Useful wrappers for containerized environments.
