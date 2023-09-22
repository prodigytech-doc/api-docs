[PHYSICS](../groups/Core.PHYSICS.md) / IntegratedMover

# IntegratedMover <Badge type="tip" text="Class" /> <Score text="IntegratedMover" />

<p class="content-big"> 运动器组件 </p>

<p style="font-size: 14px;"> 使用示例:创建一个名为"IMExample1"的脚本,放置在对象栏中,打开脚本,输入以下代码保存,运行游戏,你将在场景中看到两个长方体,分别以开启和不开启平滑运动的方式做重复线性运动.代码如下: </p>

```ts
@Component
export default class IMExample1 extends Script {

    // 声明变量
    Obj1;
    Obj2;
    IM1;
    IM2;

    // 当脚本被实例后，会在第一帧更新前调用此函数
    protected async onStart(): Promise<void> {
      if (SystemUtil.isClient()) {
          // 创建一个长方体
          this.Obj1 = await GameObject.asyncSpawn("197386") as GameObject;
          // 设置起始位置
          this.Obj1.setWorldLocation(new Vector(300.0, -100.0, 300.0));
          // 设置起始缩放
          this.Obj1.setWorldScale(new Vector(0.5, 2.0, 0.5));

          // 创建一个运动器，并将运动器挂载到长方体上
          this.IM1 = await GameObject.asyncSpawn("PhysicsSports") as IntegratedMover;
          this.IM1.attachToGameObject(this.Obj1);

          // 测试启用状态
          console.log("Enable status: " + this.IM1.enable);
          this.IM1.enable = true;
          console.log("New enable status: " + this.IM1.enable);

          // 添加一个线性运动
          this.IM1.linearSpeed = new Vector(0.0, 100.0, 0.0);
          this.IM1.linearRepeat = true;
          this.IM1.linearRepeatTime = 2.0;
          this.IM1.linearRepeatDelay = 0.0;
          this.IM1.linearReturnDelay = 0.0;

          // 用同样的方式创建第二个长方体与第二个运动器
          this.Obj2 = await GameObject.asyncSpawn("197386") as GameObject;
          this.Obj2.setWorldLocation(new Vector(300.0, -100.0, 150.0));
          this.Obj2.setWorldScale(new Vector(0.5, 2.0, 0.5));
          this.IM2 = await GameObject.asyncSpawn("PhysicsSports") as IntegratedMover;
          this.IM2.attachToGameObject(this.Obj2);
          this.IM2.enable = true;

          // 给第二个运动器开启平滑运动
          console.log("Smooth status: " + this.IM2.smooth);
          this.IM2.smooth = true;
          console.log("New smooth status: " + this.IM2.smooth);

          // 添加一个同样的线性运动
          this.IM2.linearSpeed = new Vector(0.0, 100.0, 0.0);
          this.IM2.linearRepeat = true;
          this.IM2.linearRepeatTime = 2.0;
          this.IM2.linearRepeatDelay = 0.0;
          this.IM2.linearReturnDelay = 0.0;
      }
  }
}
```

## Hierarchy

- [`GameObject`](mw.GameObject.md)

  ↳ **`IntegratedMover`**

## Table of contents

### Constructors <Score text="Constructors" /> 


::: details 点击查看继承
### Constructors <Score text="Constructors" /> 
| **new GameObject**()  |
| :----- |
:::


### Properties <Score text="Properties" /> 
| **[onLinearEnable](mw.IntegratedMover.md#onlinearenable)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| :-----|
| 平移运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码|
| **[onLinearReturn](mw.IntegratedMover.md#onlinearreturn)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 平移运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码|
| **[onLinearStart](mw.IntegratedMover.md#onlinearstart)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 平移运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码|
| **[onRotationEnable](mw.IntegratedMover.md#onrotationenable)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 旋转运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码|
| **[onRotationReturn](mw.IntegratedMover.md#onrotationreturn)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 旋转运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码|
| **[onRotationStart](mw.IntegratedMover.md#onrotationstart)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 旋转运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码|
| **[onScaleEnable](mw.IntegratedMover.md#onscaleenable)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 缩放运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码|
| **[onScaleReturn](mw.IntegratedMover.md#onscalereturn)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 缩放运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码|
| **[onScaleStart](mw.IntegratedMover.md#onscalestart)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 缩放运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码|
| **[onSwingEnable](mw.IntegratedMover.md#onswingenable)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| 摆动：延迟启动回调，使用示例详见swingSpeed的getter中的示例代码|


::: details 点击查看继承
### Properties <Score text="Properties" /> 
| **[onDestroyDelegate](mw.GameObject.md#ondestroydelegate)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>  |
| :-----|
| 物体销毁后事件回调|
:::


### Accessors <Score text="Accessors" /> 
| **[enable](mw.IntegratedMover.md#enable)**(): `boolean`  |
| :-----|
| 设置启用状态|
| **[linearDelayStartTime](mw.IntegratedMover.md#lineardelaystarttime)**(): `number`  |
| 设置延时启动平移运动时间，使用示例详见linearSpeed的getter中的示例代码|
| **[linearRepeat](mw.IntegratedMover.md#linearrepeat)**(): `boolean`  |
| 设置平移重复运动状态，使用示例详见linearSpeed的getter中的示例代码|
| **[linearRepeatDelay](mw.IntegratedMover.md#linearrepeatdelay)**(): `number`  |
| 设置平移到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码|
| **[linearRepeatTime](mw.IntegratedMover.md#linearrepeattime)**(): `number`  |
| 设置平移单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码|
| **[linearReturnDelay](mw.IntegratedMover.md#linearreturndelay)**(): `number`  |
| 设置平移返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码|
| **[linearSpeed](mw.IntegratedMover.md#linearspeed)**(): [`Vector`](mw.Vector.md)  |
| 设置平移速度大小，使用示例详见linearSpeed的getter中的示例代码|
| **[motionCoordinate](mw.IntegratedMover.md#motioncoordinate)**(): [`MotionAxis`](../enums/mw.MotionAxis.md)  |
| 设置运动坐标系|
| **[rotationDelayStartTime](mw.IntegratedMover.md#rotationdelaystarttime)**(): `number`  |
| 设置延时启动旋转运动时间，使用示例详见rotationSpeed的getter中的示例代码|
| **[rotationRepeat](mw.IntegratedMover.md#rotationrepeat)**(): `boolean`  |
| 设置旋转重复运动状态，使用示例详见rotationSpeed的getter中的示例代码|
| **[rotationRepeatDelay](mw.IntegratedMover.md#rotationrepeatdelay)**(): `number`  |
| 设置旋转到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码|
| **[rotationRepeatTime](mw.IntegratedMover.md#rotationrepeattime)**(): `number`  |
| 设置旋转单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码|
| **[rotationReturnDelay](mw.IntegratedMover.md#rotationreturndelay)**(): `number`  |
| 设置旋转返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码|
| **[rotationSpeed](mw.IntegratedMover.md#rotationspeed)**(): [`Vector`](mw.Vector.md)  |
| 设置旋转速度大小，使用示例详见rotationSpeed的getter中的示例代码|
| **[scaleDelayStartTime](mw.IntegratedMover.md#scaledelaystarttime)**(): `number`  |
| 设置延时启动缩放运动时间，使用示例详见scaleSpeed的getter中的示例代码|
| **[scaleRepeat](mw.IntegratedMover.md#scalerepeat)**(): `boolean`  |
| 设置缩放重复运动状态，使用示例详见scaleSpeed的getter中的示例代码|
| **[scaleRepeatDelay](mw.IntegratedMover.md#scalerepeatdelay)**(): `number`  |
| 设置缩放到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码|
| **[scaleRepeatTime](mw.IntegratedMover.md#scalerepeattime)**(): `number`  |
| 设置缩放单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码|
| **[scaleReturnDelay](mw.IntegratedMover.md#scalereturndelay)**(): `number`  |
| 设置缩放返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码|
| **[scaleSpeed](mw.IntegratedMover.md#scalespeed)**(): [`Vector`](mw.Vector.md)  |
| 设置缩放速度大小，使用示例详见scaleSpeed的getter中的示例代码|
| **[smooth](mw.IntegratedMover.md#smooth)**(): `boolean`  |
| 设置平滑状态，启用后运动速度会由慢逐渐加快，直到最大值|
| **[swingAngle](mw.IntegratedMover.md#swingangle)**(): `number`  |
| 设置摆动最大角度，使用示例详见swingSpeed的getter中的示例代码|
| **[swingDelayStartTime](mw.IntegratedMover.md#swingdelaystarttime)**(): `number`  |
| 设置延时启动摆动运动时间，使用示例详见swingSpeed的getter中的示例代码|
| **[swingSpeed](mw.IntegratedMover.md#swingspeed)**(): [`Vector`](mw.Vector.md)  |
| 设置摆动运动速度，使用示例详见swingSpeed的getter中的示例代码|


::: details 点击查看继承
### Accessors <Score text="Accessors" /> 
| **[assetId](mw.GameObject.md#assetid)**(): `string`  |
| :-----|
| 获取当前物体使用资源的GUID|
| **[gameObjectId](mw.GameObject.md#gameobjectid)**(): `string`  |
| 获取物体的唯一标识（唯一标识一个对象的字符串）。|
| **[isReady](mw.GameObject.md#isready)**(): `boolean`  |
| 当前物体状态|
| **[localTransform](mw.GameObject.md#localtransform)**(): [`Transform`](mw.Transform.md)  |
| 当前物体本地变换|
| **[name](mw.GameObject.md#name)**(): `string`  |
| 设置物体名称|
| **[netStatus](mw.GameObject.md#netstatus)**(): [`NetStatus`](../enums/mw.NetStatus.md)  |
| 获取当前物体同步状态|
| **[parent](mw.GameObject.md#parent)**(): [`GameObject`](mw.GameObject.md)  |
| 设置父物体|
| **[tag](mw.GameObject.md#tag)**(): `string`  |
| 设置当前物体的标签|
| **[worldTransform](mw.GameObject.md#worldtransform)**(): [`Transform`](mw.Transform.md)  |
| 当前物体世界变换|
:::


### Methods <Score text="Methods" /> 
| **[moverReset](mw.IntegratedMover.md#moverreset)**(`OnReset?`: () => `void`): `void`  |
| :-----|
| 将运动器状态重置，运动对象同时回到初始位置，使用示例详见linearSpeed、rotationSpeed等getter中的示例代码|


::: details 点击查看继承
### Methods <Score text="Methods" /> 
| **[asyncReady](mw.GameObject.md#asyncready)**(): `Promise`<[`GameObject`](mw.GameObject.md)\>  |
| :-----|
| 物体准备好后返回|
| **[clone](mw.GameObject.md#clone)**(`gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): [`GameObject`](mw.GameObject.md)  |
| 复制对象|
| **[destroy](mw.GameObject.md#destroy)**(): `void`  |
| 删除对象|
| **[getBoundingBoxExtent](mw.GameObject.md#getboundingboxextent)**(`nonColliding?`: `boolean`, `includeFromChild?`: `boolean`, `outer?`: [`Vector`](mw.Vector.md)): [`Vector`](mw.Vector.md)  |
| 获取物体包围盒大小|
| **[getBounds](mw.GameObject.md#getbounds)**(`onlyCollidingComponents`: `boolean`, `originOuter`: [`Vector`](mw.Vector.md), `boxExtentOuter`: [`Vector`](mw.Vector.md), `includeFromChild?`: `boolean`): `void`  |
| 获取物体边界|
| **[getChildByGameObjectId](mw.GameObject.md#getchildbygameobjectid)**(`gameObjectId`: `string`): [`GameObject`](mw.GameObject.md)  |
| 根据gameObjectId查找子物体|
| **[getChildByName](mw.GameObject.md#getchildbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)  |
| 根据名称查找子物体|
| **[getChildByPath](mw.GameObject.md#getchildbypath)**(`path`: `string`): [`GameObject`](mw.GameObject.md)  |
| 根据路径查找子物体|
| **[getChildren](mw.GameObject.md#getchildren)**(): [`GameObject`](mw.GameObject.md)[]  |
| 获取子物体|
| **[getChildrenBoundingBoxCenter](mw.GameObject.md#getchildrenboundingboxcenter)**(`outer?`: [`Vector`](mw.Vector.md)): [`Vector`](mw.Vector.md)  |
| 获取所有子对象包围盒中心点(不包含父对象,父对象不可用返回[0,0,0])|
| **[getChildrenByName](mw.GameObject.md#getchildrenbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)[]  |
| 通过名字查找所有的子物体|
| **[getScript](mw.GameObject.md#getscript)**(`id`: `string`): [`Script`](mw.Script.md)  |
| 获得当前物体下的指定脚本|
| **[getScriptByName](mw.GameObject.md#getscriptbyname)**(`name`: `string`): [`Script`](mw.Script.md)  |
| 获得当前物体下的指定脚本|
| **[getScripts](mw.GameObject.md#getscripts)**(): [`Script`](mw.Script.md)[]  |
| 获得当前物体下的所有脚本|
| **[getVisibility](mw.GameObject.md#getvisibility)**(): `boolean`  |
| 获取物体是否被显示|
| **[setVisibility](mw.GameObject.md#setvisibility)**(`status`: `boolean` \, `propagateToChildren?`: `boolean`): `void`  |
| 设置物体是否被显示|
| **[asyncFindGameObjectById](mw.GameObject.md#asyncfindgameobjectbyid)**(`gameObjectId`: `string`): `Promise`<[`GameObject`](mw.GameObject.md)\>  |
| 通过gameObjectId异步查找GameObject,默认是10秒,可以通过 `ScriptingSettings.setGlobalAsyncOverTime(1000 * 10);|
| **[asyncGetGameObjectByPath](mw.GameObject.md#asyncgetgameobjectbypath)**(`path`: `string`): `Promise`<[`GameObject`](mw.GameObject.md)\>  |
| 通过路径异步查找物体|
| **[asyncSpawn](mw.GameObject.md#asyncspawn)**<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>(`assetId`: `string`, `gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): `Promise`<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>  |
| 异步构造一个物体，资源不存在会先去下载资源再去创建|
| **[findGameObjectById](mw.GameObject.md#findgameobjectbyid)**(`gameObjectId`: `string`): [`GameObject`](mw.GameObject.md)  |
| 通过gameObjectId查找物体|
| **[findGameObjectByName](mw.GameObject.md#findgameobjectbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)  |
| 通过名字查找物体|
| **[findGameObjectsByName](mw.GameObject.md#findgameobjectsbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)[]  |
| 通过名字查找物体|
| **[findGameObjectsByTag](mw.GameObject.md#findgameobjectsbytag)**(`tag`: `string`): [`GameObject`](mw.GameObject.md)[]  |
| 通过自定义标签获取物体|
| **[getGameObjectByPath](mw.GameObject.md#getgameobjectbypath)**(`path`: `string`): [`GameObject`](mw.GameObject.md)  |
| 通过路径查找物体|
| **[spawn](mw.GameObject.md#spawn)**<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>(`assetId`: `string`, `gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): `T`: extends [`GameObject`](mw.GameObject.md)<`T`\>  |
| 构造一个物体|
:::


## Properties
___

### onLinearEnable <Score text="onLinearEnable" /> 

• **onLinearEnable**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

平移运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码

___

### onLinearReturn <Score text="onLinearReturn" /> 

• **onLinearReturn**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

平移运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码

___

### onLinearStart <Score text="onLinearStart" /> 

• **onLinearStart**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

平移运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见linearSpeed的getter中的示例代码

___

### onRotationEnable <Score text="onRotationEnable" /> 

• **onRotationEnable**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

旋转运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码

___

### onRotationReturn <Score text="onRotationReturn" /> 

• **onRotationReturn**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

旋转运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码

___

### onRotationStart <Score text="onRotationStart" /> 

• **onRotationStart**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

旋转运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见rotationSpeed的getter中的示例代码

___

### onScaleEnable <Score text="onScaleEnable" /> 

• **onScaleEnable**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

缩放运动首次延迟启动时回调，延迟启动时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码

___

### onScaleReturn <Score text="onScaleReturn" /> 

• **onScaleReturn**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

缩放运动到达终点停顿时回调，到达后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码

___

### onScaleStart <Score text="onScaleStart" /> 

• **onScaleStart**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

缩放运动返回起点停顿时回调，到返程后停顿时间为0时表现不启用，无法获得回调事件，使用示例详见scaleSpeed的getter中的示例代码

___

### onSwingEnable <Score text="onSwingEnable" /> 

• **onSwingEnable**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

摆动：延迟启动回调，使用示例详见swingSpeed的getter中的示例代码

## Accessors
___

### enable <Score text="enable" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **enable**(): `boolean`

</th>
<th style="text-align: left">

• `set` **enable**(`newEnable`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取启用状态

#### Returns

| `boolean` | 启用状态 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置启用状态

#### Parameters

| `newEnable` `boolean` | 启用状态 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### linearDelayStartTime <Score text="linearDelayStartTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearDelayStartTime**(): `number`

</th>
<th style="text-align: left">

• `set` **linearDelayStartTime**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取延时启动平移运行时间，使用示例详见linearSpeed的getter中的示例代码

#### Returns

| `number` | 延时启动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置延时启动平移运动时间，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 延时启动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### linearRepeat <Score text="linearRepeat" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearRepeat**(): `boolean`

</th>
<th style="text-align: left">

• `set` **linearRepeat**(`newRepeat`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平移重复运动状态，使用示例详见linearSpeed的getter中的示例代码

#### Returns

| `boolean` | 平移重复运动状态 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平移重复运动状态，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newRepeat` `boolean` | 平移重复运动状态 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### linearRepeatDelay <Score text="linearRepeatDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearRepeatDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **linearRepeatDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平移到达后停顿时间，使用示例详见linearSpeed的getter中的示例代码

#### Returns

| `number` | 平移到达后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平移到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 平移到达后停顿时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### linearRepeatTime <Score text="linearRepeatTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearRepeatTime**(): `number`

</th>
<th style="text-align: left">

• `set` **linearRepeatTime**(`newTime`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平移单程运动时间，使用示例详见linearSpeed的getter中的示例代码

#### Returns

| `number` | 平移单程运动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平移单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newTime` `number` | 平移单程运动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### linearReturnDelay <Score text="linearReturnDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearReturnDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **linearReturnDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平移返程后停顿时间，使用示例详见linearSpeed的getter中的示例代码

#### Returns

| `number` | 平移返程后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平移返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newDelay` | `number` |
| :------ | :------ |


平移返程后停顿时间


</td>
</tr></tbody>
</table>

___

### linearSpeed <Score text="linearSpeed" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **linearSpeed**(): [`Vector`](mw.Vector.md)

</th>
<th style="text-align: left">

• `set` **linearSpeed**(`newSpeed`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平移速度大小


#### Returns

| [`Vector`](mw.Vector.md) | 平移速度大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平移速度大小，使用示例详见linearSpeed的getter中的示例代码

#### Parameters

| `newSpeed` [`Vector`](mw.Vector.md) | 平移速度大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

<p style="font-size: 14px;"> 使用示例:创建一个名为"IMExample2"的脚本,放置在对象栏中,打开脚本,输入以下代码保存,运行游戏,你将在场景中看到两个长方体,分别演示有无延迟启动的非重复线性运动，以及有无起点终点停顿的重复线性运动.代码如下: </p>

```ts
@Component
export default class IMExample2 extends Script {

    // 声明变量
    Obj1;
    Obj2;
    IM1;
    IM2;

    // 当脚本被实例后，会在第一帧更新前调用此函数
    protected async onStart(): Promise<void> {
        if (SystemUtil.isClient()) {
            // 创建长方体1和长方体2
            this.Obj1 = await GameObject.asyncSpawn( "197386") as GameObject;
            this.Obj2 = await GameObject.asyncSpawn("197386") as GameObject;
            // 设置起始位置
            this.Obj1.setWorldLocation(new Vector(300.0, 0.0, 300.0));
            this.Obj2.setWorldLocation(new Vector(300.0, 0.0, 150.0));
            // 设置起始缩放
            this.Obj1.setWorldScale(new Vector(0.5, 2.0, 0.5));
            this.Obj2.setWorldScale(new Vector(0.5, 2.0, 0.5));

            // 创建运动器1和运动器2，并将运动器挂载到对应长方体上
            this.IM1 = await GameObject.asyncSpawn("PhysicsSports") as IntegratedMover;
            this.IM1.attachToGameObject(this.Obj1);
            this.IM1.enable = true;

            this.IM2 = await GameObject.asyncSpawn("PhysicsSports") as IntegratedMover;
            this.IM2.attachToGameObject(this.Obj2);
            this.IM2.enable = true;

            // 运动器1和2都设置同样的运动速度，运动器2设置延迟五秒启动
            this.IM1.linearSpeed = new Vector(0.0, 100.0, 0.0);
            this.IM1.linearRepeat = false;
            this.IM1.linearDelayStartTime = 0.0;

            this.IM2.linearSpeed = new Vector(0.0, 100.0, 0.0);
            this.IM2.linearRepeat = false;
            this.IM2.linearDelayStartTime = 5.0;
            // 运动器2绑定延迟启动回调
            this.IM2.onLinearEnable.add(() => {
                console.log("IM2 enabled with a delay");
            })

            // 等待十秒后，将长方体1和2归位，重新设置运动器1和2，让它们变成重复运动模式，且运动器2在起点和终点设置两秒延迟
            setTimeout(() => {
                this.IM1.moverReset();
                this.IM2.moverReset();

                this.IM1.linearRepeat = true;
                this.IM1.linearRepeatTime = 2.0;
                this.IM1.linearDelayStartTime = 0.0;
                this.IM1.linearRepeatDelay = 0.0;
                this.IM1.linearReturnDelay = 0.0;

                this.IM2.linearRepeat = true;
                this.IM2.linearRepeatTime = 2.0;
                this.IM2.linearDelayStartTime = 0.0;
                this.IM2.linearRepeatDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onLinearReturn.add(() => {
                    console.log("IM2 paused at end point");
                })
                this.IM2.linearReturnDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onLinearStart.add(() => {
                    console.log("IM2 paused at start point");
                })
            }, 10000);
        }
    }

    //
    // 周期函数 每帧执行
    // 此函数执行需要将this.useUpdate赋值为true
    // @param dt 当前帧与上一帧的延迟 / 秒
    protected onUpdate(dt: number): void {

    }

    // 脚本被销毁时最后一帧执行完调用此函数
    protected onDestroy(): void {

    }
}
```
___

### motionCoordinate <Score text="motionCoordinate" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **motionCoordinate**(): [`MotionAxis`](../enums/mw.MotionAxis.md)

</th>
<th style="text-align: left">

• `set` **motionCoordinate**(`newMotionCoordinate`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取运动坐标系

#### Returns

| [`MotionAxis`](../enums/mw.MotionAxis.md) | 运动坐标系 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置运动坐标系

#### Parameters

| `newMotionCoordinate` [`MotionAxis`](../enums/mw.MotionAxis.md) | 运动坐标系 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationDelayStartTime <Score text="rotationDelayStartTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationDelayStartTime**(): `number`

</th>
<th style="text-align: left">

• `set` **rotationDelayStartTime**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取延时启动旋转运行时间，使用示例详见rotationSpeed的getter中的示例代码

#### Returns

| `number` | 延时启动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置延时启动旋转运动时间，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 延时启动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationRepeat <Score text="rotationRepeat" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationRepeat**(): `boolean`

</th>
<th style="text-align: left">

• `set` **rotationRepeat**(`newRepeat`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取旋转重复运动状态，使用示例详见rotationSpeed的getter中的示例代码

#### Returns

| `boolean` | 旋转重复运动状态 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置旋转重复运动状态，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newRepeat` `boolean` | 旋转重复运动状态 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationRepeatDelay <Score text="rotationRepeatDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationRepeatDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **rotationRepeatDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取旋转到达后停顿时间，使用示例详见rotationSpeed的getter中的示例代码

#### Returns

| `number` | 旋转到达后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置旋转到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 旋转到达后停顿时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationRepeatTime <Score text="rotationRepeatTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationRepeatTime**(): `number`

</th>
<th style="text-align: left">

• `set` **rotationRepeatTime**(`newTime`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取旋转单程运动时间，使用示例详见rotationSpeed的getter中的示例代码

#### Returns

| `number` | 旋转单程运动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置旋转单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newTime` `number` | 旋转单程运动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationReturnDelay <Score text="rotationReturnDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationReturnDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **rotationReturnDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取旋转返程后停顿时间，使用示例详见rotationSpeed的getter中的示例代码

#### Returns

| `number` | 返程后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置旋转返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 返程后停顿时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### rotationSpeed <Score text="rotationSpeed" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **rotationSpeed**(): [`Vector`](mw.Vector.md)

</th>
<th style="text-align: left">

• `set` **rotationSpeed**(`newSpeed`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取旋转速度大小


#### Returns

| [`Vector`](mw.Vector.md) | 旋转速度大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置旋转速度大小，使用示例详见rotationSpeed的getter中的示例代码

#### Parameters

| `newSpeed` [`Vector`](mw.Vector.md) | 旋转速度大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

<p style="font-size: 14px;"> 使用示例:创建一个名为"IMExample3"的脚本,放置在对象栏中,打开脚本,输入以下代码保存,运行游戏,你将在场景中看到两个长方体,分别演示有无延迟启动的非重复旋转，以及有无起点终点停顿的重复旋转.代码如下: </p>

```ts
@Component
export default class IMExample3 extends mw.Script {

    // 声明变量
    Obj1;
    Obj2;
    IM1;
    IM2;

    // 当脚本被实例后，会在第一帧更新前调用此函数
    protected async onStart(): Promise<void> {
        if (Util.SystemUtil.isClient()) {
            // 创建长方体1和长方体2
            this.Obj1 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            this.Obj2 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            // 设置起始位置
            this.Obj1.setWorldLocation(new mw.Vector(300.0, 200.0, 200.0));
            this.Obj2.setWorldLocation(new mw.Vector(300.0, -200.0, 200.0));
            // 设置起始缩放
            this.Obj1.setWorldScale(new mw.Vector(0.5, 2.0, 0.5));
            this.Obj2.setWorldScale(new mw.Vector(0.5, 2.0, 0.5));

            // 创建运动器1和运动器2，并将运动器挂载到对应长方体上
            this.IM1 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM1.attachToGameObject(this.Obj1);
            this.IM1.enable = true;

            this.IM2 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM2.attachToGameObject(this.Obj2);
            this.IM2.enable = true;

            // 运动器1和2都设置同样的旋转速度，运动器2设置延迟五秒启动
            this.IM1.rotationSpeed = new mw.Vector(90.0, 0.0, 0.0);
            this.IM1.rotationRepeat = false;
            this.IM1.rotationDelayStartTime = 0.0;

            this.IM2.rotationSpeed = new mw.Vector(90.0, 0.0, 0.0);
            this.IM2.rotationRepeat = false;
            this.IM2.rotationDelayStartTime = 5.0;
            // 运动器2绑定延迟启动回调
            this.IM2.onRotationEnable.add(() => {
                console.log("IM2 enabled with a delay");
            })

            // 等待十秒后，将长方体1和2归位，重新设置运动器1和2，让它们变成重复运动模式，且运动器2在起点和终点设置两秒延迟
            setTimeout(() => {
                this.IM1.moverReset();
                this.IM2.moverReset();

                this.IM1.rotationRepeat = true;
                this.IM1.rotationRepeatTime = 2.0;
                this.IM1.rotationDelayStartTime = 0.0;
                this.IM1.rotationRepeatDelay = 0.0;
                this.IM1.rotationReturnDelay = 0.0;

                this.IM2.rotationRepeat = true;
                this.IM2.rotationRepeatTime = 2.0;
                this.IM2.rotationDelayStartTime = 0.0;
                this.IM2.rotationRepeatDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onRotationReturn.add(() => {
                    console.log("IM2 paused at end point");
                })
                this.IM2.rotationReturnDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onRotationStart.add(() => {
                    console.log("IM2 paused at start point");
                })
            }, 10000);
        }
    }

    //
    // 周期函数 每帧执行
    // 此函数执行需要将this.useUpdate赋值为true
    // @param dt 当前帧与上一帧的延迟 / 秒
    protected onUpdate(dt: number): void {

    }

    // 脚本被销毁时最后一帧执行完调用此函数
    protected onDestroy(): void {

    }
}
```
___

### scaleDelayStartTime <Score text="scaleDelayStartTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleDelayStartTime**(): `number`

</th>
<th style="text-align: left">

• `set` **scaleDelayStartTime**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取延时启动缩放运行时间，使用示例详见scaleSpeed的getter中的示例代码

#### Returns

| `number` | 延时启动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置延时启动缩放运动时间，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 延时启动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### scaleRepeat <Score text="scaleRepeat" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleRepeat**(): `boolean`

</th>
<th style="text-align: left">

• `set` **scaleRepeat**(`newRepeat`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取缩放重复运动状态，使用示例详见scaleSpeed的getter中的示例代码

#### Returns

| `boolean` | 重复运动状态 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置缩放重复运动状态，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newRepeat` `boolean` | 重复运动状态 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### scaleRepeatDelay <Score text="scaleRepeatDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleRepeatDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **scaleRepeatDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取缩放到达后停顿时间，使用示例详见scaleSpeed的getter中的示例代码

#### Returns

| `number` | 到达后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置缩放到达后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 到达后停顿时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### scaleRepeatTime <Score text="scaleRepeatTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleRepeatTime**(): `number`

</th>
<th style="text-align: left">

• `set` **scaleRepeatTime**(`newTime`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取缩放单程运动时间，使用示例详见scaleSpeed的getter中的示例代码

#### Returns

| `number` | 单程运动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置缩放单程运动时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newTime` `number` | 单程运动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### scaleReturnDelay <Score text="scaleReturnDelay" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleReturnDelay**(): `number`

</th>
<th style="text-align: left">

• `set` **scaleReturnDelay**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取缩放返程后停顿时间，使用示例详见scaleSpeed的getter中的示例代码

#### Returns

| `number` | 返程后停顿时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置缩放返程后停顿时间，该属性需要重复运动状态为true时才会生效，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 返程后停顿时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### scaleSpeed <Score text="scaleSpeed" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **scaleSpeed**(): [`Vector`](mw.Vector.md)

</th>
<th style="text-align: left">

• `set` **scaleSpeed**(`newSpeed`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取缩放速度大小


#### Returns

| [`Vector`](mw.Vector.md) | 缩放速度大小 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置缩放速度大小，使用示例详见scaleSpeed的getter中的示例代码

#### Parameters

| `newSpeed` [`Vector`](mw.Vector.md) | 缩放速度大小 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

<p style="font-size: 14px;"> 使用示例:创建一个名为"IMExample4"的脚本,放置在对象栏中,打开脚本,输入以下代码保存,运行游戏,你将在场景中看到两个正方体,分别演示有无延迟启动的非重复缩放，以及有无起点终点停顿的重复缩放.代码如下: </p>

```ts
@Component
export default class IMExample4 extends mw.Script {

    // 声明变量
    Obj1;
    Obj2;
    IM1;
    IM2;

    // 当脚本被实例后，会在第一帧更新前调用此函数
    protected async onStart(): Promise<void> {
        if (Util.SystemUtil.isClient()) {
            // 创建长方体1和长方体2
            this.Obj1 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            this.Obj2 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            // 设置起始位置
            this.Obj1.setWorldLocation(new mw.Vector(300.0, 200.0, 200.0));
            this.Obj2.setWorldLocation(new mw.Vector(300.0, -200.0, 200.0));
            // 设置起始缩放
            this.Obj1.setWorldScale(new mw.Vector(1.0, 1.0, 1.0));
            this.Obj2.setWorldScale(new mw.Vector(1.0, 1.0, 1.0));

            // 创建运动器1和运动器2，并将运动器挂载到对应长方体上
            this.IM1 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM1.attachToGameObject(this.Obj1);
            this.IM1.enable = true;

            this.IM2 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM2.attachToGameObject(this.Obj2);
            this.IM2.enable = true;

            // 运动器1和2都设置同样的缩放速度，运动器2设置延迟五秒启动
            this.IM1.scaleSpeed = new mw.Vector(-0.1, -0.1, -0.1);
            this.IM1.scaleRepeat = false;
            this.IM1.scaleDelayStartTime = 0.0;

            this.IM2.scaleSpeed = new mw.Vector(-0.1, -0.1, -0.1);
            this.IM2.scaleRepeat = false;
            this.IM2.scaleDelayStartTime = 5.0;
            // 运动器2绑定延迟启动回调
            this.IM2.onScaleEnable.add(() => {
                console.log("IM2 enabled with a delay");
            })

            // 等待十秒后，将长方体1和2归位，重新设置运动器1和2，让它们变成重复运动模式，且运动器2在起点和终点设置两秒延迟
            setTimeout(() => {
                this.IM1.moverReset();
                this.IM2.moverReset();

                this.IM1.scaleRepeat = true;
                this.IM1.scaleRepeatTime = 2.0;
                this.IM1.scaleDelayStartTime = 0.0;
                this.IM1.scaleRepeatDelay = 0.0;
                this.IM1.scaleReturnDelay = 0.0;

                this.IM2.scaleRepeat = true;
                this.IM2.scaleRepeatTime = 2.0;
                this.IM2.scaleDelayStartTime = 0.0;
                this.IM2.scaleRepeatDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onScaleReturn.add(() => {
                    console.log("IM2 paused at end point");
                })
                this.IM2.scaleReturnDelay = 2.0;
                // 运动器2绑定终点停顿回调
                this.IM2.onScaleStart.add(() => {
                    console.log("IM2 paused at start point");
                })
            }, 10000);
        }
    }

    //
    // 周期函数 每帧执行
    // 此函数执行需要将this.useUpdate赋值为true
    // @param dt 当前帧与上一帧的延迟 / 秒
    protected onUpdate(dt: number): void {

    }

    // 脚本被销毁时最后一帧执行完调用此函数
    protected onDestroy(): void {

    }
}
```
___

### smooth <Score text="smooth" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **smooth**(): `boolean`

</th>
<th style="text-align: left">

• `set` **smooth**(`newSmooth`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取平滑状态

#### Returns

| `boolean` | 平滑状态 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置平滑状态，启用后运动速度会由慢逐渐加快，直到最大值

#### Parameters

| `newSmooth` `boolean` | 平滑状态 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### swingAngle <Score text="swingAngle" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **swingAngle**(): `number`

</th>
<th style="text-align: left">

• `set` **swingAngle**(`newAngle`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取摆动最大角度，使用示例详见swingSpeed的getter中的示例代码

#### Returns

| `number` | 摆动最大角度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置摆动最大角度，使用示例详见swingSpeed的getter中的示例代码

#### Parameters

| `newAngle` `number` | 摆动最大角度 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### swingDelayStartTime <Score text="swingDelayStartTime" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **swingDelayStartTime**(): `number`

</th>
<th style="text-align: left">

• `set` **swingDelayStartTime**(`newDelay`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取延时启动摆动运行时间，使用示例详见swingSpeed的getter中的示例代码

#### Returns

| `number` | 延时启动时间 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置延时启动摆动运动时间，使用示例详见swingSpeed的getter中的示例代码

#### Parameters

| `newDelay` `number` | 延时启动时间 |
| :------ | :------ |



</td>
</tr></tbody>
</table>

___

### swingSpeed <Score text="swingSpeed" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **swingSpeed**(): [`Vector`](mw.Vector.md)

</th>
<th style="text-align: left">

• `set` **swingSpeed**(`newSpeed`): `void`

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取摆动运动速度


#### Returns

| [`Vector`](mw.Vector.md) | 摆动运动速度 |
| :------ | :------ |


</td>
<td style="text-align: left">


设置摆动运动速度，使用示例详见swingSpeed的getter中的示例代码

#### Parameters

| `newSpeed` [`Vector`](mw.Vector.md) | 摆动运动速度 |
| :------ | :------ |


</td>
</tr></tbody>
</table>

<p style="font-size: 14px;"> 使用示例:创建一个名为"IMExample5"的脚本,放置在对象栏中,打开脚本,输入以下代码保存,运行游戏,你将在场景中看到两个长方体,分别演示有无延迟启动的单摆运动.代码如下: </p>

```ts
@Component
export default class IMExample5 extends mw.Script {

    // 声明变量
    Obj1;
    Obj2;
    IM1;
    IM2;

    // 当脚本被实例后，会在第一帧更新前调用此函数
    protected async onStart(): Promise<void> {
        if (Util.SystemUtil.isClient()) {
            // 创建长方体1和长方体2
            this.Obj1 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            this.Obj2 = await mw.GameObject.asyncSpawn("197386") as mw.GameObject;
            // 设置起始位置
            this.Obj1.setWorldLocation(new mw.Vector(300.0, 200.0, 200.0));
            this.Obj2.setWorldLocation(new mw.Vector(300.0, -200.0, 200.0));
            // 设置起始缩放
            this.Obj1.setWorldScale(new mw.Vector(0.5, 2.0, 0.5));
            this.Obj2.setWorldScale(new mw.Vector(0.5, 2.0, 0.5));

            // 创建运动器1和运动器2，并将运动器挂载到对应长方体上
            this.IM1 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM1.attachToGameObject(this.Obj1);
            this.IM1.enable = true;

            this.IM2 = await mw.GameObject.asyncSpawn("PhysicsSports") as mw.IntegratedMover;
            this.IM2.attachToGameObject(this.Obj2);
            this.IM2.enable = true;

            // 运动器1和2都设置同样的单摆速度和角度，运动器2设置延迟五秒启动
            this.IM1.swingSpeed = new mw.Vector(1.0, 0.0, 0.0);
            this.IM1.swingAngle = 90.0;
            this.IM1.swingDelayStartTime = 0.0;

            this.IM2.swingSpeed = new mw.Vector(1.0, 0.0, 0.0);
            this.IM2.swingAngle = 90.0;
            this.IM2.swingDelayStartTime = 5.0;
            // 运动器2绑定延迟启动回调
            this.IM2.onSwingEnable.add(() => {
                console.log("IM2 enabled with a delay");
            })
        }
    }

    //
    // 周期函数 每帧执行
    // 此函数执行需要将this.useUpdate赋值为true
    // @param dt 当前帧与上一帧的延迟 / 秒
    protected onUpdate(dt: number): void {

    }

    // 脚本被销毁时最后一帧执行完调用此函数
    protected onDestroy(): void {

    }
}
```


## Methods
___

### moverReset <Score text="moverReset" /> 

• **moverReset**(`OnReset?`): `void` 

将运动器状态重置，运动对象同时回到初始位置，使用示例详见linearSpeed、rotationSpeed等getter中的示例代码

#### Parameters

| `OnReset?` () => `void` | 执行回调 default:null |
| :------ | :------ |

