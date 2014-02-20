# &lt;polymer-localforage&gt;

A Polymer element for Mozilla's [localForage](https://github.com/mozilla/localForage) (async storage via IndexedDB or WebSQL)

> Maintained by [Addy Osmani](https://github.com/addyosmani).

## Demo

> [Check it live](http://addyosmani.github.io/polymer-localforage/smoke.html).

## Installation

Using [Bower](http://bower.io), run:

```shell
bower install polymer-localforage
```

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.1.4/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="src/polymer-localforage.html">
    ```

3. Start using it!

    ```html
    <polymer-localforage><polymer-localforage>
    ```

## Examples

Store a string/object value under a particular key name (`my-app-storage`):

```
<polymer-localforage name="my-app-storage" value="{{value}}"></polymer-localforage>
```

## Setup

In order to run it locally you'll need a basic server setup.

1. Install [NodeJS](http://nodejs.org/download/).
2. Install [GruntJS](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g grunt-cli
    ```

3. Install local dependencies:

    ```sh
    $ npm install
    ```

4. Run a local server and open `http://localhost:8000`.

    ```sh
    $ grunt connect
    ```

## Options

Attribute  | Options                   | Default             | Description
---        | ---                       | ---                 | ---
`name`      | *string*                  | `null`               | The key to the data stored in localforage.
`value`      | *string*                  | `null`               | The data associated with the specified name.
`useRaw`      | *boolean*                  | `false`               | If true, the value is stored and retrieved without JSON processing.
`autoSaveDisabled`      | *boolean*                  | `false`               | If true, auto save is disabled.


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

[MIT License](http://opensource.org/licenses/MIT)