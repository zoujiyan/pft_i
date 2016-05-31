## 获取用户积分信息

####1.基本信息
- 接口地址：`{API_URL}/dl/getscore`  
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
		"name":"张三",
		"rankc":10,
		"ranks":100,
		"rankct":5,
		"rankst":50,
		"score":2300,
		"scoret":80

	｝
}
```

|键    |类型  |说明  |
|------|------|------|
|status|int   |获取结果<br>1 成功<br>0 失败|
|msg   |String|结果信息描述|
|uid   |int   |用户ID|
|name  |String|用户名|
|rankc |int|班级排名|
|ranks |int|学校排名|
|rankct|int|今日班级排名|
|rankst|int|今日学校排名|
|score |int|总积分|
|scoret|int|今日积分|


