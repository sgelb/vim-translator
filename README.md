This is a fork of [blindFS/vim-translator](https://github.com/blindFS/vim-translator) with my little changes.
## Dependencies

* A translation tool. Defaults to  [translate-shell](https://github.com/soimort/translate-shell).
* A player for pronunciation. Defaults to mplayer


## Install

If you don't have a preferred method,
I use [Vundle.vim](https://github.com/VundleVim/Vundle.vim).

``` vim
Plugin 'tengufromsky/vim-translator'
```

## Usage

Create you own mappings like this in your vimrc

``` vim
vmap T <Plug>Translate
vmap R <Plug>TranslateReplace
vmap P <Plug>TranslateSpeak
```

* Assign `g:translate_cmd` to your preferred command for example `trans -b :ru`,
the first target language specified is used in "translate and replace".
```
let g:translate_cmd='trans -b :ru'
```
* Assign `g:translate_player` to your preferred cli stream player.
```
let g:translate_player='mplayer'

```

## Demo

![gif](./demo.gif)

## License

MIT
