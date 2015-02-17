# MakeUnity3D

A jquery plugin to easily embed Unity games into your website.

## Usage

* Import this plugin: `<script type="text/javascript" src="../js/jquery.makeunity3d.js"></script>
`
* Add a div element where your game should be embedded: `<div class="unityPlayer" data-options='{"url": "DotUnity3dURL"}'></div>`
* Call `makeUnity3D()` on the div: `$(".unityPlayer").makeUnity3D();` (probably inside `$(document).ready(function()...` or similar).

That's it.

## Options

Options can be added on two levels.

* In the `data-options` attribute of the div.
* As parameter for the `makeUnity3D` function.

Options set as parameter in makeUnity3D will override the default for all divs instantiated with that call. Options set in the attribute will take preference over any other.

The options that can be specified (name [default]: description)

* url [""]: The URL of the .unity3d objects. Required.
* event [null]: When the game should be loaded. Eg. 'mouseover'. If 'null' the game will be loaded when the page is loaded.
* width [800]: Player width.
* height [450]: Player height.
* addMissingHtml [true]: Whether the some html should be placed in case unity is missing.
