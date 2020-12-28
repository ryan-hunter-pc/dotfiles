# My Dotfiles

These are my local overrides, intended to be used with [Thoughtbot's Dotfiles](https://github.com/thoughtbot/dotfiles), in `~/dotfiles-local`, which is the supported method for personal config overrides, and will be pulled in automatically when running `rcup`.

## New Machine Setup

These are all the steps needed to set up a new Rails development environment with my usual tools, including configuring these dotfiles.

1. Download and run [Thoughtbot's laptop script](https://github.com/thoughtbot/laptop)
2. Install [Thoughbot dotfiles](https://github.com/thoughtbot/dotfiles)
3. [Generate SSH key](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key) and register it in GitHub account:
    1. `ssh-keygen -t ed25519 -C "rymalhunt@gmail.com"`
    2. `pbcopy < ~/.ssh/id_ed25519.pub` to copy the key to clipboard (Mac only)
4. Clone this repo to `~/dotfiles-local`: `git clone git@github.com:ryan-hunter-pc/dotfiles.git ~/dotfiles-local`
5. From the home directory, run `rcup` to update the dotfile symlinks to include these overrides.
6. Login to Heroku CLI: `heroku login`. ([Install](https://devcenter.heroku.com/articles/heroku-cli) if needed, but as of this writing it is installed by step #1)

## Updating these overrides

After making any updates to these `*.local` files, you must run `rcup` from the home directory for the updates to be picked up.
