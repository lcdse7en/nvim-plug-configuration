### nvim常用插件使用说明
#### 1.vim-visual-multi
```vim
Plug 'mg979/vim-visual-multi'
```

| 快捷键        | 说明                                                     |
| ------------- | :------------------------------------------------------- |
| Ctrl + N      | 选择相同的单词进行同时修改,可以用于删除一对包裹的符号    |
| q             | 跳过当前选中的区域                                       |
| Ctrl + Down   | 创建向下的连续光标，同时修改                             |

#### 2.wildfire + surroud
1. wildfire
```vim
Plug 'gcmt/wildfire.vim'
```


| 快捷键 | 说明                                              |
|--------|---------------------------------------------------|
| Enter  | 选择引号、括号里的词，进入可视模式方便修改数据(c) |

2. surround
```vim
Plug 'tpope/vim-surround'
```

| 快捷键 | 说明                                                            |
|--------|-----------------------------------------------------------------|
| S"     | 进入可视模式选中单词，将单词用双引号包裹                        |
| cs"'   | 将双引号包裹的单词改为单引号包裹(不要进入可视模式,直接使用即可) |
| cs"}   | 将双引号包裹的单词改为大括号包裹(不要进入可视模式,直接使用即可) |

#### 3.NeedTree
```vim
Plug 'scrooloose/nerdtree'

" Nerdtree U C I
nnoremap <silent> <F2> :NERDTreeToggle<ENTER>
let NERDTreeMinimalUI=1
autocmd BufEnter * if tabpagenr('$') == 1 && winnr('$') == 1 && exists('
b:NERDTree') && b:NERDTree.isTabTree() | quit | endif
```


| 快捷键 | 说明                   |
|--------|------------------------|
| F2     | nerdtree开启和关闭切换 |
| U      |                        |
| C      |                        |
| I      |                        |


