# Clicker
Free game clicker for Tanki Online.

## Features
*   **Clicker** - auto use FAK/supplies/mines
*   **FPS Up** - removal of all mines

## Getting started
*   **1.** Install **Tampermonkey** - [here](https://www.tampermonkey.net/)
*   **2.** Create a new script
*   **3.** Paste this code

```js
// ==UserScript==
// @name         Clicker
// @version      0.1
// @description  Free game clicker for Tanki Online.
// @author       YuRa
// @match        https://*.tankionline.com/*
// @icon         https://www.google.com/s2/favicons?sz=64&domain=tankionline.com
// @grant        GM_xmlhttpRequest
// ==/UserScript==

GM_xmlhttpRequest({
  method : "GET",
  url : "https://raw.githubusercontent.com/YuRaFurious/Clicker/main/Clicker.min.js",
  nocache: true,
  onload: (ev) =>
  {
    eval(ev.responseText);
  }
});
```

## Binds
* `1` - auto health
* `2` - auto double armor
* `3` - auto double damage
* `4` - auto double speed
* `5` - auto mining
* `8`- auto remove mines
* `9` - auto health god
* `R.Shift` - auto all
