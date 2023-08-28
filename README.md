
# 一、人工智能AI绘画
AI作画,用户可以在平台上输入各种与风格、主题、氛围有关的关键词，AI根据这些关键词在互联网巨量的资源和素材中搜索、学习，最后糅合与拼接成一些符合要求的画作.
# 二、使用步骤
## 1、接口

***重要提示:建议使用https协议,当https协议无法使用时再尝试使用http协议***

请求方式: POST

```
https://luckycola.com.cn/aiImg/getAiImage
```
## 2、请求参数
| 序号 | 参数 | 是否必须|说明 |
|--|--|--|--|
| 1 |imgTxt  |是 | 需要生成的AI绘画的描述,描述越准确,生成的图片越精美,下面提供几个优秀的描述实例 |
| 2 |appKey  |是 | 唯一验证AppKey, 可前往官网“个人中心“获取([http(s): //luckycola.com.cn](http://luckycola.com.cn)), 下面具体介绍获取方法|
| 3 |uid  |是 | 账号等唯一标识, 可前往官网“个人中心“获取([http(s): //luckycola.com.cn](http://luckycola.com.cn)), 下面具体介绍获取方法|
| 4 |style  |是| 需要指定的绘画风格, 现在可填写的值有以下几种: ['探索无限'、 '古风',、'二次元'、'写实风格'、'浮世绘'、 'low poly' ,、'未来主义'、 '像素风格',、'概念艺术'、'赛博朋克'、'洛丽塔风格'、 '巴洛克风格'、'超现实主义'、 '水彩画'、'蒸汽波艺术'、 '油画'、'卡通画']|
| 4 |ratio  |是 | 需要生成图片的宽高比,现在可以填写的有以下几种:("1:1"、"3:2"、"2:3") |


**注意!!!: 如果您还没有appKey和uid,请先请前往官网获取**
官网地址:[http(s): //luckycola.com.cn/](http://luckycola.com.cn/)


## 3、请求参数示例

```json
{
	// 对生成图片的详细要求的描述词,描述越准确生成结果越精美
    "imgTxt": "一张二次元的可爱的科技感的男神头像",
     // 官网-个人中心-Appkey获取
    "appKey": "6*********5",
    // 官网-个人中心-用户ID获取
    "uid": "cVLW1X1676709440059",
    // 绘画风格 可选值: ['探索无限'、 '古风',、'二次元'、'写实风格'、'浮世绘'、 'low poly' ,、'未来主义'、 '像素风格',、'概念艺术'、'赛博朋克'、'洛丽塔风格'、 '巴洛克风格'、'超现实主义'、 '水彩画'、'蒸汽波艺术'、 '油画'、'卡通画']
    "style": "探索无限",
    // 生成图片的宽高比,值可选有:"1:1"、"3:2"、"2:3"
    "ratio": "1:1"
}
```

## 4、接口 返回示例
**温馨提示:** AI绘画需要时间--接口返回平均10秒左右
**温馨提示:** AI绘画需要时间--接口返回平均10秒左右

```json
// AI绘画需要时间--接口反馈平均10秒左右
{
	// 	请求成功状态码
	"code": 0,
	// 请求结果提示
	"msg": "AI绘图返回成功",
	"data": {
		// AI绘画的结果
		"result": {
			"img": "https://wenxin.baidu.com/younger/file/ERNIE-ViLG/bd619f4b81e2de0bca1d96aef96cf60cex",
			"imgUrls": [
				{
					"image": "https://wenxin.baidu.com/younger/file/ERNIE-ViLG/bd619f4b81e2de0bca1d96aef96cf60cex"
				}
			]
		},
	}
}

```
# 三、 AI绘画优秀描述例子

| 序号 | 描述(imgTxt)|
|--|---|
| 1 |火车，田野，大师作品，宫崎骏生成风格  |
| 2 |蓝天白云，青青草坡，微风，吉卜力风格，丁达尔效应，二次元生成风格：二次元场景  |
| 3 |美人鱼，穿着蓝色的外套，海底下，深情的眼睛，双眼皮，长睫毛，红嘴唇，可爱的脸蛋，，红色头发。大师作品，最好画质，更高质量，高细节，超高分辨率  |
| 4 |中国十二生肖，老鼠，拟人，中国古代服装，站立，可爱，3D，白色背景，干净背景， 皮克斯动画， 自然光  |



# 四、 如何获取appKey和uid

### 1、申请appKey:
登录**Luckycola官网**([http(s): //luckycola.com.cn](http://luckycola.com.cn)),进入“[**个人中心**]“,即可进行申请
![在这里插入图片描述](https://img-blog.csdnimg.cn/684861db7426459c8790f65d3e0b0c84.png#pic_center)

### 2、获取appKey和uid
AppKey申请通过后,登录**Luckycola官网**([http(s): //luckycola.com.cn](http://luckycola.com.cn)),进入“[**个人中心**]“即可获取
![在这里插入图片描述](https://img-blog.csdnimg.cn/3112de0520cf4ecfa2edddefc7a15fd2.png#pic_center)


# 五、重要说明
**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!

**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!

**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!


# 六、AI绘画成果展示
![在这里插入图片描述](https://img-blog.csdnimg.cn/442fa70bd71442a090c3ebd09eb55d8b.jpeg#pic_center)
![在这里插入图片描述](https://img-blog.csdnimg.cn/d8e91016ad1c4ff7aea2b1dc7710c650.png#pic_center)
![在这里插入图片描述](https://img-blog.csdnimg.cn/08bd7fae3a0a42c9873ff64226faf5df.png#pic_center)
