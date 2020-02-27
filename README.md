# dedecms-sdk

## 安装插件

1. 复制 `include/payment/bapp.php` 到您的织梦CMS的 `include/payment/` 下  
1. 进入 「织梦CMS管理后台」-「系统」-「系统设置」-「SQL命令行工具」-「运行SQL命令行」-「单行命令」
  复制以下代码，并点击 「确认」
 
```sql
insert ignore into `dede_payment` set `code`='bapp',`name`='B.app',`fee`=0,`description`='B.app操作簡單，掃一掃即可完成支付，免礦工費，支持大額支付',`rank`=1,`config`='a:2:{s:12:"bapp_app_key";a:4:{s:5:"title";s:13:"B.app App Key";s:11:"description";s:21:"在B.app商户后台中获取";s:4:"type";s:4:"text";s:5:"value";s:0:"";}s:15:"bapp_app_secret";a:4:{s:5:"title";s:16:"B.app App Secret";s:11:"description";s:21:"在B.app商户后台中获取";s:4:"type";s:4:"text";s:5:"value";s:0:"";}}',`enabled`=0,`cod`=0,`online`=1;
```

  当有提示 `成功执行1个SQL语句！` 即可完成插件安装
  
## 配置参数

1. 进入 「织梦CMS管理后台」-「系统」-「系统设置」-「支付工具」-「支付接口设置」  
1. 找到 B.app 后点击 「安装」  
1。 点 「更改」，填上B.app `App Key` 和 `App Secret` ，并点 「确定」


------


如果安装插件遇到问题，请用B.app扫码以下二维码，联系官方客服  
![请用B.app扫码](https://www.b.app/assets/img/pic/customer_service_qrcode.png)