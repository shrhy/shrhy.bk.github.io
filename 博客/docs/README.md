# 程成的博客

>All Rights Reserved.©程成

## Fanbook机器人

### Fanbook机器人如何发送消息

#### 1.使用代码

以下是python代码,大家运行即可

```python
import requests

import json



lp=input('输入你的机器人token（令牌）')

pdid=input('输入你的频道id')

xx=input('输入你要发送的内容')

url = ' https://a1.fanbook.mobi/api/bot/'+lp+'/sendMessage'

headers = {'content-type': "multipart/form-data;charset=utf-8"}

jsonfile = json.dumps({

    "chat_id": int(pdid),

    "text": xx,

})

postreturn=requests.post(url,data=jsonfile,

                         headers=headers)

print(postreturn.text)#输出返回


```

#### 2.使用工具(推荐使用凯子制作的快捷平台)

链接:

凯子制作的快捷平台:

[Fanbook 机器人工具 (starlight.work)](https://fb-bot.starlight.work/)

进去之后输入你的机器人token(令牌)

![image-20230304140912402](D:\博客\image-20230304140912402.png)

(小声逼逼,可添加多个机器人)

然后点发送信息

![image-20230304141022132](D:\博客\image-20230304141022132.png)

接着跟着提示制作就行了

![image-20230304141046685](D:\博客\image-20230304141046685.png)

(小声逼逼,其实是我太懒了)

最后结果

![image-20230304141233195](D:\博客\image-20230304141233195.png)

(持续更新......)
