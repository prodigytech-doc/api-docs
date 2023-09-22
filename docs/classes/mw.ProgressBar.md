[UI](../groups/Core.UI.md) / ProgressBar

# ProgressBar <Badge type="tip" text="Class" /> <Score text="ProgressBar" />

<p class="content-big"> UI进度条 </p>

## Hierarchy

- [`Widget`](mw.Widget.md)

  ↳ **`ProgressBar`**

## Table of contents

### Constructors <Score text="Constructors" /> 


::: details 点击查看继承
### Constructors <Score text="Constructors" /> 
| **new Widget**()  |
| :----- |
:::


### Accessors <Score text="Accessors" /> 
| **[backgroundImageColor](mw.ProgressBar.md#backgroundimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| :-----|
| 设置背景图片颜色|
| **[backgroundImageDrawType](mw.ProgressBar.md#backgroundimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置背景图片绘制类型|
| **[backgroundImageGuid](mw.ProgressBar.md#backgroundimageguid)**(): `string`  |
| 设置进度条背景图片|
| **[backgroundImageMargin](mw.ProgressBar.md#backgroundimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置进度条背景图片边距|
| **[backgroundImageSize](mw.ProgressBar.md#backgroundimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置背景图片大小|
| **[barThickness](mw.ProgressBar.md#barthickness)**(): `number`  |
| 设置进度条厚度|
| **[currentValue](mw.ProgressBar.md#currentvalue)**(): `number`  |
| 设置当前值|
| **[fillImageColor](mw.ProgressBar.md#fillimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置填充图片颜色|
| **[fillImageDrawType](mw.ProgressBar.md#fillimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置填充图片绘制类型|
| **[fillImageGuid](mw.ProgressBar.md#fillimageguid)**(): `string`  |
| 设置进度条图片|
| **[fillImageMargin](mw.ProgressBar.md#fillimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置进度条图片边距|
| **[fillImageSize](mw.ProgressBar.md#fillimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置填充图片大小|
| **[fillType](mw.ProgressBar.md#filltype)**(): [`ProgressBarFillType`](../enums/mw.ProgressBarFillType.md)  |
| 设置进度条填充的方式|
| **[isRoundedToInt](mw.ProgressBar.md#isroundedtoint)**(): `boolean`  |
| 设置当前数值是否取整|
| **[onSliderValueChanged](mw.ProgressBar.md#onslidervaluechanged)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\>  |
| Slider值变化事件|
| **[percent](mw.ProgressBar.md#percent)**(): `number`  |
| 设置当前百分比|
| **[slideMethod](mw.ProgressBar.md#slidemethod)**(): [`SlideMethod`](../enums/mw.SlideMethod.md)  |
| 设置进度条的滑动方式|
| **[sliderButtonPressDelegate](mw.ProgressBar.md#sliderbuttonpressdelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\>  |
| Slider按下事件|
| **[sliderButtonReleaseDelegate](mw.ProgressBar.md#sliderbuttonreleasedelegate)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\>  |
| Slider抬起事件|
| **[sliderMaxValue](mw.ProgressBar.md#slidermaxvalue)**(): `number`  |
| 设置拖动条的最大值|
| **[sliderMinValue](mw.ProgressBar.md#sliderminvalue)**(): `number`  |
| 设置拖动条的最小值|
| **[thumbImageColor](mw.ProgressBar.md#thumbimagecolor)**(): [`LinearColor`](mw.LinearColor.md)  |
| 设置滑块图片颜色|
| **[thumbImageDrawType](mw.ProgressBar.md#thumbimagedrawtype)**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md)  |
| 设置滑块图片绘制类型|
| **[thumbImageGuid](mw.ProgressBar.md#thumbimageguid)**(): `string`  |
| 设置拖动条的样式|
| **[thumbImageMargin](mw.ProgressBar.md#thumbimagemargin)**(): [`Margin`](mw.Margin.md)  |
| 设置拖动条图片边距|
| **[thumbImageSize](mw.ProgressBar.md#thumbimagesize)**(): [`Vector2`](mw.Vector2.md)  |
| 设置滑块图片大小|


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
| **[newObject](mw.ProgressBar.md#newobject)**(`parent?`: [`Canvas`](mw.Canvas.md), `inName?`: `string`): [`ProgressBar`](mw.ProgressBar.md)  |
| :-----|
| 创建 ProgressBar 控件，当parent和inName与已有的对象相同时，旧的对象会被销毁|


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

### backgroundImageColor <Score text="backgroundImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **backgroundImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **backgroundImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取背景图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 背景图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置背景图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 背景颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### backgroundImageDrawType <Score text="backgroundImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **backgroundImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **backgroundImageDrawType**(`InDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取背景图片绘制类型


#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 背景图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置背景图片绘制类型


#### Parameters

| `InDrawType` [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | Brush类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### backgroundImageGuid <Score text="backgroundImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **backgroundImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **backgroundImageGuid**(`inGUID`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取背景图片id


#### Returns

| `string` | 背景图片id |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条背景图片


#### Parameters

| `inGUID` `string` | 图片GUID |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### backgroundImageMargin <Score text="backgroundImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **backgroundImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **backgroundImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取进度条背景图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 进度条背景图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条背景图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 进度条背景图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### backgroundImageSize <Score text="backgroundImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **backgroundImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **backgroundImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取背景图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置背景图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 图片大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### barThickness <Score text="barThickness" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **barThickness**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **barThickness**(`inputBarThickness`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取进度条厚度


#### Returns

| `number` | 厚度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条厚度


#### Parameters

| `inputBarThickness` `number` | 厚度 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### currentValue <Score text="currentValue" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **currentValue**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **currentValue**(`inValue`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取当前值


#### Returns

| `number` | 当前值 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置当前值


#### Parameters

| `inValue` `number` | 当前值 |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### fillImageColor <Score text="fillImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fillImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取填充图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 填充图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置填充图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 设置的颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fillImageDrawType <Score text="fillImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="other" />

</th>
<th style="text-align: left">

• `set` **fillImageDrawType**(`inDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取填充图片绘制类型

只在客户端调用生效\

#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 填充图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置填充图片绘制类型


#### Parameters

| `inDrawType` [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 填充类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fillImageGuid <Score text="fillImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fillImageGuid**(`inGUID`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取填充区图片id


#### Returns

| `string` | 填充区图片id |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条图片


#### Parameters

| `inGUID` `string` | 图片GUID |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### fillImageMargin <Score text="fillImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fillImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取进度条图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 进度条图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 进度条图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fillImageSize <Score text="fillImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fillImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取填充图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置填充图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### fillType <Score text="fillType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **fillType**(): [`ProgressBarFillType`](../enums/mw.ProgressBarFillType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **fillType**(`inType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取进度条填充的方式


#### Returns

| [`ProgressBarFillType`](../enums/mw.ProgressBarFillType.md) | 进度条填充 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条填充的方式


#### Parameters

| `inType` [`ProgressBarFillType`](../enums/mw.ProgressBarFillType.md) | `{ 从左到右,从右到左,从上到下,从下到上 }` |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### isRoundedToInt <Score text="isRoundedToInt" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **isRoundedToInt**(): `boolean` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **isRoundedToInt**(`inToInt`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取当前数值是否取整


#### Returns

| `boolean` | 当前数值是否取整 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置当前数值是否取整


#### Parameters

| `inToInt` `boolean` | 是否取整 |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### onSliderValueChanged <Score text="onSliderValueChanged" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **onSliderValueChanged**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


Slider值变化事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> | 变化事件 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### percent <Score text="percent" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **percent**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **percent**(`inPercent`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取当前百分比


#### Returns

| `number` | 当前百分比 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置当前百分比


#### Parameters

| `inPercent` `number` | 百分比 |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### slideMethod <Score text="slideMethod" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **slideMethod**(): [`SlideMethod`](../enums/mw.SlideMethod.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **slideMethod**(`inSlideMethod`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取进度条的滑动方式


#### Returns

| [`SlideMethod`](../enums/mw.SlideMethod.md) |  |
| :------ | :------ |


</td>
<td style="text-align: left">


设置进度条的滑动方式


#### Parameters

| `inSlideMethod` | [`SlideMethod`](../enums/mw.SlideMethod.md) |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### sliderButtonPressDelegate <Score text="sliderButtonPressDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **sliderButtonPressDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


Slider按下事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> | 按下事件 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### sliderButtonReleaseDelegate <Score text="sliderButtonReleaseDelegate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **sliderButtonReleaseDelegate**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


Slider抬起事件


#### Returns

| [`MulticastDelegate`](mw.MulticastDelegate.md)<(`CurrentValue`: `number`) => `void`\> | 抬起事件 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

___

### sliderMaxValue <Score text="sliderMaxValue" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **sliderMaxValue**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **sliderMaxValue**(`inValue`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取拖动条最大值


#### Returns

| `number` | 拖动条最大值 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置拖动条的最大值


#### Parameters

| `inValue` `number` | 拖动条最大值 |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### sliderMinValue <Score text="sliderMinValue" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **sliderMinValue**(): `number` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **sliderMinValue**(`inValue`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取拖动条最小值


#### Returns

| `number` | 拖动条最小值 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置拖动条的最小值


#### Parameters

| `inValue` `number` | 拖动条最小值 |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### thumbImageColor <Score text="thumbImageColor" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **thumbImageColor**(): [`LinearColor`](mw.LinearColor.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **thumbImageColor**(`inColor`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取滑块图片颜色


#### Returns

| [`LinearColor`](mw.LinearColor.md) | 滑块图片颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置滑块图片颜色


#### Parameters

| `inColor` [`LinearColor`](mw.LinearColor.md) | 设置的颜色，Type.LinearColor类型，数据范围0~1 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### thumbImageDrawType <Score text="thumbImageDrawType" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **thumbImageDrawType**(): [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **thumbImageDrawType**(`inDrawType`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取滑块图片绘制类型


#### Returns

| [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 滑块图片绘制类型 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置滑块图片绘制类型


#### Parameters

| `inDrawType` [`SlateBrushDrawType`](../enums/mw.SlateBrushDrawType.md) | 绘制类型 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### thumbImageGuid <Score text="thumbImageGuid" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **thumbImageGuid**(): `string` <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **thumbImageGuid**(`inGUID`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取填充区图片id


#### Returns

| `string` | 填充区图片id |
| :------ | :------ |


</td>
<td style="text-align: left">


设置拖动条的样式


#### Parameters

| `inGUID` `string` | 拖动条样式GUID |
| :------ | :------ |


void


</td>
</tr></tbody>
</table>

___

### thumbImageMargin <Score text="thumbImageMargin" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **thumbImageMargin**(): [`Margin`](mw.Margin.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **thumbImageMargin**(`inMargin`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取拖动条图片边距


#### Returns

| [`Margin`](mw.Margin.md) | 拖动条图片边距 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置拖动条图片边距


#### Parameters

| `inMargin` [`Margin`](mw.Margin.md) | 拖动条图片边距 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### thumbImageSize <Score text="thumbImageSize" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **thumbImageSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

</th>
<th style="text-align: left">

• `set` **thumbImageSize**(`inSize`): `void` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取滑块图片大小


#### Returns

| [`Vector2`](mw.Vector2.md) | 图片大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置滑块图片大小


#### Parameters

| `inSize` [`Vector2`](mw.Vector2.md) | 滑块图片大小 |
| :------ | :------ |


</td>
</tr></tbody>
</table>



## Methods
___

### newObject <Score text="newObject" /> 

• `Static` **newObject**(`parent?`, `inName?`): [`ProgressBar`](mw.ProgressBar.md) <Badge type="tip" text="client" />

创建 ProgressBar 控件，当parent和inName与已有的对象相同时，旧的对象会被销毁

#### Parameters

| `parent?` [`Canvas`](mw.Canvas.md) | 创建控件的外parent对象 default:null |
| :------ | :------ |
| `inName?` `string` | 创建控件的名称 default:null |

#### Returns

| [`ProgressBar`](mw.ProgressBar.md) | 创建的对象 |
| :------ | :------ |
