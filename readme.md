dotmanager
==========

dotmanager is bash script for easy manage your dotfiles

#### Installing

```bash
wget https://git.io/JvKXM
chmod +x JvKXM
mv JvKXM ~/bin/dotmanager
```


#### Using

```
Usage: dotmanager -d dir -c command
```

You may store all dotfiles in general directory.

For Example if you have nvim directory with configure you can execute ```dotmanager -d nvim -c add```. The script will create links to these files in the home directory

```
nvim
└── .config
    └── nvim
        ├── basic.vim
        ├── extended.vim
        ├── init.vim
        └── plugins_config.vim
```

```
~/
└─ nvim
    ├── basic.vim -> ../dotfiles/nvim/.config/nvim/basic.vim
    ├── extended. -> ../dotfiles/nvim/.config/nvim/extended.vim
    ├── init.vim -> ../dotfiles/nvim/.config/nvim/init.vim
    └── plugins_config.vim -> ../dotfiles/nvim/.config/nvim/plugins_config.vim
```

To delete, execute ```manager -d nvim -c delete```
