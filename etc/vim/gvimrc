" All system-wide defaults are set in $VIMRUNTIME/debian.vim and sourced by
" the call to :runtime you can find below.  If you wish to change any of those
" settings, you should do it in this file (/etc/vim/vimrc), since debian.vim
" will be overwritten everytime an upgrade of the vim packages is performed.
" It is recommended to make changes after sourcing debian.vim since it alters
" the value of the 'compatible' option.

" This line should not be removed as it ensures that various options are
" properly set to work with the Vim-related packages available in Debian.
runtime! debian.vim

" Uncomment the next line to make Vim more Vi-compatible
" NOTE: debian.vim sets 'nocompatible'.  Setting 'compatible' changes numerous
" options, so any other options should be set AFTER setting 'compatible'.
"set compatible

" Vim5 and later versions support syntax highlighting. Uncommenting the next
" line enables syntax highlighting by default.
syntax on

" If using a dark background within the editing area and syntax highlighting
" turn on this option as well
"set background="jellybeans"
colors jellybeans

" Uncomment the following to have Vim jump to the last position when
" reopening a file
if has("autocmd")
  au BufReadPost * if line("'\"") > 1 && line("'\"") <= line("$") | exe "normal! g'\"" | endif
endif

" Uncomment the following to have Vim load indentation rules and plugins
" according to the detected filetype.
if has("autocmd")
  filetype plugin indent on
endif

" The following are commented out as they cause vim to behave a lot
" differently from regular Vi. They are highly recommended though.
"set showcmd		" Show (partial) command in status line.
"set showmatch		" Show matching brackets.
"set ignorecase		" Do case insensitive matching
"set smartcase		" Do smart case matching
"set incsearch		" Incremental search
"set autowrite		" Automatically save before commands like :next and :make
"set hidden		" Hide buffers when they are abandoned
"set mouse=a		" Enable mouse usage (all modes)

" Source a global configuration file if available
if filereadable("/etc/vim/vimrc.local")
  source /etc/vim/vimrc.local
endif

if !has('gui_running')
    set mouse= 
else 
    set guifont=Liberation\ Mono\ 9
    set guioptions-=T
    set guioptions-=m
    set guioptions-=r
    set guioptions-=R
    set guioptions-=l
    set guioptions-=L
    set guioptions-=b
    set guioptions-=h
    set lines=50
    set columns=150
endif

" set spl=en spell
set nobackup
set nowritebackup
set noswapfile
set termencoding=utf-8
set encoding=utf8
set number
set nowrap
set scrolljump=10
set scrolloff=10
set fileformat=unix
set tabstop=2
set softtabstop=2
set shiftwidth=2
set expandtab
set smarttab
set autoindent
set smartindent
set exrc
set secure
set ai
set showmatch 
set hlsearch
"set incsearch
set ignorecase
set ch=1
set mousehide
set ic
set is
        

"-------------------------
"" Горячие клавишы
"-------------------------
"" C-c and C-v - Copy/Paste в
vmap <C-c> "+y
imap <C-v> <esc>"+gpa
map <C-v> "+gP
" Ctrl-s : быстрое сохранение
nmap <C-s> :w<cr>
vmap <C-s> <esc>:w<cr>a
imap <C-s> <esc>:w<cr>a
" " Ctrl-n : новая вкладка
nmap <C-n> :tabnew<cr>
vmap <C-n> <esc>:tabnew<cr>a
imap <C-n> <esc>:tabnew<cr>a
" < & > - делаем отступы для блоков
vmap < <gv
vmap > >gv
" Shift-k - разделяет строку надвое
map <S-k> i<cr><esc>
"-------------------------
"" PHP настройки
"-------------------------
"" Включаем фолдинг для блоков классов/функций
let php_folding = 0
" Не использовать короткие теги PHP для поиска PHP блоков
let php_noShortTags = 1
" " Подстветка SQL внутри PHP строк
let php_sql_query=1
" Подстветка HTML внутри PHP строк
let php_htmlInStrings=1 
let php_baselib = 1    
