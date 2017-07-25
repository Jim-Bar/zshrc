# How to use this zshrc

  - Clone the repository to `/etc/zsh/zshrc.d` (create this directory)
  - Then in `/etc/zsh/zshrc`, add:

```zsh
if [ -d zshrc.d ]; then
    source `ls zshrc.d`
else
    echo "zshrc.d not found."
fi
```
