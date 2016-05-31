## 获取积分兑换信息列表

####1.基本信息
- 接口地址：`{API_URL}/user/getpre`  
- 请求方式：POST


####2.参数信息  

| 参数名    | 必填      | 说明      |
| -------   |:-------:  |--------   |
| uid       | 是        | 用户ID    |
| token     | 是        | 用户令牌  |
| sign      | 是        | 数据校验码|


####3.报文响应

```
{
	"status":1,
	"msg":"success",
	"data":｛
		"size":10,	
		"list":[
			{
				"pid":123,
				"name":"杜莎夫人蜡像馆门票",
				"img":"http://img.mp.itc.cn/upload/20160531/feef848c2dc140eabfb16f8680fcf95c_th.jpg",
				"score":80,
				"detail":"Lorem ipsum dolor sit amet,consectetur adipiscing elit. ",
				"method":"Aenean euismod bibendum laoreet. ",
				"flow":"Proin gravida dolor sit amet lacus"
			},
			...
		]
	｝
}
```

|键    |类型  |说明  |
|------|------|------|
|status  |int   |获取结果<br>1 成功<br>0 失败|
|msg     |String|结果信息描述|
|size    |int   |列表大小|
|pid     |int   |产品id|
|name    |String|产品名称|
|img     |String|产品图片url    |
|score   |int|兑换所需积分|
|detail  |String|产品详情    |
|method  |String|使用方法    |
|flow    |String|兑换流程    |

