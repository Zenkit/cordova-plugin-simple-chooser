# Simple Chooser

## Overview

A simple file chooser plugin for Cordova.

Based on [`cordova-plugin-simple-chooser`](https://github.com/cyph/cordova-plugin-chooser),
but without using `Promise` and without loading the file `data` (can be done with `cordova-plugin-file`).

Install with Cordova CLI:

```sh
cordova plugin add https://github.com/zenkit/cordova-plugin-simple-chooser#v2.0.0
```

Supported Platforms:

- Android

- iOS

## API

### chooser.chooseFile(successCallback, errorCallback, [accept])

#### successCallback

Type: `function`

The success callback will be called with the information of the picked file

```js
    {
        uri: 'string',
        name: 'string',
        mediaType: 'string',
    }
```

#### errorCallback

Type: `function`

Will be called if an error occurs or the user cancels the picker

#### accept

Type: `string`

Optional MIME type filter (e.g. 'image/gif,video/\*').
