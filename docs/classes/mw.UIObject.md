[界面](../groups/界面.界面.md) / UIObject

# UIObject <Badge type="tip" text="Class" /> <Score text="UIObject" />

UI 对象

----------------------------

当你 UIPrefab 制作完成挂载到对象管理器中时，他便成为场景中的一份子，可以使用 GameObject 来查找。

此类中的方法均在客户端调用。

## Hierarchy

- [`GameObject`](mw.GameObject.md)

  ↳ **`UIObject`**

## Table of contents

### Properties <Score text="Properties" /> 


::: details click
### Properties <Score text="Properties" /> 
| **[onDestroyDelegate](mw.GameObject.md#ondestroydelegate)**: [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>   |
| :-----|
| 物体销毁后事件回调|
:::


### Accessors <Score text="Accessors" /> 
| **[uiPath](mw.UIObject.md#uipath)**(): `string` <Badge type="tip" text="client" />  |
| :-----|
| 获取挂载在对象管理器的 UIPrefab 完整路径|
| **[uiScript](mw.UIObject.md#uiscript)**(): [`UIScript`](mw.UIScript.md) <Badge type="tip" text="other" />  |
| 获取在对象管理器中的 UIPrefab 上挂载的脚本|
| **[uiWidgetBase](mw.UIObject.md#uiwidgetbase)**(): [`UserWidget`](mw.UserWidget.md) <Badge type="tip" text="client" />  |
| 获取该对象下所绑定的 UI 根控件|


::: details click
### Accessors <Score text="Accessors" /> 
| **[assetId](mw.GameObject.md#assetid)**(): `string`   |
| :-----|
| 获取当前物体使用资源的GUID|
| **[gameObjectId](mw.GameObject.md#gameobjectid)**(): `string`   |
| 获取物体的唯一标识（唯一标识一个对象的字符串）。|
| **[isReady](mw.GameObject.md#isready)**(): `boolean`   |
| 当前物体状态|
| **[localTransform](mw.GameObject.md#localtransform)**(): [`Transform`](mw.Transform.md)   |
| 当前物体本地变换|
| **[name](mw.GameObject.md#name)**(): `string`   |
| 返回当前物体名称|
| **[netStatus](mw.GameObject.md#netstatus)**(): [`NetStatus`](../enums/mw.NetStatus.md)   |
| 获取当前物体同步状态|
| **[parent](mw.GameObject.md#parent)**(): [`GameObject`](mw.GameObject.md)   |
| 获取当前父物体|
| **[tag](mw.GameObject.md#tag)**(): `string`   |
| 获取当前物体的标签|
| **[worldTransform](mw.GameObject.md#worldtransform)**(): [`Transform`](mw.Transform.md)   |
| 当前物体世界变换|
:::


### Methods <Score text="Methods" /> 


::: details click
### Methods <Score text="Methods" /> 
| **[addComponent](mw.GameObject.md#addcomponent)**<`T`: extends [`Script`](mw.Script.md)<`T`\>\>(`constructor`: (...`args`: `unknown`[]) => `T`: extends [`Script`](mw.Script.md)<`T`\>, `bInReplicates?`: `boolean`): `T`: extends [`Script`](mw.Script.md)<`T`\>  |
| :-----|
| 添加一个脚本组件|
| **[addScriptToObject](mw.GameObject.md#addscripttoobject)**(`script`: [`Script`](mw.Script.md)): `void`   |
| 附加脚本|
| **[asyncReady](mw.GameObject.md#asyncready)**(): `Promise`<[`GameObject`](mw.GameObject.md)\>   |
| 物体准备好后返回|
| **[clone](mw.GameObject.md#clone)**(`gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): [`GameObject`](mw.GameObject.md)   |
| 复制对象|
| **[delScriptFromObject](mw.GameObject.md#delscriptfromobject)**(`script`: [`Script`](mw.Script.md)): `void`   |
| 移除脚本|
| **[destroy](mw.GameObject.md#destroy)**(): `void`   |
| 删除对象|
| **[getBoundingBoxExtent](mw.GameObject.md#getboundingboxextent)**(`nonColliding?`: `boolean`, `includeFromChild?`: `boolean`, `outer?`: [`Vector`](mw.Vector.md)): [`Vector`](mw.Vector.md)   |
| 获取物体包围盒大小|
| **[getBounds](mw.GameObject.md#getbounds)**(`onlyCollidingComponents`: `boolean`, `originOuter`: [`Vector`](mw.Vector.md), `boxExtentOuter`: [`Vector`](mw.Vector.md), `includeFromChild?`: `boolean`): `void`   |
| 获取物体边界|
| **[getChildByGameObjectId](mw.GameObject.md#getchildbygameobjectid)**(`gameObjectId`: `string`): [`GameObject`](mw.GameObject.md)   |
| 根据gameObjectId查找子物体|
| **[getChildByName](mw.GameObject.md#getchildbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)   |
| 根据名称查找子物体|
| **[getChildByPath](mw.GameObject.md#getchildbypath)**(`path`: `string`): [`GameObject`](mw.GameObject.md)   |
| 根据路径查找子物体|
| **[getChildren](mw.GameObject.md#getchildren)**(): [`GameObject`](mw.GameObject.md)[]   |
| 获取子物体|
| **[getChildrenBoundingBoxCenter](mw.GameObject.md#getchildrenboundingboxcenter)**(`outer?`: [`Vector`](mw.Vector.md)): [`Vector`](mw.Vector.md)   |
| 获取所有子对象包围盒中心点(不包含父对象,父对象不可用返回[0,0,0])|
| **[getChildrenByName](mw.GameObject.md#getchildrenbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)[]   |
| 通过名字查找所有的子物体|
| **[getComponent](mw.GameObject.md#getcomponent)**<`T`: extends [`Script`](mw.Script.md)<`T`\>\>(`constructor?`): `T`: extends [`Script`](mw.Script.md)<`T`\> |
| **[getComponentPropertys](mw.GameObject.md#getcomponentpropertys)**<`T`: extends [`Script`](mw.Script.md)<`T`\>\>(`constructor`: (...`args`: `unknown`[]) => `T`: extends [`Script`](mw.Script.md)<`T`\>): `Map`<`string`, `IPropertyOptions`\>  |
| 获取脚本组件属性|
| **[getComponents](mw.GameObject.md#getcomponents)**<`T`: extends [`Script`](mw.Script.md)<`T`\>\>(`constructor?`): `T`: extends [`Script`](mw.Script.md)<`T`\>[] |
| **[getVisibility](mw.GameObject.md#getvisibility)**(): `boolean`   |
| 获取物体是否被显示|
| **[setVisibility](mw.GameObject.md#setvisibility)**(`status`: `boolean`  [`PropertyStatus`](../enums/mw.PropertyStatus.md), `propagateToChildren?`: `boolean`): `void`   |
| 设置物体是否被显示|
| **[asyncFindGameObjectById](mw.GameObject.md#asyncfindgameobjectbyid)**(`gameObjectId`: `string`): `Promise`<[`GameObject`](mw.GameObject.md)\>   |
| 通过gameObjectId异步查找GameObject,默认是10秒,可以通过 `ScriptingSettings.setGlobalAsyncOverTime(1000 * 10);|
| **[asyncGetGameObjectByPath](mw.GameObject.md#asyncgetgameobjectbypath)**(`path`: `string`): `Promise`<[`GameObject`](mw.GameObject.md)\>   |
| 通过路径异步查找物体|
| **[asyncSpawn](mw.GameObject.md#asyncspawn)**<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>(`assetId`: `string`, `gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): `Promise`<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>   |
| 异步构造一个物体，资源不存在会先去下载资源再去创建|
| **[findGameObjectById](mw.GameObject.md#findgameobjectbyid)**(`gameObjectId`: `string`): [`GameObject`](mw.GameObject.md)   |
| 通过gameObjectId查找物体|
| **[findGameObjectByName](mw.GameObject.md#findgameobjectbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)   |
| 通过名字查找物体|
| **[findGameObjectsByName](mw.GameObject.md#findgameobjectsbyname)**(`name`: `string`): [`GameObject`](mw.GameObject.md)[]   |
| 通过名字查找物体|
| **[findGameObjectsByTag](mw.GameObject.md#findgameobjectsbytag)**(`tag`: `string`): [`GameObject`](mw.GameObject.md)[]   |
| 通过自定义标签获取物体|
| **[getGameObjectByPath](mw.GameObject.md#getgameobjectbypath)**(`path`: `string`): [`GameObject`](mw.GameObject.md)   |
| 通过路径查找物体|
| **[spawn](mw.GameObject.md#spawn)**<`T`: extends [`GameObject`](mw.GameObject.md)<`T`\>\>(`assetId`: `string`, `gameObjectInfo?`: [`GameObjectInfo`](../interfaces/mw.GameObjectInfo.md)): `T`: extends [`GameObject`](mw.GameObject.md)<`T`\>   |
| 构造一个物体|
:::


## Properties

## Accessors

___

### uiPath <Score text="uiPath" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **uiPath**(): `string` <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取挂载在对象管理器的 UIPrefab 完整路径


#### Returns

| `string` | UIPrefab 路径 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

<span style="font-size: 14px;">
使用示例:创建一个名为"NewScript"默认脚本脚本，放置在对象栏中，打开脚本，输入以下代码保存，运行游戏。代码如下：
</span>

```ts
@Component
export default class NewScript extends Script {
    protected onStart(): void {
        if(SystemUtil.isClient()){
            // 传入的ID需要修改为你编辑器中挂载在对象管理器中的UIPrefab ID
            let ui = GameObject.findGameObjectById("28504DC8") as UIObject;
            console.log("The complete path of this UIPrefab is:" + ui.uiPath);
        }
    }
}
```
___

### uiScript <Score text="uiScript" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **uiScript**(): [`UIScript`](mw.UIScript.md) <Badge type="tip" text="other" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取在对象管理器中的 UIPrefab 上挂载的脚本


#### Returns

| [`UIScript`](mw.UIScript.md) | UI绑定的脚本 |
| :------ | :------ |

</td>
</tr></tbody>
</table>

<span style="font-size: 14px;">
使用示例:创建一个名为"NewScript"默认脚本脚本，放置在对象栏中，打开脚本，输入以下代码保存，运行游戏。代码如下：
</span>

```ts
@Component
export default class NewScript extends Script {
    protected onStart    (): void {
        if(SystemUtil.isClient()){
            // 传入的ID需要修改为你编辑器中挂载在对象管理器中的UIPrefab ID
            let ui = GameObject.findGameObjectById("28504DC8") as UIObject;
            console.log("The name of the script root control mounted by this UIPrefab:" + ui.uiScript.rootCanvas.name);
        }
    }
}
```
___

### uiWidgetBase <Score text="uiWidgetBase" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `get` **uiWidgetBase**(): [`UserWidget`](mw.UserWidget.md) <Badge type="tip" text="client" />

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取该对象下所绑定的 UI 根控件


#### Returns

</td>
</tr></tbody>
</table>

<span style="font-size: 14px;">
使用示例:创建一个名为"NewScript"默认脚本脚本，放置在对象栏中，打开脚本，输入以下代码保存，运行游戏。代码如下：
</span>

```ts
@Component
export default class NewScript extends Script {
    protected onStart(): void {
        if(SystemUtil.isClient()){
            // 传入的ID需要修改为你编辑器中挂载在对象管理器中的UIPrefab ID
            let ui = GameObject.findGameObjectById("28504DC8") as UIObject;
            console.log("The name of the script canvas mounted by this UIPrefab:" + ui.uiWidgetBase.name);
        }
    }
}
```
| [`UserWidget`](mw.UserWidget.md) | UIPrefab 中的根控件 |
| :------ | :------ |

## Methods
