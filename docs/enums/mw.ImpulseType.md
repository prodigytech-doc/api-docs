[玩法](../groups/玩法.玩法.md) / ImpulseType

# ImpulseType <Badge type="tip" text="Enumeration" /> <Score text="ImpulseType" />

冲量的应用方式

## Table of contents

### Enumeration Members <Score text="Enumeration" /> 
| **[Absolute](mw.ImpulseType.md#absolute)** = ``0``  |
| :----- |
| **[Relative](mw.ImpulseType.md#relative)** = ``1`` |

## Enumeration Members

### Absolute <Score text="Absolute" /> 

• **Absolute** = ``0``

绝对冲量，为冲量功能对象设定一个绝对方向的冲量值，
当被施力对象与冲量功能对象发生碰撞时，将冲量力直接应用到被施力对象上。

___

### Relative <Score text="Relative" /> 

• **Relative** = ``1``

相对冲量，为冲量功能对象设定一个相对方向的冲量值，当被施力对象与冲量功能对象发生碰撞时，
会将被施力对象的矢量值叠加到冲量对象上，计算一个新的冲量值应用到被施力对象上。
