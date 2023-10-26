[UI](../groups/Core.UI.md) / MaskButton

# MaskButton <Badge type="tip" text="Class" /> <Score text="MaskButton" />

<span class="content-big">

遮罩

</span>

## Hierarchy

- [`Widget`](mw.Widget.md)

  ↳ **`MaskButton`**

## Table of contents

### Accessors <Score text="Accessors" /> 
| **[circleCenter](mw.MaskButton.md#circlecenter)**(): [`Vector2`](mw.Vector2.md)  |
| :-----|
| 设置圆形遮罩的中心旋转点|
| **[circleValue](mw.MaskButton.md#circlevalue)**(): `number`  |
| 设置圆形遮罩的遮挡百分值|
| **[clickMethod](mw.MaskButton.md#clickmethod)**(): [`ButtonClickMethod`](../enums/mw.ButtonClickMethod.md)  |
| 设置点击模式|
| **[clickedDelegate](mw.MaskButton.md#clickeddelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 点击事件|
| **[disableImageColor](mw.MaskButton.md#disableimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置禁用图片颜色|
| **[disableImageDrawType](mw.MaskButton.md#disableimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置禁用图片绘制类型|
| **[disableImageGuid](mw.MaskButton.md#disableimageguid)**(): `string`  |
| 设置不可用图片ID|
| **[disableImageMargin](mw.MaskButton.md#disableimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置禁用图片边距|
| **[disableImageSize](mw.MaskButton.md#disableimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置禁用图片大小|
| **[enableTransition](mw.MaskButton.md#enabletransition)**(`inBoolean`: `boolean`): `void`  |
| 是否套用不同的按下方案|
| **[fanShapedRotated](mw.MaskButton.md#fanshapedrotated)**(): `number`  |
| 设置扇形遮罩的旋转|
| **[fanShapedRotatedCenter](mw.MaskButton.md#fanshapedrotatedcenter)**(): [`Vector2`](mw.Vector2.md)  |
| 设置扇形遮罩的中心旋转点|
| **[fanShapedValue](mw.MaskButton.md#fanshapedvalue)**(): `number`  |
| 设置扇形遮罩的遮罩进度|
| **[focusable](mw.MaskButton.md#focusable)**(): `boolean`  |
| 设置是否获取输入焦点|
| **[hoveredDelegate](mw.MaskButton.md#hovereddelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 悬浮事件|
| **[inverseOpacity](mw.MaskButton.md#inverseopacity)**(): `boolean`  |
| 反转透明度权重|
| **[isTransitionEnable](mw.MaskButton.md#istransitionenable)**(): `boolean`  |
| 按钮是否启用过度模式,按下是否有效果|
| **[maskImageColor](mw.MaskButton.md#maskimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置遮罩图片颜色|
| **[maskImageGuid](mw.MaskButton.md#maskimageguid)**(): `string`  |
| 设置遮罩图片ID|
| **[maskOpacity](mw.MaskButton.md#maskopacity)**(): `number`  |
| 设置遮挡处的底图的透明度|
| **[maskTextureOpacity](mw.MaskButton.md#masktextureopacity)**(): `number`  |
| 设置遮挡处的遮挡图的透明度|
| **[maskType](mw.MaskButton.md#masktype)**(): [`MaskButtonType`](../enums/mw.MaskButtonType.md)  |
| 设置遮罩裁剪类型|
| **[normalImageColor](mw.MaskButton.md#normalimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置普通图片颜色|
| **[normalImageDrawType](mw.MaskButton.md#normalimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置普通图片绘制类型|
| **[normalImageGuid](mw.MaskButton.md#normalimageguid)**(): `string`  |
| 设置普通图片ID|
| **[normalImageMargin](mw.MaskButton.md#normalimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置普通图片边距|
| **[normalImageSize](mw.MaskButton.md#normalimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置图片大小|
| **[pressedDelegate](mw.MaskButton.md#presseddelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 按下事件|
| **[pressedImageColor](mw.MaskButton.md#pressedimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置按压图片颜色|
| **[pressedImageDrawType](mw.MaskButton.md#pressedimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置按压图片绘制类型|
| **[pressedImageGuid](mw.MaskButton.md#pressedimageguid)**(): `string`  |
| 设置按下图片ID|
| **[pressedImageMargin](mw.MaskButton.md#pressedimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置按压图片边距|
| **[pressedImageSize](mw.MaskButton.md#pressedimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置按压图片大小|
| **[pressedMethod](mw.MaskButton.md#pressedmethod)**(): [`ButtonPressMethod`](../enums/mw.ButtonPressMethod.md)  |
| 设置按压模式|
| **[releasedDelegate](mw.MaskButton.md#releaseddelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 释放事件|
| **[roundBoxPercentOffset](mw.MaskButton.md#roundboxpercentoffset)**(): [`Vector2`](mw.Vector2.md)  |
| 设置矩形大小边距偏移|
| **[roundBoxRadius](mw.MaskButton.md#roundboxradius)**(): `number`  |
| 设置角半径|
| **[roundBoxSharpness](mw.MaskButton.md#roundboxsharpness)**(): `number`  |
| 设置的圆角锐化度|
| **[roundBoxUVRatio](mw.MaskButton.md#roundboxuvratio)**(): `number`  |
| 设置圆角调节大小|
| **[touchMethod](mw.MaskButton.md#touchmethod)**(): [`ButtonTouchMethod`](../enums/mw.ButtonTouchMethod.md)  |
| 设置触摸模式|
| **[unHoveredDelegate](mw.MaskButton.md#unhovereddelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 未悬浮事件|
| **[useMaskTextureOpacity](mw.MaskButton.md#usemasktextureopacity)**(): `boolean`  |
| 设置遮罩轮廓是否裁剪底图|


::: details 点击查看继承
### Accessors <Score text="Accessors" /> 
| **[autoSizeEnable](mw.Widget.md#autosizeenable)**(): `boolean`  |
| :-----|
| 设置是否自动设置大小|
| **[cachedGeometry](mw.Widget.md#cachedgeometry)**(): [`Geometry`](mw.Geometry.md)  |
| 获取上一次的GetTickSpaceGeometry|
| **[constraints](mw.Widget.md#constraints)**(): `Readonly`<[`UIConstraintAnchors`](mw.UIConstraintAnchors.md)\>  |
| 设置控件的布局|
| **[desiredSize](mw.Widget.md#desiredsize)**(): [`Vector2`](mw.Vector2.md)  |
| 获取期望大小|
| **[enable](mw.Widget.md#enable)**(): `boolean`  |
| 设置可用性|
| **[guid](mw.Widget.md#guid)**(): `string`  |
| 获取控件GUID|
| **[isHovered](mw.Widget.md#ishovered)**(): `boolean`  |
| 是否是hovered|
| **[name](mw.Widget.md#name)**(): `string`  |
| 设定名字|
| **[paintSpaceGeometry](mw.Widget.md#paintspacegeometry)**(): [`Geometry`](mw.Geometry.md)  |
| 获取最后一次用于渲染Widget的几何信息|
| **[parent](mw.Widget.md#parent)**(): [`Widget`](mw.Widget.md)  |
| 获取父节点|
| **[position](mw.Widget.md#position)**(): `Readonly`<[`Vector2`](mw.Vector2.md)\>  |
| 设置控件的位置|
| **[renderOpacity](mw.Widget.md#renderopacity)**(): `number`  |
| 设置渲染透明度 0 ~ 1|
| **[renderScale](mw.Widget.md#renderscale)**(): [`Vector2`](mw.Vector2.md)  |
| 设置渲染缩放|
| **[renderShear](mw.Widget.md#rendershear)**(): [`Vector2`](mw.Vector2.md)  |
| 设置渲染错切形变|
| **[renderTransformAngle](mw.Widget.md#rendertransformangle)**(): `number`  |
| 设置渲染的角度|
| **[renderTransformPivot](mw.Widget.md#rendertransformpivot)**(): [`Vector2`](mw.Vector2.md)  |
| 设置渲染锚点|
| **[size](mw.Widget.md#size)**(): [`Vector2`](mw.Vector2.md)  |
| 设置控件的大小|
| **[tickSpaceGeometry](mw.Widget.md#tickspacegeometry)**(): [`Geometry`](mw.Geometry.md)  |
| 获取最后一次用于驱动Widget Tick的几何信息|
| **[transform](mw.Widget.md#transform)**(): `Readonly`<[`UITransform`](mw.UITransform.md)\>  |
| 设置控件的大小和位置|
| **[visibility](mw.Widget.md#visibility)**(): [`SlateVisibility`](../enums/mw.SlateVisibility.md)  |
| 设置可见性|
| **[visible](mw.Widget.md#visible)**(): `boolean`  |
| 是否可见|
| **[zOrder](mw.Widget.md#zorder)**(): `number`  |
| 设置zoder|
:::


### Methods <Score text="Methods" /> 
| **[isPressed](mw.MaskButton.md#ispressed)**(): `boolean`  |
| :-----|
| 是否按下|
| **[setDisableImageColorByHex](mw.MaskButton.md#setdisableimagecolorbyhex)**(`inHexString`: `string`): `void`  |
| 设置不可用颜色指定Hex的颜色文本设定颜色 #05050505|
| **[setDisableImageColorDecimal](mw.MaskButton.md#setdisableimagecolordecimal)**(`R`: `number`, `G`: `number`, `B`: `number`, `A`: `number`): `void`  |
| 设置禁用颜色指定R、G、B、A设置颜色 0 ~255|
| **[setMaskImageColorByHex](mw.MaskButton.md#setmaskimagecolorbyhex)**(`inHexString`: `string`): `void`  |
| 设置遮罩图片颜色指定Hex的颜色文本设定颜色 #05050505|
| **[setMaskImageColorDecimal](mw.MaskButton.md#setmaskimagecolordecimal)**(`R`: `number`, `G`: `number`, `B`: `number`, `A`: `number`): `void`  |
| 设置遮罩图片颜色指定R、G、B、A设置颜色 0 ~255|
| **[setNormalImageColorByHex](mw.MaskButton.md#setnormalimagecolorbyhex)**(`inHexString`: `string`): `void`  |
| 设置普通图片颜色指定Hex的颜色文本设定颜色 #05050505|
| **[setNormalImageColorDecimal](mw.MaskButton.md#setnormalimagecolordecimal)**(`R`: `number`, `G`: `number`, `B`: `number`, `A`: `number`): `void`  |
| 设置普通图片颜色 指定R、G、B、A设置颜色 0 ~255|
| **[setPressedImageColorByHex](mw.MaskButton.md#setpressedimagecolorbyhex)**(`inHexString`: `string`): `void`  |
| 设置按压图片颜色指定Hex的颜色文本设定颜色 #05050505|
| **[setPressedImageColorDecimal](mw.MaskButton.md#setpressedimagecolordecimal)**(`R`: `number`, `G`: `number`, `B`: `number`, `A`: `number`): `void`  |
| 设置按压图片颜色指定R、G、B、A设置颜色 0 ~255|
| **[newObject](mw.MaskButton.md#newobject)**(`parent?`: [`Canvas`](mw.Canvas.md), `inName?`: `string`): [`MaskButton`](mw.MaskButton.md)  |
| 创建 Mask 控件 当Outer和InName与已有的对象相同时，旧的对象会被销毁|


::: details 点击查看继承
### Methods <Score text="Methods" /> 
| **[destroyObject](mw.Widget.md#destroyobject)**(): `void`  |
| :-----|
| 立刻移除并销毁 不可以在使用|
| **[equal](mw.Widget.md#equal)**(`that`: [`Widget`](mw.Widget.md)): `boolean`  |
| 判断是不是同一个对象|
| **[invalidateLayoutAndVolatility](mw.Widget.md#invalidatelayoutandvolatility)**(): `void`  |
| 立刻触发重新渲染的和排布计算|
| **[removeObject](mw.Widget.md#removeobject)**(): `void`  |
| 立刻移除并添加到根节点 可以再使用|
:::


## Accessors
___

### circleCenter <Score text="circleCenter" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **circleCenter**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **circleCenter**(`center`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取圆形遮罩的中心旋转点


#### Returns

| [`Vector2`](mw.Vector2.md) | 中心百分点 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置圆形遮罩的中心旋转点


#### Parameters

| `center` [`Vector2`](mw.Vector2.md) | 中心点百分比 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### circleValue <Score text="circleValue" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **circleValue**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **circleValue**(`value`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取圆形遮罩的遮挡百分值


#### Returns

| `number` | 进度值,0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置圆形遮罩的遮挡百分值


#### Parameters

| `value` `number` | 百分进度值,0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### clickMethod <Score text="clickMethod" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **clickMethod**(): [`ButtonClickMethod`](../enums/mw.ButtonClickMethod.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **clickMethod**(`inClickMethod`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取点击模式


#### Returns

| [`ButtonClickMethod`](../enums/mw.ButtonClickMethod.md) | 点击模式 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置点击模式


#### Parameters

| `inClickMethod` [`ButtonClickMethod`](../enums/mw.ButtonClickMethod.md) | 点击模式选择 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### clickedDelegate <Score text="clickedDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **clickedDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


点击事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> | 返回事件的代理 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### disableImageColor <Score text="disableImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **disableImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **disableImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取禁用图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 禁用图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置禁用图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### disableImageDrawType <Score text="disableImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **disableImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **disableImageDrawType**(`inDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取禁用图片绘制类型


#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 禁用图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置禁用图片绘制类型


#### Parameters

| `inDrawType` | [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) |
| :------ | :------ |


禁用图片绘制类型


</td>
</tr></tbody>
</table>

___

### disableImageGuid <Score text="disableImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **disableImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **disableImageGuid**(`inGuid`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取禁用图片ID


#### Returns

| `string` | 禁用图片ID |
| :------ | :------ |


</td>
<td style="text-align: left">


设置不可用图片ID


#### Parameters

| `inGuid` `string` | 图片id |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### disableImageMargin <Score text="disableImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **disableImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **disableImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取禁用图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 禁用图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置禁用图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 禁用图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### disableImageSize <Score text="disableImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **disableImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **disableImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取禁用图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 禁用图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置禁用图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### enableTransition <Score text="enableTransition" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `set` **enableTransition**(`inBoolean`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


是否套用不同的按下方案


#### Parameters

| `inBoolean` `boolean` | 是否套用不同的按下方案 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fanShapedRotated <Score text="fanShapedRotated" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fanShapedRotated**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fanShapedRotated**(`value`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取扇形遮罩的旋转


#### Returns

| `number` | 旋转角度 0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置扇形遮罩的旋转


#### Parameters

| `value` `number` | 旋转角度 0 ~ 1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fanShapedRotatedCenter <Score text="fanShapedRotatedCenter" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fanShapedRotatedCenter**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fanShapedRotatedCenter**(`center`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取扇形遮罩的中心旋转点


#### Returns

| [`Vector2`](mw.Vector2.md) | 旋转中心百分点 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置扇形遮罩的中心旋转点


#### Parameters

| `center` [`Vector2`](mw.Vector2.md) | 中心点百分比 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fanShapedValue <Score text="fanShapedValue" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fanShapedValue**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fanShapedValue**(`value`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取扇形遮罩的遮罩进度


#### Returns

| `number` | 进度值 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置扇形遮罩的遮罩进度


#### Parameters

| `value` `number` | 百分进度值 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### focusable <Score text="focusable" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **focusable**(): `boolean` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **focusable**(`inFocus`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取是否获取输入焦点


#### Returns

| `boolean` | 是否获取输入焦点 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置是否获取输入焦点


#### Parameters

| `inFocus` `boolean` | 是否获取输入焦点 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### hoveredDelegate <Score text="hoveredDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **hoveredDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


悬浮事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> | 返回事件的代理 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### inverseOpacity <Score text="inverseOpacity" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **inverseOpacity**(): `boolean` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **inverseOpacity**(`inverseOpacityWeight`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取反转透明度权重


#### Returns

| `boolean` | 权重 |
| :------ | :------ |


</td>
<td style="text-align: left">


反转透明度权重


#### Parameters

| `inverseOpacityWeight` `boolean` | 权重 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### isTransitionEnable <Score text="isTransitionEnable" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **isTransitionEnable**(): `boolean` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


按钮是否启用过度模式,按下是否有效果


#### Returns

| `boolean` | 按钮是否启用过度模式 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### maskImageColor <Score text="maskImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **maskImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **maskImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取遮罩图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 图片的颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮罩图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### maskImageGuid <Score text="maskImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **maskImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **maskImageGuid**(`InGuid`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取设置遮罩图片ID


#### Returns

| `string` | 遮罩图片ID |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮罩图片ID


#### Parameters

| `InGuid` | `string` |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### maskOpacity <Score text="maskOpacity" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **maskOpacity**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **maskOpacity**(`o`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取遮挡处的底图的透明度


#### Returns

| `number` | 透明度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮挡处的底图的透明度


#### Parameters

| `o` `number` | 透明度 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### maskTextureOpacity <Score text="maskTextureOpacity" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **maskTextureOpacity**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **maskTextureOpacity**(`o`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取遮挡处的遮挡图的透明度


#### Returns

| `number` | 透明度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮挡处的遮挡图的透明度


#### Parameters

| `o` `number` | 透明度 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### maskType <Score text="maskType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **maskType**(): [`MaskButtonType`](../enums/mw.MaskButtonType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **maskType**(`inType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取遮罩裁剪类型


#### Returns

| [`MaskButtonType`](../enums/mw.MaskButtonType.md) | 裁剪类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮罩裁剪类型


#### Parameters

| `inType` [`MaskButtonType`](../enums/mw.MaskButtonType.md) | 裁剪类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### normalImageColor <Score text="normalImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **normalImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **normalImageColor**(`inNormalColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取普通图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 普通图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置普通图片颜色


#### Parameters

| `inNormalColor` [`LinearColor`](mw.LinearColor.md) | 颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### normalImageDrawType <Score text="normalImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **normalImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **normalImageDrawType**(`inDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取普通图片绘制类型


#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 普通图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置普通图片绘制类型


#### Parameters

| `inDrawType` [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### normalImageGuid <Score text="normalImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **normalImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **normalImageGuid**(`inGuid`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取普通图片ID


#### Returns

| `string` | 普通图片ID |
| :------ | :------ |


</td>
<td style="text-align: left">


设置普通图片ID


#### Parameters

| `inGuid` `string` | 图片id |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### normalImageMargin <Score text="normalImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **normalImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **normalImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取普通图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 普通图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置普通图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 普通图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### normalImageSize <Score text="normalImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **normalImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **normalImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 普通图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedDelegate <Score text="pressedDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


按下事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> | 返回事件的代理 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### pressedImageColor <Score text="pressedImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按压图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 按压图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按压图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedImageDrawType <Score text="pressedImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedImageDrawType**(`inDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按压图片绘制类型


#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 按压图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按压图片绘制类型


#### Parameters

| `inDrawType` [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedImageGuid <Score text="pressedImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedImageGuid**(`inGuid`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按下图片ID


#### Returns

| `string` | 按下图片ID |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按下图片ID


#### Parameters

| `inGuid` `string` | 图片id |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedImageMargin <Score text="pressedImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按压图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 按压图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按压图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 按压图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedImageSize <Score text="pressedImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按压图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 按压图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按压图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### pressedMethod <Score text="pressedMethod" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **pressedMethod**(): [`ButtonPressMethod`](../enums/mw.ButtonPressMethod.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **pressedMethod**(`inPressedMethod`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取按压模式


#### Returns

| [`ButtonPressMethod`](../enums/mw.ButtonPressMethod.md) | 按压模式 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置按压模式


#### Parameters

| `inPressedMethod` [`ButtonPressMethod`](../enums/mw.ButtonPressMethod.md) | Press模式选择 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### releasedDelegate <Score text="releasedDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **releasedDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


释放事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> | 返回事件的代理 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### roundBoxPercentOffset <Score text="roundBoxPercentOffset" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **roundBoxPercentOffset**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **roundBoxPercentOffset**(`percent`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取矩形百分比大小边距偏移


#### Returns

| [`Vector2`](mw.Vector2.md) | 矩形大小边距偏移的百分比占据，0~0.5 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置矩形大小边距偏移


#### Parameters

| `percent` [`Vector2`](mw.Vector2.md) | 矩形大小百分比，0~0.5 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### roundBoxRadius <Score text="roundBoxRadius" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **roundBoxRadius**(): `number`

</th>
<th style="text-align: left">

• `set` **roundBoxRadius**(`value`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取设置的角半径

#### Returns

| `number` | 角半径百分比 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置角半径

#### Parameters

| `value` `number` | 角半径百分比 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### roundBoxSharpness <Score text="roundBoxSharpness" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **roundBoxSharpness**(): `number`

</th>
<th style="text-align: left">

• `set` **roundBoxSharpness**(`v`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取设置的圆角锐化度

#### Returns

| `number` | 锐化度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置的圆角锐化度

#### Parameters

| `v` `number` | 锐化度 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### roundBoxUVRatio <Score text="roundBoxUVRatio" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **roundBoxUVRatio**(): `number`

</th>
<th style="text-align: left">

• `set` **roundBoxUVRatio**(`v`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取圆角调节大小

#### Returns

| `number` | 圆角调节大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置圆角调节大小

#### Parameters

| `v` `number` | 圆角调节大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### touchMethod <Score text="touchMethod" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **touchMethod**(): [`ButtonTouchMethod`](../enums/mw.ButtonTouchMethod.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **touchMethod**(`inTouchMethod`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取触摸模式


#### Returns

| [`ButtonTouchMethod`](../enums/mw.ButtonTouchMethod.md) | 触摸模式 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置触摸模式


#### Parameters

| `inTouchMethod` [`ButtonTouchMethod`](../enums/mw.ButtonTouchMethod.md) | Touch模式选择 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### unHoveredDelegate <Score text="unHoveredDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **unHoveredDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


未悬浮事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> | 返回事件的代理 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### useMaskTextureOpacity <Score text="useMaskTextureOpacity" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **useMaskTextureOpacity**(): `boolean` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **useMaskTextureOpacity**(`inUseWeight`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取遮罩轮廓是否裁剪底图


#### Returns

| `boolean` | 权重 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置遮罩轮廓是否裁剪底图


#### Parameters

| `inUseWeight` `boolean` | 是否裁剪 |
| :------ | :------ |


</td>
</tr></tbody>
</table>



## Methods
___

### isPressed <Score text="isPressed" /> 

• **isPressed**(): `boolean` <Badge type="tip" text="client" />

是否按下

#### Returns

| `boolean` | 返回按钮是否按下 |
| :------ | :------ |


___

### setDisableImageColorByHex <Score text="setDisableImageColorByHex" /> 

• **setDisableImageColorByHex**(`inHexString`): `void` <Badge type="tip" text="client" />

设置不可用颜色指定Hex的颜色文本设定颜色 #05050505

#### Parameters

| `inHexString` `string` | 颜色字符串 |
| :------ | :------ |



___

### setDisableImageColorDecimal <Score text="setDisableImageColorDecimal" /> 

• **setDisableImageColorDecimal**(`R`, `G`, `B`, `A`): `void` <Badge type="tip" text="client" />

设置禁用颜色指定R、G、B、A设置颜色 0 ~255

#### Parameters

| `R` `number` | 颜色R值，数据范围0~255 |
| :------ | :------ |
| `G` `number` | 颜色G值，数据范围0~255 |
| `B` `number` | 颜色B值，数据范围0~255 |
| `A` `number` | 颜色透明度，数据范围0~255 |



___

### setMaskImageColorByHex <Score text="setMaskImageColorByHex" /> 

• **setMaskImageColorByHex**(`inHexString`): `void` <Badge type="tip" text="client" />

设置遮罩图片颜色指定Hex的颜色文本设定颜色 #05050505

#### Parameters

| `inHexString` `string` | 颜色字符串 |
| :------ | :------ |



___

### setMaskImageColorDecimal <Score text="setMaskImageColorDecimal" /> 

• **setMaskImageColorDecimal**(`R`, `G`, `B`, `A`): `void` <Badge type="tip" text="client" />

设置遮罩图片颜色指定R、G、B、A设置颜色 0 ~255

#### Parameters

| `R` `number` | 颜色R值，数据范围0~255 |
| :------ | :------ |
| `G` `number` | 颜色G值，数据范围0~255 |
| `B` `number` | 颜色B值，数据范围0~255 |
| `A` `number` | 颜色透明度，数据范围0~255 |



___

### setNormalImageColorByHex <Score text="setNormalImageColorByHex" /> 

• **setNormalImageColorByHex**(`inHexString`): `void` <Badge type="tip" text="client" />

设置普通图片颜色指定Hex的颜色文本设定颜色 #05050505

#### Parameters

| `inHexString` `string` | 颜色字符串 |
| :------ | :------ |



___

### setNormalImageColorDecimal <Score text="setNormalImageColorDecimal" /> 

• **setNormalImageColorDecimal**(`R`, `G`, `B`, `A`): `void` <Badge type="tip" text="client" />

设置普通图片颜色 指定R、G、B、A设置颜色 0 ~255

#### Parameters

| `R` `number` | 颜色R值，数据范围0~255 |
| :------ | :------ |
| `G` `number` | 颜色G值，数据范围0~255 |
| `B` `number` | 颜色B值，数据范围0~255 |
| `A` `number` | 颜色透明度，数据范围0~255 |



___

### setPressedImageColorByHex <Score text="setPressedImageColorByHex" /> 

• **setPressedImageColorByHex**(`inHexString`): `void` <Badge type="tip" text="client" />

设置按压图片颜色指定Hex的颜色文本设定颜色 #05050505

#### Parameters

| `inHexString` `string` | 颜色字符串 |
| :------ | :------ |



___

### setPressedImageColorDecimal <Score text="setPressedImageColorDecimal" /> 

• **setPressedImageColorDecimal**(`R`, `G`, `B`, `A`): `void` <Badge type="tip" text="client" />

设置按压图片颜色指定R、G、B、A设置颜色 0 ~255

#### Parameters

| `R` `number` | 颜色R值，数据范围0~255 |
| :------ | :------ |
| `G` `number` | 颜色G值，数据范围0~255 |
| `B` `number` | 颜色B值，数据范围0~255 |
| `A` `number` | 颜色透明度，数据范围0~255 |



___

### newObject <Score text="newObject" /> 

• `Static` **newObject**(`parent?`, `inName?`): [`MaskButton`](mw.MaskButton.md) <Badge type="tip" text="client" />

创建 Mask 控件 当Outer和InName与已有的对象相同时，旧的对象会被销毁

#### Parameters

| `parent?` [`Canvas`](mw.Canvas.md) | 创建控件的外parent对象 default: null |
| :------ | :------ |
| `inName?` `string` | 创建控件的名称 default:null |

#### Returns

| [`MaskButton`](mw.MaskButton.md) | 返回创建的对象 |
| :------ | :------ |
