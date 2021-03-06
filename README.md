Vim-php-cs-fixer
================

Integrate [php-cs-fixer](https://github.com/fabpot/PHP-CS-Fixer) created by fabpot.

This plugin will execute the `php-cs-fixer` command on the directory or file (depends on which command you call). See options to know how to customize that.

**Options available**:

```viml
" If php-cs-fixer is in $PATH, you don't need to define line below
" let g:php_cs_fixer_path = "~/php-cs-fixer.phar" " define the path to the php-cs-fixer.phar
let g:php_cs_fixer_level = "all"                  " which level ?
let g:php_cs_fixer_config = "default"             " configuration
let g:php_cs_fixer_php_path = "php"               " Path to PHP
" If you want to define specific fixers:
"let g:php_cs_fixer_fixers_list = "linefeed,short_tag,indentation"
let g:php_cs_fixer_enable_default_mapping = 1     " Enable the mapping by default (<leader>pcd)
let g:php_cs_fixer_dry_run = 0                    " Call command with dry-run option
let g:php_cs_fixer_verbose = 0                    " Return the output of command if 1, else an inline information.
```

Default mapping is `<leader>pcd`

If you want to change it:

```viml
nnoremap <silent><leader>pcd :call PhpCsFixerFixDirectory()<CR>
nnoremap <silent><leader>pcf :call PhpCsFixerFixFile()<CR>
```

# Installation

Via **[Vundle](https://github.com/gmarik/vundle)**, add:

```viml
Bundle 'stephpy/vim-php-cs-fixer'
```

Via **[Pathogen](https://github.com/tpope/vim-pathogen)**, do:

```bash
cd ~/.vim/bundle
git clone git@github.com:stephpy/vim-php-cs-fixer.git
```

To see how to install `php-cs-fixer`, look at [php-cs-fixer](https://github.com/fabpot/PHP-CS-Fixer) repository.

If you see any improvement or question, contribute or create an issue

