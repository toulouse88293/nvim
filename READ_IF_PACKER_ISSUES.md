# Trouble with trouble.nvim
What helped was adding `opt=true` to configuration of this plugin inside the `packer.lua` file
Additionally after this you should clear packer cache and reinstall it:
```
rm -rf ~/.local/share/nvim/site/pack/packer/start/*
rm -rf ~/.local/share/nvim/site/pack/packer/opt/*
rm -rf ~/.local/share/nvim/site/pack/packer/compile/*
```
and then
```
git clone --depth 1 https://github.com/wbthomason/packer.nvim \
  ~/.local/share/nvim/site/pack/packer/start/packer.nvim

```
