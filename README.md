# mac-setup

### 1. Install dropbox

### 2. Install [MacPass](https://macpassapp.org/)

### 3. Login to github

NOTE: Here you can optionally clone & run setup of your dotfiles (step 5/6) now and make sure oh-my-zsh is in place so that the dotfiles setup script from Strapi properly aliases ~/.oh-my-zsh to /dev/dotfiles/.oh-my-zsh. Upside: not sure where Strapi puts dotfiles when executing direct from https://github.com/danielrob/dotfiles. By doing it now, it means that /dev/dotfiles becomes your live dotfiles. Downsides: You'll end up doing step 5 twice/or having to manually preserve the .ssh folder between cloning dotfiles and running setup, or the .ssh folder will get overridden. You'll also need to install command tools. Some optimisation to do here! 

### 4. Use [Strapi](https://macos-strap.herokuapp.com/) 
(Note: You may optionally edit https://github.com/danielrob/dotfiles and in particular https://github.com/danielrob/dotfiles/Brewfile) prior to running this). 

### 4 - manual: Complete manual steps as per https://github.com/danielrob/dotfiles/blob/master/script/strap-after-setup#L20

### 5. Add a [new ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

### 6. Git clone https://github.com/danielrob/dotfiles

```
$ cd ~
$ mkdir dev
$ cd dev
$ git clone --recurse-submodules https://github.com/danielrob/dotfiles
```
You'll probably now need to fixup the fact that Strapi didn't alias oh-my-zsh from your custom dotfiles since it's a submodule manually... see dotfiles/setup.sh script. You can ignore this if you completed step 5 & 6 before step 4. 

### 7. Copy [https://github.com/danielrob/ohmyzsh/blob/master/custom/themes/agnoster-custom.zsh-theme](agnoster-custom.zsh-theme) to ~/.oh-my-zsh/custom/themes

### 8. Copy fonts across to new computers font book from your personal dropbox. 

### 9. Open iterm and load the default profile from dropbox's default.json. 

### 10. Open vs code and turn on settings sync. Deselect ui-state. 
