---
editUrl: false
next: false
prev: false
title: "sendPointToPlane"
---

> **sendPointToPlane**(`point`, `from`?, `to`?): [`Point`](/api/classes/point/)

## Parameters

• **point**: [`Point`](/api/classes/point/)

• **from?**: [`TMat2D`](/api/type-aliases/tmat2d/) = `iMatrix`

plane matrix containing object. Passing `undefined` is equivalent to passing the identity matrix, which means `point` exists in the canvas coordinate plane.

• **to?**: [`TMat2D`](/api/type-aliases/tmat2d/) = `iMatrix`

destination plane matrix to contain object. Passing `undefined` means `point` should be sent to the canvas coordinate plane.

## Returns

[`Point`](/api/classes/point/)

transformed point

## Defined in

[src/util/misc/planeChange.ts:36](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/util/misc/planeChange.ts#L36)
