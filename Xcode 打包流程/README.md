# 生成 app id
```
如果已经创建好 app id, 可以跳过这一步
```
* 登录 apple 后台
```
https://developer.apple.com/membercenter
```

* 添加 app id

  ![](./Resource/1.jpg)

  继续

  ![](./Resource/2.jpg)

  如果提示如下,说明 id 被占用了,需要替换.`(注意 Xcode 中的 bundle id也要对应修改)`
  ![](./Resource/3.jpg)

# 生成证书

* Xcode 登录开发者账号  

  ![](./Resource/5.jpg)  
  ![](./Resource/6.jpg)

* 创建开发者证书  
Xcode -> Accounts -> Manager Certificates
![](./Resource/4.jpg)
![](./Resource/7.jpg)

* 开启自动签名  
![](./Resource/8.jpg)

* 设置 Archive 参数  
![](./Resource/9.jpg)
![](./Resource/10.jpg)

* 选择 Devices  
![](./Resource/11.jpg)

* 打包  
![](./Resource/12.jpg)  

  如果因第三库不支持 bitcode 导致打包失败  
  ![](./Resource/14.jpg)

  关闭 bitcode  
  ![](./Resource/15.jpg)

* 导出  
![](./Resource/13.jpg)
![](./Resource/16.jpg)
![](./Resource/17.jpg)

  App Thinning 用来打指定架构的包,减少 app 体积
  ![](./Resource/18.jpg)

  自动签名  
  ![](./Resource/19.jpg)
  ![](./Resource/20.jpg)
