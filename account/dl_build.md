##锻炼数据录入   test

####1.基本信息
- 接口地址：`{API_URL}/dl/build` 
- 请求方式：POST


####2.参数信息  

| 参数名    | 必填      | 说明      |
| -------   |:-------:  |--------   |
| uid       | 是        | 用户ID    |
| token     | 是        | 用户令牌  |
| sign      | 是        | 数据校验码|
| stature   | 否        | 身高|
| weight    | 否        | 体重|
| item1     | 否        | 规定项目1|
| time1     | 否        | 运动时长1|
| count1    | 否        | 运动成果数量1|
| item2     | 否        | 规定项目2|
| time2     | 否        | 运动时长2|
| count2    | 否        | 运动成果数量2|
| item3     | 否        | 自选项目|
| time3     | 否        | 运动时长3|
| count3    | 否        | 运动成果数量3|


####3.报文响应

```
{
	"status":1,
	"msg":"success",
	"data":
}
```

|键      |类型  |说明  |
|--------|------|------|
|status  |int   |结果<br>1 成功<br>0 失败|
|msg     |String|结果信息描述|

