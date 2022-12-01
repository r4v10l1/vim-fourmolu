# vim-fourmolu
This plugin provides an interface for [fourmolu](https://github.com/fourmolu/fourmolu) and [ormolu](https://github.com/tweag/ormolu) in Vim

## Usage
The default behavior of this plugin formats a file when saving, but the `FourmoluFmt` command can be used to format source manually. Ranges are supported when using `FourmoluFmt` too. The plugin provides additional commands to enable, disable, or toggle formatting when saving a file using `FourmoluWriteOn`, `FourmoluWriteOff`, and `FourmoluWriteToggle`.

## Installation
Install my fork with [plug](https://github.com/junegunn/vim-plug) adding the following lines to your `.vimrc`:
```VimL
Plug 'r4v10l1/vim-fourmolu'
```
Or the original one by feature-not-a-bug with:
```VimL
Plug 'feature-not-a-bug/vim-fourmolu'
```

## Configuration
If you only want to format content manually setting the following variable to 0 will disable automatic formatting when saving your file:
```VimL
let g:fourmolu_write = 0
```
By default the plugin expects to find a fourmolu executable in your PATH but this can be changed by setting:
```VimL
let g:fourmolu_executable = "ormolu"
```

Any modifications to fourmolu's formatting should be set in fourmolu.yaml
