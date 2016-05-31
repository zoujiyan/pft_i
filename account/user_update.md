## 修改用户信息

####1.基本信息
- 接口地址：`{API_URL}/user/update`  
- 请求方式：POST


####2.参数信息  

| 参数名    | 必填      | 说明      |
| -------   |:-------:  |--------   |
| uid       | 是        | 用户ID    |
| token     | 是        | 用户令牌  |
| sign      | 是        | 数据校验码|
| phone     | 否        | 会员用户新手机号  |
| vcode     | 否        | 短信验证码（新手机号）  |
| name      | 否        | 用户名  |
| sex       | 否        | 性别<br>0 女<br>1 男|
| face      | 否        | 用户头像  |
| sno       | 否        | 学号      |
| birthym   | 否        | 出生年月  |
| school    | 否        | 学校      |
| class     | 否        | 班级      |
| stature   | 否        | 身高      |
| weight    | 否        | 体重      |

####3.报文响应

```
{
	"status":1,
	"msg":"success",
	"data":
}
```

|键    |类型  |说明  |
|------|------|------|
|status|int   |修改结果<br>1 成功<br>0 失败|
|msg   |String|结果信息描述|
