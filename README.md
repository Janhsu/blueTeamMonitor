# buleTeamMonitor

重保期间监测网站页面内容变动的小工具

### 项目用途

用于无系统接管权限的蓝队驻场情况，通过该项目可以实现挂机监测网站页面内容变动情况，在被挂黑页时可及时做出响应。

### 用法

1.填写单个网站或者批量导入网站，点击增加

2.设置刷新间隔，默认60秒

3.开启监控

![image](https://user-images.githubusercontent.com/62692103/197106095-3781f704-1b9a-4fa2-af31-924659ff0422.png)

导入txt文件内容格式如下:
百度,https://www.baidu.com
github,https://github.com
名字与网址用英文逗号隔开，每个目标一行

### 开启飞书提醒
默认注释了飞书发送消息的相关代码，目前仅支持弹窗提醒和日志记录的功能。
如何开启？
1.暂时没有在界面上开放飞书webhook输入选项，需要在代码中填入飞书的webhook地址
![image](https://user-images.githubusercontent.com/62692103/197106789-2b2ceffa-f981-4a4a-858c-1c3f9613e11b.png)
2.飞书捷径的配置如下
![image](https://user-images.githubusercontent.com/62692103/197107156-372bb97d-54e5-4104-b9e1-7373fec1195c.png)
3.取消注释
![image](https://user-images.githubusercontent.com/62692103/197107408-a12adf38-54e8-45c4-9d3c-c7b10ca4fed0.png)

开启后的效果
![164110e5c086abf26f03eb678f6e165](https://user-images.githubusercontent.com/62692103/197108180-cb0c5741-fc38-469c-bdb6-744db6a98cc6.jpg)

### 注意事项
该工具目前只能用于每次页面请求内容不动态更新的网站，暂时不支持动态更新的网站，如百度等。因为原理很简单，就是根据每次请求数据包长度是否变化进行判断。

### 免责声明
在使用本工具时，您应确保该行为符合当地的法律法规，并且已经取得了足够的授权。请勿对非授权目标进行访问。
如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，我们将不承担任何法律及连带责任。
