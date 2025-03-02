---
editUrl: false
next: false
prev: false
title: "createRotateMatrix"
---

> **createRotateMatrix**(`angle`, `pivotPoint`?): [`TMat2D`](/api/type-aliases/tmat2d/)

Generate a rotation matrix around around a point (x,y), defaulting to (0,0)

A matrix in the form of
[cos(a) -sin(a) -x*cos(a)+y*sin(a)+x]
[sin(a)  cos(a) -x*sin(a)-y*cos(a)+y]
[0       0      1                 ]

## Parameters

• **angle**: [`TRotateMatrixArgs`](/api/namespaces/util/type-aliases/trotatematrixargs/) = `{}`

rotation in degrees

• **pivotPoint?**: `Partial`\<[`XY`](/api/interfaces/xy/)\> = `{}`

pivot point to rotate around

## Returns

[`TMat2D`](/api/type-aliases/tmat2d/)

matrix

## Defined in

[src/util/misc/matrix.ts:169](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/util/misc/matrix.ts#L169)
