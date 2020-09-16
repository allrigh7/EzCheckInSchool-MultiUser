# EzCheckInSchool-MultiUser         
 
修改自[chillsoul的EzCheckInSchool](https://github.com/chillsoul/EzCheckInSchool)
 
功能与使用方法均与其相同

唯一的不同之处在于此版本可同时为多个成员打卡

修改这个的主要原因是不愿意早起

用了大佬的脚本自己不担心打卡了 

但是每天早上依旧被舍友的闹钟吵醒

于是乎

为了早上舒舒服服的睡懒觉

我改写了这个脚本用来为舍友打卡••••••

## 更新日志

2020.9.16  更换微信推送使用的api，不再需要github账户绑定server酱，并且可以想每个用户单独推送其打卡状态

2020.9.15  更新微信推送，现在所有人的打卡信息只会发送一条推送信息

2020.9.14  第一版发布，对应chillsoul的版本9.12更新

## 使用方法

首先，点击页面上方`Star`并`Fork`，此时你将得到复制的项目

点击此链接获取二维码

[QRcode](http://wxpusher.zjiecode.com/api/qrcode/1men6ZnAtqckyldYHDbYfOKSsqcxxhXtu6nXChdP9iybdir048fJ1VxU0W5Kwlgo.jpg)

每个用户都需要扫描此二维码关注新消息服务公众号

然后依次点击`我的`->`我的UID`，获取每个用户的UID

接下来你需要设置`Secert`添加以下四项内容 

Fork的项目->Settings->Secert->New Secert

打开完美校园健康打卡，参照打卡页面上方个人信息及如下表格设置

这一步与原版本不同，每项secert可以添加多个信息

中间使用半角逗号分隔

个数不限

要注意每项数据的顺序需要一一对应

|Name|Value|示例|
| :-----| :---- | :---- |
|`DEPT_TEXT`|`学院-专业-班级`|`理学院-应用物理学-应物1901,理学院-应用物理学-应物1901`|
|`STU_ID`|`学号`|`201912340101,201912340101`|
|`STU_NAME`|`姓名`|`张三,李四`|
|`UID`|`公众号获取的UID`|`UID_abcdefghijklmnopqrstuvwxyz,UID_abcdefghijklmnopqrstuvwxyz`| 

以上步骤完成后

Fork的项目主页->Action->I understand... 开启Actions

回到项目主页，修改[README.md](/README.md)随便加几个空格即可

**首次开启若不在打卡时间将会重打早间卡作为测试**

设置完成打卡后打卡时间内会每天自动打卡三次，第一次使用请观察效果。

**注意：本项目默认学校为河南工业大学，其他学校请自行抓包修改代码。**



## 友情链接

https://github.com/chillsoul/EzCheckInSchool - 修改自此项目



