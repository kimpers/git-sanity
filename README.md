# git-sanity
Helps make sure you're not doing stupid things in Git by mistake.

## Features
* Prompts for verification before allowing pushes to the `master` branch

## Setup

1. Clone repo `git clone git@github.com:kimpers/git-sanity.git .`
2. Create a git templates folder `mkdir -p ~/.git-templates/hooks`
3. Create symlinks for the sanity checks that you want to use. Eg. `ln -s ~/path/to/git-sanity/pre-push ~/.git-templates/hooks`
4. Enable hooks `git config --global init.templatedir '~/.git-templates'`
5. Make sure the hooks are executable. Eg. `chmod a+x ~/.git-templates/hooks/pre-push`
5. Re-initialize git in each repo where you want sanity `git init`
