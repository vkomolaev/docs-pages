---
id: "cgeom"
title: "Class: CGeom"
sidebar_label: "CGeom"
hide_title: "true"
---

# Class: CGeom

## Hierarchy

* **CGeom**

## Index

### Properties

* [HALF_PI](cgeom.md#static-half_pi)
* [RAD_TO_DEG](cgeom.md#static-rad_to_deg)
* [TWO_PI](cgeom.md#static-two_pi)

### Methods

* [extendBounds](cgeom.md#static-extendbounds)
* [pointInRect](cgeom.md#static-pointinrect)
* [rectInRect](cgeom.md#static-rectinrect)
* [rectRectIntersection](cgeom.md#static-rectrectintersection)

## Properties

### `Static` HALF_PI

▪ **HALF_PI**: *number* = Math.PI / 2

Defined in geometry.ts:28

PI divided by two - 90 degrees

**`default`** Math.PI / 2

___

### `Static` RAD_TO_DEG

▪ **RAD_TO_DEG**: *number* = Math.PI / 2

Defined in geometry.ts:35

Constant for radians to degrees conversion

**`default`** Math.PI / 180

___

### `Static` TWO_PI

▪ **TWO_PI**: *number* = 2 * Math.PI

Defined in geometry.ts:21

Doubled PI - 360 degrees

**`default`** 2 * Math.PI

## Methods

### `Static` extendBounds

▸ **extendBounds**(`b`: [CBounds](cbounds.md), `bounds`: [CBounds](cbounds.md)): *void*

Defined in geometry.ts:96

Extend bounds object

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`b` | [CBounds](cbounds.md) | Bounds to be extended |
`bounds` | [CBounds](cbounds.md) | Bounds  |

**Returns:** *void*

___

### `Static` pointInRect

▸ **pointInRect**(`px`: number, `py`: number, `x`: number, `y`: number, `w`: number, `h`: number): *boolean*

Defined in geometry.ts:47

Check if point inside rect or not

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`px` | number | Point X coordinate |
`py` | number | Point Y coordinate |
`x` | number | Rect X coordinate |
`y` | number | Rect Y coordinate |
`w` | number | Rect width |
`h` | number | Rect height |

**Returns:** *boolean*

True if point inside rect

___

### `Static` rectInRect

▸ **rectInRect**(`outerX`: number, `outerY`: number, `outerW`: number, `outerH`: number, `innerX`: number, `innerY`: number, `innerW`: number, `innerH`: number): *boolean*

Defined in geometry.ts:63

Check if rectangle fully inside other rectangle

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`outerX` | number | Outer rectangle X coordinate |
`outerY` | number | Outer rectangle Y coordinate |
`outerW` | number | Outer rectangle width |
`outerH` | number | Outer rectangle height |
`innerX` | number | Inner rectangle X coordinate |
`innerY` | number | Inner rectangle Y coordinate |
`innerW` | number | Inner rectangle width |
`innerH` | number | Inner rectangle height |

**Returns:** *boolean*

True if inner rectangle fully inside outer rectangle

___

### `Static` rectRectIntersection

▸ **rectRectIntersection**(`outerX`: number, `outerY`: number, `outerW`: number, `outerH`: number, `innerX`: number, `innerY`: number, `innerW`: number, `innerH`: number): *boolean*

Defined in geometry.ts:81

Check if one rectangle intersect another

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`outerX` | number | Outer rectangle X coordinate |
`outerY` | number | Outer rectangle Y coordinate |
`outerW` | number | Outer rectangle width |
`outerH` | number | Outer rectangle height |
`innerX` | number | Inner rectangle X coordinate |
`innerY` | number | Inner rectangle Y coordinate |
`innerW` | number | Inner rectangle width |
`innerH` | number | Inner rectangle height |

**Returns:** *boolean*

True if inner rectangle fully inside outer rectangle
