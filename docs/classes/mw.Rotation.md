[TYPE](../groups/TYPE.TYPE.md) / Rotation

# Rotation <Badge type="tip" text="Class" /> <Score text="Rotation" />

由分量 (x,y,z) 组成的三维空间中的旋转量。
Rotation 是三个欧拉角Picth、Yaw、Roll的封装类，

::: warning Precautions

所有旋转值均以度为单位存储

:::

## Table of contents

### Properties <Score text="Properties" /> 
| **[x](mw.Rotation.md#x)**: `number`  |
| :-----|
| 旋转的 x 分量|
| **[y](mw.Rotation.md#y)**: `number`  |
| 旋转的 y 分量|
| **[z](mw.Rotation.md#z)**: `number`  |
| 旋转的 z 分量|

### Accessors <Score text="Accessors" /> 
| **[zero](mw.Rotation.md#zero)**(): [`Rotation`](mw.Rotation.md)  |
| :-----|
| 获取一个空旋转的角度 (0, 0, 0)|

### Methods <Score text="Methods" /> 
| **[add](mw.Rotation.md#add)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| :-----|
| 旋转量a加上旋转量b|
| **[clone](mw.Rotation.md#clone)**(): [`Rotation`](mw.Rotation.md)  |
| 克隆当前旋转量|
| **[equals](mw.Rotation.md#equals)**(`other`: [`Rotation`](mw.Rotation.md), `epsilon?`: `number`): `boolean`  |
| 判断当前角度是否在误差范围内与指定向量相等。|
| **[fromQuaternion](mw.Rotation.md#fromquaternion)**(`v`: [`Quaternion`](mw.Quaternion.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换Quaternion为Rotation|
| **[fromString](mw.Rotation.md#fromstring)**(`v`: `string`, `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换字符串数据为Rotation|
| **[fromVector](mw.Rotation.md#fromvector)**(`v`: [`Vector`](mw.Vector.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换Vector为Rotation|
| **[getForce](mw.Rotation.md#getforce)**(`outer?`): [`Vector`](mw.Vector.md)  |
| 获取此旋转后的方向向量|
| **[getInverse](mw.Rotation.md#getinverse)**(`outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 返回一个新的反向旋转。|
| **[multiply](mw.Rotation.md#multiply)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 当前旋转量减去一个旋转量|
| **[rotateVector](mw.Rotation.md#rotatevector)**(`v`): [`Vector`](mw.Vector.md)  |
| 当前角度旋转一个向量|
| **[set](mw.Rotation.md#set)**(`v`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 为当前旋转量设置每个分量|
| **[strictEquals](mw.Rotation.md#strictequals)**(`other`: [`Rotation`](mw.Rotation.md)): `boolean`  |
| 判断当前角度是否与指定向量相等。|
| **[subtract](mw.Rotation.md#subtract)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 当前旋转量减去一个旋转量|
| **[toQuaternion](mw.Rotation.md#toquaternion)**(): [`Quaternion`](mw.Quaternion.md)  |
| 当前Rotation输出为四元数|
| **[toString](mw.Rotation.md#tostring)**(): `string`  |
| 当前Rotation输出为字符串|
| **[add](mw.Rotation.md#add-1)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 旋转量a加上旋转量b|
| **[copy](mw.Rotation.md#copy)**(`a`: [`Rotation`](mw.Rotation.md), `outer`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 复制目标旋转|
| **[fromQuaternion](mw.Rotation.md#fromquaternion-1)**(`v`: [`Quaternion`](mw.Quaternion.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换Quaternion为Rotation|
| **[fromString](mw.Rotation.md#fromstring-1)**(`v`: `string`, `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换字符串数据为Rotation|
| **[fromVector](mw.Rotation.md#fromvector-1)**(`v`: [`Vector`](mw.Vector.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 转换Vector为Rotation|
| **[lerp](mw.Rotation.md#lerp)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `alpha`: `number`): [`Rotation`](mw.Rotation.md)  |
| 对两个旋转量进行插值|
| **[multiply](mw.Rotation.md#multiply-1)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 当前旋转量减去一个旋转量|
| **[subtract](mw.Rotation.md#subtract-1)**(`a`: [`Rotation`](mw.Rotation.md), `b`: [`Rotation`](mw.Rotation.md), `outer?`: [`Rotation`](mw.Rotation.md)): [`Rotation`](mw.Rotation.md)  |
| 当前旋转量减去一个旋转量|

构建一个新的 Rotation。值为(0, 0, 0)

• **new Rotation**(`vector`)

用给定的 vector 中的x, y, z值设定给 x, y, z 。

#### Parameters

| `vector` [`Vector`](mw.Vector.md) | 给定的 vector |
| :------ | :------ |

• **new Rotation**(`forward`, `up`)

构造一个旋转，将旋转 Vector.FORWARD 以指向给定的前向矢量的方向，向上矢量作为参考。

::: warning Precautions

如果向前和向上指向完全相同 (或相反)的方向，或者其中之一的长度为 0，则返回 (0, 0, 0)。

:::

#### Parameters

| `forward` [`Vector`](mw.Vector.md) | 前向矢量 |
| :------ | :------ |
| `up` [`Vector`](mw.Vector.md) | 向上矢量 |

• **new Rotation**(`rotation`)

复制rotation，并返回一个新的。

#### Parameters

| `rotation` [`Rotation`](mw.Rotation.md) | 复制的 Rotation 对象 |
| :------ | :------ |

• **new Rotation**(`v`)

通过四元数构造

#### Parameters

| `v` [`Quaternion`](mw.Quaternion.md) | 四元数 |
| :------ | :------ |

• **new Rotation**(`x`, `y`, `z`)

通过三个分量构造

#### Parameters

| `x` `number` | 旋转的 x 分量 |
| :------ | :------ |
| `y` `number` | 旋转的 y 分量 |
| `z` `number` | 旋转的 z 分量 |

## Properties

### x <Score text="x" /> 

• **x**: `number`

旋转的 x 分量

___

### y <Score text="y" /> 

• **y**: `number`

旋转的 y 分量

___

### z <Score text="z" /> 

• **z**: `number`

旋转的 z 分量

## Accessors

### zero <Score text="zero" /> 

<table class="get-set-table">
<thead><tr>
<th style="text-align: left">

• `Static` `get` **zero**(): [`Rotation`](mw.Rotation.md)

</th>
</tr></thead>
<tbody><tr>
<td style="text-align: left">


获取一个空旋转的角度 (0, 0, 0)

#### Returns

</td>
</tr></tbody>
</table>

| [`Rotation`](mw.Rotation.md) | Rotation (0, 0, 0) |
| :------ | :------ |

## Methods

### add <Score text="add" /> 

• **add**(`a`): [`Rotation`](mw.Rotation.md) 

当前旋转量加上一个旋转量

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量,即旋转相加的结果 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相加的结果 |
| :------ | :------ |


#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |
### clone <Score text="clone" /> 

• **clone**(): [`Rotation`](mw.Rotation.md) 

克隆当前旋转量

#### Returns

| [`Rotation`](mw.Rotation.md) | 返回一个新的旋转量 |
| :------ | :------ |


___

### equals <Score text="equals" /> 

• **equals**(`other`, `epsilon?`): `boolean` 

判断当前角度是否在误差范围内与指定向量相等。

#### Parameters

| `other` [`Rotation`](mw.Rotation.md) | 比对的旋转量 |
| :------ | :------ |
| `epsilon?` `number` | 误差值 default:1.e-7 |

#### Returns

| `boolean` | 比对的结果 |
| :------ | :------ |


___

### fromQuaternion <Score text="fromQuaternion" /> 

• **fromQuaternion**(`v`): `void` 

当前Rotation读取一个四元数

#### Parameters

| `v` [`Quaternion`](mw.Quaternion.md) | Quaternion |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |


#### Parameters

| `v` [`Quaternion`](mw.Quaternion.md) | 读取的四元数数据 |
| :------ | :------ |

### fromString <Score text="fromString" /> 

• **fromString**(`str`): `void` 

当前Rotation读取一个字符串数据

#### Parameters

| `v` `string` | string |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |


#### Parameters

| `str` `string` | 字符串数据 |
| :------ | :------ |

### fromVector <Score text="fromVector" /> 

• **fromVector**(`v`): `void` 

当前Rotation读取一个Vector

#### Parameters

| `v` [`Vector`](mw.Vector.md) | Vector |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |


#### Parameters

| `v` [`Vector`](mw.Vector.md) | 读取的向量数据 |
| :------ | :------ |

### getForce <Score text="getForce" /> 

• **getForce**(`outer?`): [`Vector`](mw.Vector.md) 

获取此旋转后的方向向量

#### Parameters

| `outer?` [`Vector`](mw.Vector.md) | 被写入数据的向量, 传入的 outer 不能为null/undefined default:null |
| :------ | :------ |

#### Returns

| [`Vector`](mw.Vector.md) | 旋转的方向向量 |
| :------ | :------ |


::: warning Precautions

如果 outer 不为空, 返回 outer,否则返回一个新的 Rotation 对象, 建议传入 outer 来减少 new 对象且 outer 不能为 null/undefined

:::

___

### getInverse <Score text="getInverse" /> 

• **getInverse**(`outer?`): [`Rotation`](mw.Rotation.md) 

返回一个新的反向旋转。

#### Parameters

| `outer?` [`Rotation`](mw.Rotation.md) | 被写入数据的旋转量 default:null |
| :------ | :------ |

#### Returns

| [`Rotation`](mw.Rotation.md) | 反方向的旋转 |
| :------ | :------ |


::: warning Precautions

如果 outer 不为空, 返回 outer,否则返回一个新的 Rotation 对象, 建议传入 outer 来减少 new 对象且 outer 不能为 null/undefined

:::

___

### multiply <Score text="multiply" /> 

• **multiply**(`v`): [`Rotation`](mw.Rotation.md) 

当前旋转量乘以一个旋转量 (相当于四元数叉乘)

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量变量 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相乘的结果 |
| :------ | :------ |


#### Parameters

| `v` [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |
### rotateVector <Score text="rotateVector" /> 

• **rotateVector**(`v`): [`Vector`](mw.Vector.md) 

当前角度旋转一个向量

#### Parameters

| `v` [`Vector`](mw.Vector.md) | 被旋转的向量 |
| :------ | :------ |

#### Returns

| [`Vector`](mw.Vector.md) | 旋转后的向量 |
| :------ | :------ |


___

### set <Score text="set" /> 

• **set**(`v`): [`Rotation`](mw.Rotation.md)

当前旋转量设置为新的旋转量

#### Parameters

| `v` [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |

#### Returns

| [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |

• **set**(`x`, `y`, `z`): [`Rotation`](mw.Rotation.md) 

为当前旋转量设置每个分量


#### Parameters

| `x` `number` | 旋转的 x 分量 |
| :------ | :------ |
| `y` `number` | 旋转的 y 分量 |
| `z` `number` | 旋转的 z 分量 |

#### Returns

| [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |

**`Effect`**


___

### strictEquals <Score text="strictEquals" /> 

• **strictEquals**(`other`): `boolean` 

判断当前角度是否与指定向量相等。

#### Parameters

| `other` [`Rotation`](mw.Rotation.md) | 比对的旋转量 |
| :------ | :------ |

#### Returns

| `boolean` | 比对的结果 |
| :------ | :------ |


___

### subtract <Score text="subtract" /> 

• **subtract**(`a`): [`Rotation`](mw.Rotation.md) 

当前旋转量减去一个旋转量

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量变量 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相减的结果 |
| :------ | :------ |


#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量 |
| :------ | :------ |
### toQuaternion <Score text="toQuaternion" /> 

• **toQuaternion**(): [`Quaternion`](mw.Quaternion.md) 

当前Rotation输出为四元数

#### Returns

| [`Quaternion`](mw.Quaternion.md) | 输出的四元数 |
| :------ | :------ |


___

### toString <Score text="toString" /> 

• **toString**(): `string` 

当前Rotation输出为字符串

#### Returns

| `string` | 输出的字符串数据 |
| :------ | :------ |


___

### add <Score text="add" /> 

• `Static` **add**(`a`, `b`, `outer?`): [`Rotation`](mw.Rotation.md) 

旋转量a加上旋转量b


::: warning Precautions

outer 不能为 null/undefined

:::

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量,即旋转相加的结果 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相加的结果 |
| :------ | :------ |

___

### copy <Score text="copy" /> 

• `Static` **copy**(`a`, `outer`): [`Rotation`](mw.Rotation.md) 

复制目标旋转

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 目标旋转 |
| :------ | :------ |
| `outer` [`Rotation`](mw.Rotation.md) | 接收结果的旋转 |

#### Returns

| [`Rotation`](mw.Rotation.md) | 拷贝得到的新旋转对象 |
| :------ | :------ |


::: warning Precautions

outer 不能为 null/undefined

:::

___

### fromQuaternion <Score text="fromQuaternion" /> 

• `Static` **fromQuaternion**(`v`, `outer?`): [`Rotation`](mw.Rotation.md) 

转换Quaternion为Rotation


::: warning Precautions

如果 outer 不为空, 返回 outer,否则返回一个新的 Rotation 对象, 建议传入 outer 来减少 new 对象且 outer 不能为 null/undefined

:::

#### Parameters

| `v` [`Quaternion`](mw.Quaternion.md) | Quaternion |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |

___

### fromString <Score text="fromString" /> 

• `Static` **fromString**(`v`, `outer?`): [`Rotation`](mw.Rotation.md) 

转换字符串数据为Rotation


::: warning Precautions

如果 outer 不为空, 返回 outer,否则返回一个新的 Rotation 对象, 建议传入 outer 来减少 new 对象且 outer 不能为 null/undefined

:::

#### Parameters

| `v` `string` | string |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |

___

### fromVector <Score text="fromVector" /> 

• `Static` **fromVector**(`v`, `outer?`): [`Rotation`](mw.Rotation.md) 

转换Vector为Rotation


::: warning Precautions

如果 outer 不为空, 返回 outer,否则返回一个新的 Rotation 对象, 建议传入 outer 来减少 new 对象且 outer 不能为 null/undefined

:::

#### Parameters

| `v` [`Vector`](mw.Vector.md) | Vector |
| :------ | :------ |
| `outer?` [`Rotation`](mw.Rotation.md) | 传入的Rotation对象 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |

___

### lerp <Score text="lerp" /> 

• `Static` **lerp**(`a`, `b`, `alpha`): [`Rotation`](mw.Rotation.md) 

对两个旋转量进行插值

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `alpha` `number` | 插值 |

#### Returns

| [`Rotation`](mw.Rotation.md) | Rotation |
| :------ | :------ |


___

### multiply <Score text="multiply" /> 

• `Static` **multiply**(`a`, `b`, `outer?`): [`Rotation`](mw.Rotation.md) 

当前旋转量减去一个旋转量


::: warning Precautions

outer 不能为 null/undefined

:::

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量变量 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相乘的结果 |
| :------ | :------ |

___

### subtract <Score text="subtract" /> 

• `Static` **subtract**(`a`, `b`, `outer?`): [`Rotation`](mw.Rotation.md) 

当前旋转量减去一个旋转量


::: warning Precautions

outer 不能为 null/undefined

:::

#### Parameters

| `a` [`Rotation`](mw.Rotation.md) | 旋转量a |
| :------ | :------ |
| `b` [`Rotation`](mw.Rotation.md) | 旋转量b |
| `outer?` [`Rotation`](mw.Rotation.md) | 接收结果的旋转量变量 default:null |

#### Returns

| [`Rotation`](mw.Rotation.md) | 相减的结果 |
| :------ | :------ |
