# parcel-reporter-web-ext
A parcel plugin for web-ext. This plugin integrates [Parcel](https://parceljs.org/) and [web-ext](https://github.com/mozilla/web-ext).

This plugin is for Parcel v2. The Parcel v1 version is [here](https://github.com/mmktomato/parcel-plugin-web-ext-tool).

If you run `parcel`, `parcel serve` or `parcel watch`, the plugin runs `web-ext run` within it. If you modify your extension code, Parcel detects and rebuilds it, then web-ext detects it and reloads your extension.

# Install
Install via npm. In addtion, you need to install `parcel` and `web-ext` by yourself.

```
$ npm install --save-dev parcel web-ext parcel-reporter-web-ext
```

# Usage
Run `parcel`, `parcel serve` or `parcel watch` in any way you like.

## Config
You can specify web-ext's settings via config files. The plugin reads config files in the following order. The same option is overwritten by the latter one.

* ~/.web-ext-config.js
* package.json
* web-ext-config.js

See [web-ext's official doc](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/#automatic-discovery-of-configuration-files) for details.

# Development
See `DEVELOPMENT.md`.
