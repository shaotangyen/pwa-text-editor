[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# pwa-text-editor

This is a PWA powered text editor that runs in the browser. It features a number of data persistence techniques that serve as redundancy in case one of the options is not supported by the browser. The application will also function offline.

The text editor uses the `idb` package which is a lightweight around the IndexedDB API. It features methods that are useful for storing and retrieving data used by companies like Google and Mozilla.

The deployed heroku site is linked [here](https://polar-castle-95331.herokuapp.com/).

## Table of Contents
1. [Setup](#setup)
2. [Design](#design)
3. [Links](#links)
4. [License](#license)

<a name="setup"></a>

## Setup

You can simply visit the deployed site [here](https://polar-castle-95331.herokuapp.com/) without setting it up.

If you want to download the code from github and set it up in your local machine, you can use `npm install && npm run start` to start the local server.

<a name="design"></a>

## Design

* The app is installed as a PWA (Progressive Web Application) application
* The app uses Localstorage to temporary store typed content and offline content, and store it to IndexedDB when mouse is out of focus of the app
* The app is bundled with webpack
* The app creates a service worker with workbox that caches static assets 
* The app uses babel in order to use async / await
* The app generated `manifest.json` using the `WebpackPwaManifest` plug-in

<a name="links"></a>

## Demo and Links

The deployed site is [here](https://polar-castle-95331.herokuapp.com/).

Or go to the Github page for the full code: [Link](https://github.com/shaotangyen/pwa-text-editor).

<a name="license"></a>

## License

Copyright 2021 Shao Yen

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
