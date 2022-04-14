---
description: 调用此api会随机返回电脑端或手机端的图片
---

# 完全随机返回随机图片

### 请求URL

```
https://www.loliapi.com/bg/
```

{% hint style="success" %}
URL中的 bg 是**Background**的简写
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

[https://www.loliapi.com/bg/](https://www.loliapi.com/bg/)

访问会返回一个随机图片

#### 高级调用格式

如果想获取 id 为 23 的图片的 json 数据，就应该访问

[https://www.loliapi.com/bg/?id=23\&type=json](https://www.loliapi.com/bg/?id=23\&type=json)

访问会返回

```
{
    "site": "www.Loliapi.com",
    "imgurl": "https:\/\/tva1.sinaimg.cn\/large\/0075ueBvly1gxct1fxp2ij31hc0u0qq0.jpg",
    "width": "1920",
    "height": "1080"
}
```

或

```
{
    "site": "www.Loliapi.com",
    "imgurl": "https:\/\/tva1.sinaimg.cn\/large\/0075ueBvly1gxcsxrhtsdj312z1kwtiu.jpg",
    "width": "1403",
    "height": "2048"
}
```
