AssetManager JS [![Build Status](https://travis-ci.org/ain/assetmanager-js.png?branch=master)](https://travis-ci.org/ain/assetmanager-js)
===============

AssetManager JS is a robust and lightweight JavaScript asset manager for images.
For example it can be used to quickly preload a set of images for your HTML5 project.

## Requirements
None.

## Installation
1. Download a 1KB _dist/Assetmanager.min.js_
2. Include it in your website or application

## Usage
Initialize:
```
var assetManager = new AssetManager();
```
Queue assets:
```
assetManager.add('firstAssetId', 'path/to/asset1.file');
assetManager.add('secondAssetId', 'path/to/asset2.file');
```
Download all assets:
```
// callbackFunction will be called once all assets have been downloaded
assetManager.downloadAll(callbackFunction);
```
Retrieve asset:
```
var firstAssetObject = assetManager.get('firstAssetId');
```

## Example
See _example/index.html_.

## License
AssetManager JS is a robust JavaScript asset manager for images.
Copyright (C) 2013 Ain Tohvri

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.