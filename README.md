# My Dotfiles

These are my local overrides, intended to be used with [Thoughtbot's Dotfiles](https://github.com/thoughtbot/dotfiles).

## Install on a new machine

1. Follow the instructions to install the [Thoughbot dotfiles](https://github.com/thoughtbot/dotfiles).
2. Install these overrides to `~/dotfiles-local` as recommended in the Thoughtbot dotfiles readme: `git clone git@github.com:ryan-hunter-pc/dotfiles.git ~/dotfiles-local`
3. From the home directory, run `rcup` to update the symlinks to include these overrides.

## Updating these overrides

After making any updates to these `*.local` files, run `rcup` from the home directory to update the symlinks or else the updates will not be picked up.
