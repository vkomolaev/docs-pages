---
id: "cgfx"
title: "Class: CGfx"
sidebar_label: "CGfx"
hide_title: "true"
---

# Class: CGfx

**`module`** app/canvas/main

**`description`** Main module for canvas lib

**`author`** Vitalii Komolaev

## Hierarchy

* **CGfx**

## Index

### Properties

* [cancelAnimFrame](cgfx.md#static-cancelanimframe)
* [requestAnimFrame](cgfx.md#static-requestanimframe)

### Methods

* [RGB2HSV](cgfx.md#static-rgb2hsv)
* [hsvToRgb](cgfx.md#static-hsvtorgb)
* [patchSylvester](cgfx.md#static-patchsylvester)

## Properties

### `Static` cancelAnimFrame

▪ **cancelAnimFrame**: *any* = (function () {
        return window.cancelAnimationFrame ||
            window['webkitCancelAnimationFrame'] ||
            window['mozCancelAnimationFrame'] ||
            window['oCancelAnimationFrame'] ||
            window['msCancelAnimationFrame'] ||
            function (callback) {
                clearTimeout(callback);
            };
    })().bind(window)

Defined in src/gfx1.ts:133

___

### `Static` requestAnimFrame

▪ **requestAnimFrame**: *any* = (function () {
        return window.requestAnimationFrame ||
            window['webkitRequestAnimationFrame'] ||
            window['mozRequestAnimationFrame'] ||
            window['oRequestAnimationFrame'] ||
            window['msRequestAnimationFrame'] ||
            function (callback) {
                window.setTimeout(callback, 1000 / 60);
            };
    })().bind(window)

Defined in src/gfx1.ts:121

## Methods

### `Static` RGB2HSV

▸ **RGB2HSV**(`r`: number, `g`: number, `b`: number, `hsv`: number[]): *void*

Defined in src/gfx1.ts:151

Converts rgb to hsv

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`r` | number | Red value 0..255 |
`g` | number | Green value 0..255 |
`b` | number | Blue value 0..255 |
`hsv` | number[] | Result of conversion [h, s, v] [0..1, 0..1, 0..255]  |

**Returns:** *void*

___

### `Static` hsvToRgb

▸ **hsvToRgb**(`rgb`: number[], `hsv`: number[]): *void*

Defined in src/gfx1.ts:177

Convert HSV color to RGB color

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`rgb` | number[] | Rgb values [r, g, b] [0..255, 0..255, 0..255] |
`hsv` | number[] | Hsv values [h, s, v] [0..1, 0..1, 0..255]  |

**Returns:** *void*

___

### `Static` patchSylvester

▸ **patchSylvester**(): *void*

Defined in src/gfx1.ts:12

**Returns:** *void*
