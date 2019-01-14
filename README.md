<img src="./img/logo.png" alt="json logo" width="250" />

# Placeholder IMAGE Snippets for EMMET-Vim

Fastly image placeholder service snippet (From [placeholder.com](placeholder.com))

![presentation of snippet](./img/snippets-ph.gif)

```
i:ph
```
---

## REQUIREMENTS

* A Plugin manager
* [EMMET-VIM](https://vimawesome.com/plugin/emmet-vim)
* [WEBAPI-VIM](https://github.com/mattn/webapi-vim)


## SOURCES & HELPFUL DOCS

* https://docs.emmet.io/cheat-sheet/
* https://docs.emmet.io/customization/snippets/
* https://github.com/emmetio/emmet/blob/master/lib/snippets.json
* https://github.com/mattn/webapi-vim
* https://placeholder.com/

---

### HOW TO INSTALL

1) Install [EMMET-VIM](https://vimawesome.com/plugin/emmet-vim) with your plugin manager
2) Install [WEBAPI-VIM](https://github.com/mattn/webapi-vim) with your plugin manager
3) Add the config line to your ***.vimrc*** by taking care of <style color="red">***change the path***</style>

```
let g:user_emmet_settings = webapi#json#decode(join(readfile(expand('CHANGE_THE_PATH_HERE')), "\n    "))
```

> In Example
```
let g:user_emmet_settings = webapi#json#decode(join(readfile(expand('~/github/simplon/snippets/emmet/imagePlaceHolder/json/snippets-placeholder.json')), "\n    "))
```

4) Source ***(:so %)*** your .vimrc (or reboot the terminal)
5) Enjoy with the ``` i:ph``` command

### HOW TO USE

When you do the ```i:ph``` the cursor is placed end of url, you just need add a size like ```150`` or ```150x150```
if you want more go to [PlaceHolder Website](https://placeholder.com/)

> In Example
```
<img src="https://via.placeholder.com/150x150" alt="">
```


---

## THANKS TO

* mattn for "emmet-vim" & "webapi-vim"
* djefry for the logo


## LICENCE

MIT
