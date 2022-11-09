## Guide to  install packages in your goinfre

We may receive an error when we try to install a package, which indicates that we do not have permission to write to the directories that npm uses to store packages and commands.
 We can fix this problem by Changing the npm's default directory to another. We can configure npm to use a different directory; this directory will be hidden in our goinfre.

Make a directory for installations:

```mkdir ~/goinfre/.npm```

Make a symbolic link to .npm directory:

```ln -s ~/goinfre/.npm ~/.npm ```

Create ~/.npmrc file:

```touch ~/.npmrc ```

Configure npm to use the new directory path:

```npm config set prefix /Users/YOUR_LOGIN/.npm ```

## ZSH Users
if u have ZSH u need to add path to your .zshrc open ur .zshrc file with vim :

```vim .zshrc ```

then paste the path:

```export PATH=~/goinfre/.npm/bin:$PATH```

## Now u can install your packages enjoy😝
