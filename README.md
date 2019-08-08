# es6dialog
**ES6 Dialog** is a minimal and easy-to-use dialog plugin, which uses the ``<dialog>`` html element. It is written in ECMAScript 9 Object-Oriented Javascript (OOJS).

## How to

1. Download the [es6dialog.js script](#) and include **es6dialog** in your webpage. (Or install via ``npm install es6dialog --save`` or ``yarn add es6dialog --save``)

    ```html
    <script src="es6dialog.min.js"></script>
    ```

    Or:
	```js
	import 'es6dialog';

	// Note: Never import/require the *.min.js files from the npm package.
	```

2. An ES6 Dialog can be triggered as follows ::

    **HTML triggered**
    ```js
    dialog.init() // Adds a listener on all the js-dialog links
    ```
    ```html
    <!-- This js-dialog element targetes the data-dialog value -->
    <a href="#" class="js-dialog" data-dialog="myDialog">Show dialog</a>

    <dialog id="myDialog">
      <h2>My Dialog</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
    </dialog>
    ```
    **JS triggered  (import/require needed):**
    ```js
    import dialog from "dialog"
    dialog.create(myDialog)
    ```
    **JS triggered through Window Object (no import/require needed):**
    ```js
    new window.globalDialog(myDialog).open()
    ```
## [Demo with code examples](https://es6dialog.netlify.com) [![Netlify Status](https://api.netlify.com/api/v1/badges/4580be38-f647-4e58-aa2c-8dbfc2617535/deploy-status)](https://app.netlify.com/sites/es6dialog/deploys)
Can be seen [here](https://es6dialog.netlify.com)

## Advanced configuration
...
