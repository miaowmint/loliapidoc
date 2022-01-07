---
description: 目前收录了98张图片
---

# 手机端随机图片

### 请求URL

```
https://www.loliapi.com/acg/pe/
```

{% hint style="success" %}
URL中的 pe 是**Pocket Edition**的简写
{% endhint %}

### 请求参数（get）

| 参数名称 |     参数值     |    参数说明   | 参数类型 |
| :--: | :---------: | :-------: | :--: |
|  id  | 不多于图片收录数的整数 | 指定id对应的图片 |  可选  |

| 参数名称 |  参数值 |     参数说明     | 参数类型 |
| :--: | :--: | :----------: | :--: |
| type |      |   重定向到图片源网址  |  默认  |
| type |  url |    返回图片源网址   |  可选  |
| type |  img |  返回图片源网址对应图片 |  可选  |
| type | json | 返回图片相关json数据 |  可选  |

### 请求示例

#### 最基本调用格式

[https://www.loliapi.com/acg/pe/](https://www.loliapi.com/acg/pe/)

访问会返回一个随机图片

#### 高级调用格式

如果想获取 id 为 23 的图片的 json 数据，就应该访问

[https://www.loliapi.com/acg/pe/?id=23\&type=json](https://www.loliapi.com/acg/pe/?id=23\&type=json)

访问会返回

```
{
    "site": "www.Loliapi.com",
    "imgurl": "https:\/\/tva1.sinaimg.cn\/large\/0075ueBvly1gxcsxrhtsdj312z1kwtiu.jpg",
    "width": "1403",
    "height": "2048"
}
```
