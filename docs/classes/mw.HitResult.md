[工具](../groups/工具.工具.md) / HitResult

# HitResult <Badge type="tip" text="Class" /> <Score text="HitResult" />

命中结果，包含关于轨迹的一次命中的信息，例如撞击点和该点的表面法线。

<span style="font-size: 14px;">
使用示例:创建一个名为"HitResultExample"的脚本，放置在对象栏中，打开脚本，输入以下代码保存，并在场景中创建一个模型放置在200, 10, 0的位置，运行游戏，你将在日志中看到射线检测到的HitResult信息数组。代码如下：
</span>

```ts
const result = QueryUtil.lineTrace(new Vector(100), new Vector(1000), true, true);
@Component
export default class HitResultExample extends Script {

    protected onStart(): void {
        if (this.isRunningClient()) {
            // 开始位置
            let startLocation = new Vector(100, 10, 100);
            // 结束位置
            let endLocation = new Vector(1000, 10, 100);
            // 返回的HitResult数组
            const result = QueryUtil.lineTrace(startLocation, endLocation, true, true);
            result.forEach(element => {
                // 通过HitResult访问返回值gameObject的名字
                console.log(`命中GameObject的名字: ${element.gameObject.name}`);
            });
        }
    }
}
```

## Table of contents

### Properties <Score text="Properties" /> 
| **[blockingHit](mw.HitResult.md#blockinghit)**: `boolean`  |
| :-----|
| 是否击中了物体，如果发生了碰撞则为 true, 否则为 false|
| **[boneName](mw.HitResult.md#bonename)**: `string`  |
| 碰撞的骨骼名称|
| **[distance](mw.HitResult.md#distance)**: `number`  |
| 距离，traceStart到location的距离|
| **[gameObject](mw.HitResult.md#gameobject)**: [`GameObject`](mw.GameObject.md)  |
| 命中的GameObject|
| **[impactNormal](mw.HitResult.md#impactnormal)**: [`Vector`](mw.Vector.md)  |
| 世界空间中被扫掠击中的对象（如果有）的法线。例如，如果球体撞击平面，这是一个从平面指向的规范化向量。在与曲面的角或边碰撞的情况下，通常选择“最相反”的法线（与查询方向相反）。|
| **[impactPoint](mw.HitResult.md#impactpoint)**: [`Vector`](mw.Vector.md)  |
| 轨迹形状（长方体、球体、光线等）与受影响对象的实际接触在世界空间中的位置。示例：对于球体跟踪测试，这是球体表面接触其他对象的点。|
| **[normal](mw.HitResult.md#normal)**: [`Vector`](mw.Vector.md)  |
| 世界空间中被扫过的物体的法线。等于线路测试的ImpactNormal。这是为胶囊和球体计算的，否则将与ImpactNormal相同。示例：对于球体轨迹测试，这是指向撞击点处球体中心的归一化矢量。|
| **[position](mw.HitResult.md#position)**: [`Vector`](mw.Vector.md)  |
| 世界空间中的位置，如果发生碰撞，移动的形状将最终抵靠受影响的对象。等于线路测试的冲击点。示例：对于球体跟踪测试，这是当球体接触其他对象时，球体中心所在的点。对于扫掠移动（但不是查询），这可能不等于形状的最终位置，因为命中会稍微向后拉，以防止精度问题与另一个曲面重叠。|
| **[time](mw.HitResult.md#time)**: `number`  |
| 这是沿追踪方向的命中时间，范围介于[0.0到1.0]之间。如未命中，将返回1.0。|
| **[traceEnd](mw.HitResult.md#traceend)**: [`Vector`](mw.Vector.md)  |
| 碰撞检测的终点位置|
| **[traceStart](mw.HitResult.md#tracestart)**: [`Vector`](mw.Vector.md)  |
| 碰撞检测的起点位置|

## Properties

### blockingHit <Score text="blockingHit" /> 

• **blockingHit**: `boolean`

是否击中了物体，如果发生了碰撞则为 true, 否则为 false

___

### boneName <Score text="boneName" /> 

• **boneName**: `string`

碰撞的骨骼名称

___

### distance <Score text="distance" /> 

• **distance**: `number`

距离，traceStart到location的距离

___

### gameObject <Score text="gameObject" /> 

• **gameObject**: [`GameObject`](mw.GameObject.md)

命中的GameObject

___

### impactNormal <Score text="impactNormal" /> 

• **impactNormal**: [`Vector`](mw.Vector.md)

世界空间中被扫掠击中的对象（如果有）的法线。例如，如果球体撞击平面，这是一个从平面指向的规范化向量。在与曲面的角或边碰撞的情况下，通常选择“最相反”的法线（与查询方向相反）。

___

### impactPoint <Score text="impactPoint" /> 

• **impactPoint**: [`Vector`](mw.Vector.md)

轨迹形状（长方体、球体、光线等）与受影响对象的实际接触在世界空间中的位置。示例：对于球体跟踪测试，这是球体表面接触其他对象的点。

___

### normal <Score text="normal" /> 

• **normal**: [`Vector`](mw.Vector.md)

世界空间中被扫过的物体的法线。等于线路测试的ImpactNormal。这是为胶囊和球体计算的，否则将与ImpactNormal相同。示例：对于球体轨迹测试，这是指向撞击点处球体中心的归一化矢量。

___

### position <Score text="position" /> 

• **position**: [`Vector`](mw.Vector.md)

世界空间中的位置，如果发生碰撞，移动的形状将最终抵靠受影响的对象。等于线路测试的冲击点。示例：对于球体跟踪测试，这是当球体接触其他对象时，球体中心所在的点。对于扫掠移动（但不是查询），这可能不等于形状的最终位置，因为命中会稍微向后拉，以防止精度问题与另一个曲面重叠。

___

### time <Score text="time" /> 

• **time**: `number`

这是沿追踪方向的命中时间，范围介于[0.0到1.0]之间。如未命中，将返回1.0。

___

### traceEnd <Score text="traceEnd" /> 

• **traceEnd**: [`Vector`](mw.Vector.md)

碰撞检测的终点位置

___

### traceStart <Score text="traceStart" /> 

• **traceStart**: [`Vector`](mw.Vector.md)

碰撞检测的起点位置
