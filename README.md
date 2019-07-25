# dotfiles-public
My public dotfiles forked from [romkatv/dotfiles-public](https://github.com/romkatv/dotfiles-public).

# Using these
There are two scripts to get things up and running. First run
`bin/boostrap-dotfiles.sh`, then run `setup-machin.sh`.

**boostrap-dotfile.sh**
Clones the `dotfiles-public` and `dotfiles-private` git repos locally to
`$HOME/.dotfiles_public` and `$HOME/.dotfiles-private`, while setting `$HOME` as the
`git` `work-tree`, so the actual contents of these repos will live there. This had the
advantage that additional configuration does not have to be done to point to a
`.dotfiles` directory.

**setup-machine.sh**
This script sets configuration for `gnome` and some `gnome` applications, as well as
installs desired Debian packages via `apt`. Some other fixes and system configuration is done
here, such as fixing the shared memory limit and gnu compiler.

There is some configuration left over from `romkatv`'s original repo that configure things
for an MS Window environment and `vscode`, which have been commented out for the time
being.
