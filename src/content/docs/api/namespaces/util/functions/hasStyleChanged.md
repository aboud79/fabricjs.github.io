---
editUrl: false
next: false
prev: false
title: "hasStyleChanged"
---

> **hasStyleChanged**(`prevStyle`, `thisStyle`, `forTextSpans`): `boolean`

## Parameters

• **prevStyle**: `Partial`\<[`CompleteTextStyleDeclaration`](/api/type-aliases/completetextstyledeclaration/)\>

first style to compare

• **thisStyle**: `Partial`\<[`CompleteTextStyleDeclaration`](/api/type-aliases/completetextstyledeclaration/)\>

second style to compare

• **forTextSpans**: `boolean` = `false`

whether to check overline, underline, and line-through properties

## Returns

`boolean`

true if the style changed

## Defined in

[src/util/misc/textStyles.ts:21](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/util/misc/textStyles.ts#L21)
