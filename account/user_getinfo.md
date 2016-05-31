## 获取用户信息

####1.基本信息
- 接口地址：`{API_URL}/user/getinfo`  
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
		"user":"12345678901",
		"name":"张三",
		"sex":1,
		"isvip":1,
		"phone":18612345678,
		"face":"",
		"token":"f88205a4eb1c15339158156380579dd1"
	｝
}
```

|键    |类型  |说明  |
|------|------|------|
|status|int   |获取结果<br>1 成功<br>0 失败|
|msg   |String|结果信息描述|
|uid   |int   |用户ID|
|user  |String|用户登录名|
|name  |String|用户名|
|sex   |int|性别<br>0 女 <br>1 男|
|isvip |int|是否为会员<br>0 不是 <br>1 是|
|phone |String|会员绑定的电话，非会员时为空|
|face  |String|用户头像（默认为空，按显示默认头像）|
|token |String|用户令牌（校验用户登录状态的有效性）|

