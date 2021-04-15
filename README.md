# dotfiles
```sh
git clone --bare --single-branch --depth 1 --config status.showUntrackedFiles=no --config core.sparseCheckout=true -- https://github.com/dougimus/dotfiles.git $HOME/.dotfiles
echo '/*' > .dotfiles/info/sparse-checkout
echo '!README.md' > .dotfiles/info/sparse-checkout
git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME checkout
```
