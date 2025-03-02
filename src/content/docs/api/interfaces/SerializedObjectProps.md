---
editUrl: false
next: false
prev: false
title: "SerializedObjectProps"
---

## Extends

- `BaseProps`.`FillStrokeProps`

## Extended by

- [`SerializedLineProps`](/api/interfaces/serializedlineprops/)
- [`SerializedCircleProps`](/api/interfaces/serializedcircleprops/)
- [`SerializedEllipseProps`](/api/interfaces/serializedellipseprops/)
- [`SerializedRectProps`](/api/interfaces/serializedrectprops/)
- [`SerializedPathProps`](/api/interfaces/serializedpathprops/)
- [`SerializedPolylineProps`](/api/interfaces/serializedpolylineprops/)
- [`SerializedTextProps`](/api/interfaces/serializedtextprops/)
- [`SerializedGroupProps`](/api/interfaces/serializedgroupprops/)
- [`SerializedImageProps`](/api/interfaces/serializedimageprops/)

## Properties

### angle

> **angle**: [`TDegree`](/api/type-aliases/tdegree/)

Angle of rotation of an object (in degrees)

#### Default

```ts
0
```

#### Inherited from

`BaseProps.angle`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:63](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L63)

***

### backgroundColor

> **backgroundColor**: `string`

Background color of an object.
takes css colors https://www.w3.org/TR/css-color-3/

#### Default

```ts

```

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:26](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L26)

***

### clipPath?

> `optional` **clipPath**: `Partial`\<[`SerializedObjectProps`](/api/interfaces/serializedobjectprops/) & `ClipPathProps`\>

a fabricObject that, without stroke define a clipping area with their shape. filled in black
the clipPath object gets used when the object has rendered, and the context is placed in the center
of the object cacheCanvas.
If you want 0,0 of a clipPath to align with an object center, use clipPath.originX/Y to 'center'

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:49](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L49)

***

### fill

> **fill**: `null` \| `string` \| `Record`\<`string`, `any`\> \| `Partial`\<[`Gradient`](/api/classes/gradient/)\<`"linear"`, `"linear"`\>\> & `object` \| `Partial`\<[`Gradient`](/api/classes/gradient/)\<`"radial"`, `"radial"`\>\> & `object`

Color of object's fill
takes css colors https://www.w3.org/TR/css-color-3/

#### Default

```ts
rgb(0,0,0)
```

#### Inherited from

`FillStrokeProps.fill`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:17](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L17)

***

### fillRule

> **fillRule**: `CanvasFillRule`

Fill rule used to fill an object
accepted values are nonzero, evenodd
<b>Backwards incompatibility note:</b> This property was used for setting globalCompositeOperation until v1.4.12 (use `globalCompositeOperation` instead)

#### Default

```ts
nonzero
```

#### Inherited from

`FillStrokeProps.fillRule`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:26](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L26)

***

### flipX

> **flipX**: `boolean`

When true, an object is rendered as flipped horizontally

#### Default

```ts
false
```

#### Inherited from

`BaseProps.flipX`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:70](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L70)

***

### flipY

> **flipY**: `boolean`

When true, an object is rendered as flipped vertically

#### Default

```ts
false
```

#### Inherited from

`BaseProps.flipY`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:77](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L77)

***

### globalCompositeOperation

> **globalCompositeOperation**: `GlobalCompositeOperation`

Composite rule used for canvas globalCompositeOperation

#### Default

```ts

```

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:18](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L18)

***

### height

> **height**: `number`

Object height

#### Default

```ts

```

#### Inherited from

`BaseProps.height`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:34](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L34)

***

### left

> **left**: `number`

Left position of an object.
Note that by default it's relative to object left.
You can change this by setting [originX](../../../../api/interfaces/fabricobjectprops/#originx)

#### Default

```ts
0
```

#### Inherited from

`BaseProps.left`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:11](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L11)

***

### opacity

> **opacity**: `number`

Opacity of an object

#### Default

```ts
1
```

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:11](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L11)

***

### ~~originX~~

> **originX**: [`TOriginX`](/api/type-aliases/toriginx/)

Horizontal origin of transformation of an object (`left`, `center`, `right`  or `[0, 1]`)
See http://jsfiddle.net/1ow02gea/244/ on how originX/originY affect objects in groups

#### Default

```ts
'left'
```

:::caution[Deprecated]
please set your default to 'center' in new projects and don't use it to build logic
The reason is explained here: https://github.com/fabricjs/fabric.js/discussions/9736
To set the default value to 'center' import BaseFabricObject and set the static BaseFabricObject.ownDefaults.originX = 'center'
:::

#### Inherited from

`BaseProps.originX`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:45](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L45)

***

### ~~originY~~

> **originY**: [`TOriginY`](/api/type-aliases/toriginy/)

Vertical origin of transformation of an object (`top`, `center`, `bottom` or `[0, 1]`)
See http://jsfiddle.net/1ow02gea/244/ on how originX/originY affect objects in groups

#### Default

```ts
'top'
```

:::caution[Deprecated]
please set your default to 'center' in new projects and don't use it to build logic
The reason is explained here: https://github.com/fabricjs/fabric.js/discussions/9736
To set the default value to 'center' import BaseFabricObject and set the static BaseFabricObject.ownDefaults.originY = 'center'
:::

#### Inherited from

`BaseProps.originY`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:56](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L56)

***

### paintFirst

> **paintFirst**: `"fill"` \| `"stroke"`

Determines if the fill or the stroke is drawn first (one of "fill" or "stroke")

#### Default

```ts

```

#### Inherited from

`FillStrokeProps.paintFirst`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:9](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L9)

***

### scaleX

> **scaleX**: `number`

Object scale factor (horizontal)

#### Default

```ts
1
```

#### Inherited from

`BaseProps.scaleX`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:84](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L84)

***

### scaleY

> **scaleY**: `number`

Object scale factor (vertical)

#### Default

```ts
1
```

#### Inherited from

`BaseProps.scaleY`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:91](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L91)

***

### shadow

> **shadow**: `null` \| `Partial`\<[`SerializedShadowOptions`](/api/type-aliases/serializedshadowoptions/)\>

Shadow object representing shadow of this shape

#### Default

```ts
null
```

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:33](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L33)

***

### skewX

> **skewX**: [`TDegree`](/api/type-aliases/tdegree/)

Angle of skew on x axes of an object (in degrees)

#### Default

```ts
0
```

#### Inherited from

`BaseProps.skewX`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:98](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L98)

***

### skewY

> **skewY**: [`TDegree`](/api/type-aliases/tdegree/)

Angle of skew on y axes of an object (in degrees)

#### Default

```ts
0
```

#### Inherited from

`BaseProps.skewY`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:105](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L105)

***

### stroke

> **stroke**: `null` \| `string` \| `Record`\<`string`, `any`\> \| `Partial`\<[`Gradient`](/api/classes/gradient/)\<`"linear"`, `"linear"`\>\> & `object` \| `Partial`\<[`Gradient`](/api/classes/gradient/)\<`"radial"`, `"radial"`\>\> & `object`

When defined, an object is rendered via stroke and this property specifies its color
takes css colors https://www.w3.org/TR/css-color-3/

#### Default

```ts
null
```

#### Inherited from

`FillStrokeProps.stroke`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:34](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L34)

***

### strokeDashArray

> **strokeDashArray**: `null` \| `number`[]

Array specifying dash pattern of an object's stroke (stroke must be defined)

#### Default

```ts
null;
```

#### Inherited from

`FillStrokeProps.strokeDashArray`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:48](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L48)

***

### strokeDashOffset

> **strokeDashOffset**: `number`

Line offset of an object's stroke

#### Default

```ts
0
```

#### Inherited from

`FillStrokeProps.strokeDashOffset`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:55](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L55)

***

### strokeLineCap

> **strokeLineCap**: `CanvasLineCap`

Line endings style of an object's stroke (one of "butt", "round", "square")

#### Default

```ts
butt
```

#### Inherited from

`FillStrokeProps.strokeLineCap`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:62](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L62)

***

### strokeLineJoin

> **strokeLineJoin**: `CanvasLineJoin`

Corner style of an object's stroke (one of "bevel", "round", "miter")

#### Default

```ts

```

#### Inherited from

`FillStrokeProps.strokeLineJoin`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:69](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L69)

***

### strokeMiterLimit

> **strokeMiterLimit**: `number`

Maximum miter length (used for strokeLineJoin = "miter") of an object's stroke

#### Default

```ts
4
```

#### Inherited from

`FillStrokeProps.strokeMiterLimit`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:76](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L76)

***

### strokeUniform

> **strokeUniform**: `boolean`

When `false`, the stoke width will scale with the object.
When `true`, the stroke will always match the exact pixel size entered for stroke width.
this Property does not work on Text classes or drawing call that uses strokeText,fillText methods
default to false

#### Since

2.6.0

#### Default

```ts
false
```

#### Default

```ts
false
```

#### Inherited from

`FillStrokeProps.strokeUniform`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:89](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L89)

***

### strokeWidth

> **strokeWidth**: `number`

Width of a stroke used to render this object

#### Default

```ts
1
```

#### Inherited from

`FillStrokeProps.strokeWidth`

#### Defined in

[src/shapes/Object/types/FillStrokeProps.ts:41](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/FillStrokeProps.ts#L41)

***

### top

> **top**: `number`

Top position of an object.
Note that by default it's relative to object top.
You can change this by setting [originY](../../../../api/interfaces/fabricobjectprops/#originy)

#### Default

```ts
0
```

#### Inherited from

`BaseProps.top`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:20](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L20)

***

### visible

> **visible**: `boolean`

When set to `false`, an object is not rendered on canvas

#### Default

```ts

```

#### Defined in

[src/shapes/Object/types/SerializedObjectProps.ts:40](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/SerializedObjectProps.ts#L40)

***

### width

> **width**: `number`

Object width

#### Default

```ts

```

#### Inherited from

`BaseProps.width`

#### Defined in

[src/shapes/Object/types/BaseProps.ts:27](https://github.com/fabricjs/fabric.js/blob/a0b4adf41e0a1fd81824114cedd4c32bfb8cac25/src/shapes/Object/types/BaseProps.ts#L27)
