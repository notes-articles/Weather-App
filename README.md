---
typora-root-url: ..\..\..\..\img
---



## 关于CSS文件一会有效，一会样式代码缺失

清除浏览器缓存文件

清除liver-server本地项目缓存





## 停止liver

停止liver-server

![image-20240531104536001](/image-20240531104536001.png)



![image-20240531104630641](/image-20240531104630641.png)



 

## 关于liver-server缓存项目css文件

它会在Chrome下载内容目录下，缓存特定端口的文件，

比如:5500端口，那它的文件名就是，`127.0.0.1%3A5500`。

![image-20240531103848697](image-20240531103848697.png)

在这个目录下，存放具体项目的css缓存文件

![image-20240531104113320](/image-20240531104113320.png)

![image-20240531104129025](/image-20240531104129025.png)





## [openweather](https://openweathermap.org/)

注册信息

xy

stormyangzy@qq.com

33333333





API key

```txt
22feff554f32c4e3995eb9643c54d78c
```





[weather API 文档](https://openweathermap.org/current)

接口：

```txt
https://api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={API key}
```

Parameters

**lat（必需）**：

- **含义**：Latitude（纬度）。该参数用于指定地理位置的纬度。
- **建议**：如果你需要自动将城市名称和邮政编码转换为地理坐标（即经纬度）或将地理坐标转换为城市名称和邮政编码，请使用 Geocoding API。

**lon（必需）**：

- **含义**：Longitude（经度）。该参数用于指定地理位置的经度。
- **建议**：同样地，如果你需要自动将城市名称和邮政编码转换为地理坐标（即经纬度）或将地理坐标转换为城市名称和邮政编码，请使用 Geocoding API。





## [汉字转拼音](https://pinyin-pro.cn/guide/start.html)

```js
<script src="https://unpkg.com/pinyin-pro"></script>

<script>
  var { pinyin } = pinyinPro;
  pinyin('汉语拼音'); // 'hàn yǔ pīn yīn'
</script>
```

### [参数](https://pinyin-pro.cn/use/pinyin.html#%E8%AF%AD%E6%B3%95%E5%8F%8A%E5%8F%82%E6%95%B0)

**toneType**

```js
pinyin('汉语拼音', { toneType: 'none' }); // 'han yu pin yin'
```

**separator**

```js
pinyin('汉语拼音', { separator: '-' }); // 'hàn-yǔ-pīn-yīn'
=
```

**参数组合**

```js
pinyin('汉语拼音', { toneType: 'none',separator: '-' }); // 'hanyupinyin'
```

