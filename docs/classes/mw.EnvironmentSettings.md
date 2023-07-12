[SETTINGS](../groups/Core.SETTINGS.md) / EnvironmentSettings

# EnvironmentSettings <Badge type="tip" text="Class" /> <Score text="EnvironmentSettings" />

环境设置

**`Effect`**


使用示例:创建一个名为"ClassExample"的脚本，放置在对象栏中，打开脚本，输入以下代码保存，运行游戏，你将在服务器Log中看到对应方法调用信息。代码如下：
```ts
@Class
export default class ClassExample extends Script {

    protected onStart(): void {
        this.RoomSettings();
    }

    public RoomSettings(){
        let gra = EnvironmentSettings.getGravity();
        console.log("当前重力大小：" + gra);

        //设置重力模式
        let mode = EnvironmentSettings.getGravityMode();
    }
}
```

## Table of contents

| Methods |
| :-----|
| **[getGravity](mw.EnvironmentSettings.md#getgravity)**(): `number` <br> 获取当前重力大小|
| **[getGravityMode](mw.EnvironmentSettings.md#getgravitymode)**(): [`GravityMode`](../enums/mw.GravityMode.md) <br> 获取当前重力模式|
| **[setGlobalTimeDilation](mw.EnvironmentSettings.md#setglobaltimedilation)**(`time`: `number`): `void` <br> 设置世界整体膨胀时间速度|

## Methods

### getGravity <Score text="getGravity" /> 

• `Static` **getGravity**(): `number` <Badge type="tip" text="client" />

获取当前重力大小


#### Returns

`number`

重力大小。如果返回值为undefined，请检查是否在客户端调用或者是否设置重力大小

___

### getGravityMode <Score text="getGravityMode" /> 

• `Static` **getGravityMode**(): [`GravityMode`](../enums/mw.GravityMode.md) <Badge type="tip" text="client" />

获取当前重力模式


#### Returns

[`GravityMode`](../enums/mw.GravityMode.md)

重力模式。如果返回值为undefined，请检查是否在客户端调用或者是否设置重力模式

___

### setGlobalTimeDilation <Score text="setGlobalTimeDilation" /> 

• `Static` **setGlobalTimeDilation**(`time`): `void` <Badge type="tip" text="other" />

设置世界整体膨胀时间速度

调用端自动广播

::: warning Precautions

世界整体膨胀时间速度默认为1，当膨胀时间速度设置小于1时，世界中所有对象的整体运行时间会开始变慢。膨胀时间速度最小值为0.2。

:::

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `time` | `number` | 膨胀时间速度 |
