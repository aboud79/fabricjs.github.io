---
editUrl: false
next: false
prev: false
title: "saveObjectTransform"
---

> **saveObjectTransform**(`target`): `object`

## Parameters

• **target**: [`BaseFabricObject`](/api/classes/basefabricobject/)\<`Partial`\<`ObjectProps`\>, [`SerializedObjectProps`](/api/interfaces/serializedobjectprops/), [`ObjectEvents`](/api/interfaces/objectevents/)\>

object to read from

## Returns

`object`

Components of transform

### angle

> **angle**: [`TDegree`](/api/type-aliases/tdegree/) = `target.angle`

### flipX

> **flipX**: `boolean` = `target.flipX`

### flipY

> **flipY**: `boolean` = `target.flipY`

### left

> **left**: `number` = `target.left`

### scaleX

> **scaleX**: `number` = `target.scaleX`

### scaleY

> **scaleY**: `number` = `target.scaleY`

### skewX

> **skewX**: `number` = `target.skewX`

### skewY

> **skewY**: `number` = `target.skewY`

### top

> **top**: `number` = `target.top`

## Defined in

[src/util/misc/objectTransforms.ts:86](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/util/misc/objectTransforms.ts#L86)
