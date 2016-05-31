##获取教练信息列表

####1.基本信息
- 接口地址：`{API_URL}/dl/getcoach` 
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
	"data":{
		"size":10,	
		"list":[
			{
				"cid":62,
				"name":"张教练"
				"sex":1,
				"school":"人大",
				"item":"篮球，游泳",
				"award":"优秀教练",
				"face":""
			},
			...
		]
	}
}
```

|键    |类型  |说明  |
|--------|------|------|
|status  |int   |获取结果<br>1 成功<br>0 失败|
|msg     |String|结果信息描述|
|size    |int   |列表大小|
|cid     |int   |教练ID|
|name    |String|教练姓名|
|sex     |int   |性别    |
|school  |String|毕业院校|
|item    |String|擅长项目   |
|award   |String|曾获荣誉   |
|face    |String|头像|
