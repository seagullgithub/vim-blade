# vim-blade #

Vim syntax highlighting for Blade templates (Laravel 4+).

this is forked from jwalton512/vim-blade which was archived by the owner on Feb 22, 2024

note: I haven't updated all syntax tokens. Just those I ran into

updated concerns:

* CompilesConditionals.php [Laravel 12](https://github.com/laravel/framework/blob/12.x/src/Illuminate/View/Compilers/Concerns/CompilesConditionals.php)
* CompilesSessions.php [Laravel 12](https://github.com/laravel/framework/blob/12.x/src/Illuminate/View/Compilers/Concerns/CompilesSessions.php)
* CompilesContexts.php [laravel 12](https://github.com/laravel/framework/blob/12.x/src/Illuminate/View/Compilers/Concerns/CompilesContexts.php)



Installation
------------

Using vim-plug
[vim-plug](https://github.com/junegunn/vim-plug).

    Plug 'seagullgithub/vim-blade'

Using pathogen 
[pathogen.vim](https://github.com/tpope/vim-pathogen).  

    cd ~/.vim/bundle
    git clone git://github.com/seagullgithub/vim-blade.git

Configuration
-------------

Because Blade allows you to define your own directives, you can let the plugin
know about them through some variables. Examples:

```vim
" Define some single Blade directives. This variable is used for highlighting only.
let g:blade_custom_directives = ['datetime', 'javascript']

" Define pairs of Blade directives. This variable is used for highlighting and indentation.
let g:blade_custom_directives_pairs = {
      \   'markdown': 'endmarkdown',
      \   'cache': 'endcache',
      \ }
```

Contributing
------------

Pull requests are greatly appreciated. Please be certain to include a test where applicable (`test.blade.php`). You may test locally by using `vim -u vimrc`.
