[玩法](../groups/玩法.玩法.md) / CameraSwitchBlendFunction

# CameraSwitchBlendFunction <Badge type="tip" text="Enumeration" /> <Score text="CameraSwitchBlendFunction" />

切换摄像机时运用的混合函数

## Table of contents

### Enumeration Members <Score text="Enumeration" /> 
| **[Cubic](mw.CameraSwitchBlendFunction.md#cubic)** = ``1``  |
| :----- |
| **[EaseIn](mw.CameraSwitchBlendFunction.md#easein)** = ``2`` |
| **[EaseInOut](mw.CameraSwitchBlendFunction.md#easeinout)** = ``4`` |
| **[EaseOut](mw.CameraSwitchBlendFunction.md#easeout)** = ``3`` |
| **[Linear](mw.CameraSwitchBlendFunction.md#linear)** = ``0`` |

## Enumeration Members

### Cubic <Score text="Cubic" /> 

• **Cubic** = ``1``

有轻微的缓入和缓出,但缓和程度无法调整

___

### EaseIn <Score text="EaseIn" /> 

• **EaseIn** = ``2``

立即加速,但平稳减速到目标,由blendExp参数控制的缓和程度

___

### EaseInOut <Score text="EaseInOut" /> 

• **EaseInOut** = ``4``

相机平稳地加速和减速,由 BlendExp 控制缓和程度

___

### EaseOut <Score text="EaseOut" /> 

• **EaseOut** = ``3``

相机平稳加速,但不会减速到目标,由blendExp参数控制的缓和程度

___

### Linear <Score text="Linear" /> 

• **Linear** = ``0``

简单的线性插值
