vim-listchars
===

(Neo)vim plugin that allows to cycle through different listchars configurations and when you finished
cycling between configurations disables display of invisible chars. 
Next activation will reenable it and start cycling again from your first entry.

To install
===
For vim-plug:
```
Plug 'jiftle/vim-jiftle-listchars'
```

How to configure
===

If you don't like the default values, you can setup your own list of configurations
```vim
let g:listchar_formats=[ 
   \"trail:·",
   \"tab:»·,eol:↲,nbsp:␣,extends:…,space:␣,precedes:<,extends:>,trail:·",
   \"tab:»·,nbsp:↲,trail:↲"
   \]
```

There is no default mapping, you have to add it yourself, for instance:

```noremap <F11> <Plug>(ToggleListchars)```


## 修改

- 默认显示控制字符(TAB，SPACE)

## History

- 2020-10-26
    - 默认不修改set list，避免影响.vimrc中的配置
