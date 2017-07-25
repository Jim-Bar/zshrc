# How to use this zshrc

  - Clone the repository to `/etc/zsh/zshrc.d` (create this directory)
  - Then in `/etc/zsh/zshrc`, append:

```zsh
# Load sub-zshrc files
local zshrc_root=/etc/zsh/zshrc.d
if [ -d $zshrc_root ]; then
    source `find $zshrc_root -maxdepth 1 -type f ! -name README.md`
else
    echo "$zshrc_root not found"
fi
```
