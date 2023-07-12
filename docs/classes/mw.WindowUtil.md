[UTILITY](../groups/Core.UTILITY.md) / WindowUtil

# WindowUtil <Badge type="tip" text="Class" /> <Score text="WindowUtil" />

窗口设置

使用示例:创建一个名为WindowExample的脚本，放置在对象栏中，打开脚本，将原本内容修改为如下内容，保存并运行游戏，会在控制台打印出屏幕的分辨率大小。
```ts
@Class
export default class WindowExample extends Script {

    protected onStart(): void {
        this.test();
    }

    private async test(): Promise<void> {
        if (!SystemUtil.isClient()) return;
        let viewportSize = WindowUtil.getViewportSize();
        // X=1920 Y=1080
        console.log(`viewportSize ${viewportSize}`);
    }
}
```

## Table of contents

| Accessors |
| :-----|
| **[onDefocused](mw.WindowUtil.md#ondefocused)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <br> 用户游戏窗口失焦，显示器当前游戏窗口切出。调用onDefocused。返回一个多播委托类型。可使用多播委托中的Add、remove、clear、broadcast等函数，当出现窗口聚焦时编写你想要的逻辑。|
| **[onFocused](mw.WindowUtil.md#onfocused)**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\> <br> 用户游戏窗口聚焦，显示器显示当前游戏窗口。调用onFocused，返回一个多播委托类型。可使用多播委托中的Add、remove、clear、broadcast等函数，当出现窗口聚焦时编写你想要的逻辑。|

| Methods |
| :-----|
| **[getViewportSize](mw.WindowUtil.md#getviewportsize)**(): [`Vector2`](mw.Vector2.md) <br> 获取屏幕的分辨率大小（不跟随屏幕缩放变化）。|

## Accessors

### onDefocused <Score text="onDefocused" /> 

• `Static` `get` **onDefocused**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

用户游戏窗口失焦，显示器当前游戏窗口切出。调用onDefocused。返回一个多播委托类型。可使用多播委托中的Add、remove、clear、broadcast等函数，当出现窗口聚焦时编写你想要的逻辑。

#### Returns

[`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

___

### onFocused <Score text="onFocused" /> 

• `Static` `get` **onFocused**(): [`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

用户游戏窗口聚焦，显示器显示当前游戏窗口。调用onFocused，返回一个多播委托类型。可使用多播委托中的Add、remove、clear、broadcast等函数，当出现窗口聚焦时编写你想要的逻辑。

使用示例:创建一个名为"NewScript"的脚本,放置在对象管理器对象子级中,打开脚本,输入以下代码保存,运行游戏,将屏幕切出会显示"游戏窗口失焦，屏幕切出"的log,将屏幕切回，将显示"游戏窗口聚焦，屏幕显现"的log。
```ts
@Class
export default class NewScript extends Script {

     protected onStart(): void {
         WindowUtil.onDefocused.add(()=>{console.log("游戏窗口失焦，屏幕切出")});
         WindowUtil.onFocused.add(()=>{console.log("游戏窗口聚焦，屏幕显现")});
     }
 }
```

#### Returns

[`MulticastDelegate`](mw.MulticastDelegate.md)<() => `void`\>

## Methods

### getViewportSize <Score text="getViewportSize" /> 

• `Static` **getViewportSize**(): [`Vector2`](mw.Vector2.md) <Badge type="tip" text="client" />

获取屏幕的分辨率大小（不跟随屏幕缩放变化）。


使用示例:调用方法
```ts
let viewportSize = WindowUtil.getViewportSize();
console.log(`viewportSize ${viewportSize}`);
// X=1920 Y=1080
```

#### Returns

[`Vector2`](mw.Vector2.md)

返回屏幕的分辨率大小。