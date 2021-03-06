<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## Omnibar

The omnibar provides kinds of functions that need user input, for example,

-   Open url(from both bookmarks and history) with `t`
-   Open bookmarks with `b`
-   Open search engines with `og` / `ow` ...
-   Open commands with `:`

Key bindings in Omnibar:

-   `Enter` to open selected item and close omnibar.
-   `Ctrl-Enter` to open selected item, but keep omnibar open for more items to be opened.
-   `Shift-Enter` to open selected item in current tab and close omnibar.
    If you'd like to open in current tab by default, please use go.
-   Tab to forward cycle through the candidates.
-   `Shift-Tab` to backward cycle through the candidates.
-   `Ctrl-`. to show results of next page
-   `Ctrl-`, to show results of previous page
-   `Ctrl-c` to copy all listed items
-   In omnibar opened with `t:`

`Ctrl - d` to delete from bookmark or history

-   In omnibar opened with `b:`

`Ctrl - Shift - <any letter>` to create vim-like mark

cmap could be used for Omnibar to change mappings, for example:

```js
cmap('<Ctrl-n>', '<Tab>');
cmap('<Ctrl-p>', '<Shift-Tab>');
```

* * *

**Parameters**

-   `mode` **[Object][1]** 

Returns **[Omnibar][2]** Omnibar instance

### listURLs

List URLs like {url: "[https://github.com"][3], title: "github.com"} beneath omnibar

**Parameters**

-   `items` **[Array][4]** Array of url items with title.
-   `showFolder` **[boolean][5]** True to show a item as folder if it has no property url.

**Examples**

```javascript
Omnibar.listURLs ([{url: 'http://google.com', title: 'Google'}], false)
```

Returns **[undefined][6]** 

### onOpen

List commands when OmniBar opens

Returns **[undefined][6]** 

### onEnter

Execute command after pressing the return key.

Displays any output if the command.

Returns **[boolean][5]** 

## StatusBar

The status bar displays the status of Surfingkeys current mode: Normal, visual, etc.

**Parameters**

-   `ui` **[Object][1]** 

Returns **[StatusBar][7]** StatusBar instance

### open

Opens the status bar

Returns **[undefined][6]** 

[1]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[2]: #omnibar

[3]: https://github.com"

[4]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/undefined

[7]: #statusbar
