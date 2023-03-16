# 放行接口提示认证失败
- - -
## 可能的原因
接口放行后不需要token即可访问<br>
但是没有token也就无法获取用户信息与鉴权

## 解决方案
删除接口上的鉴权注解<br>
删除接口内获取用户信息功能<br>
删除数据库实体类 自动注入 `createBy` `updateBy` 因为会获取用户数据