## 获取用户消费信息列表

####1.基本信息
- 接口地址：`{API_URL}/user/getuserpre`  
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
		"uid":123,
		"size":10,	
		"list":[
			{
				"pid":123,
				"name":"杜莎夫人蜡像馆门票",
				"img":"http://img.mp.itc.cn/upload/20160531/feef848c2dc140eabfb16f8680fcf95c_th.jpg",
				"score":80,
				"time":"2015-10-02 16:30",
				"code":"JHI561280",
				"status":1
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
|uid     |int   |用户id|
|pid     |int   |产品id|
|name    |String|产品名称|
|img     |String|产品图片url    |
|score   |int|兑换所需积分|
|time    |String|兑换时间    |
|code    |String|兑换码      |
|status  |int|兑换状态<br>1.已兑换 2.已使用 3.已失效    |

