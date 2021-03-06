# yuketangHelper

#### 介绍

分享华南理工大学大佬写的5分钟刷完雨课堂视频代码

#### 说明

特别鸣谢：https://github.com/heyblackC/yuketangHelper
特别声明：一切代码均来自华南理工大学大佬，github见上，可以给大佬star一下，tql，orz。

我只是实践一下跨校功能，并传播好的工具。

长江雨课堂参考大佬的github，这里没有测试长江雨课堂的。

**对于没有任何编程基础的非计算机专业的同学，务必确保你的电脑上有python环境再来使用该脚本**

**刷课期间保持网页端雨课堂在线**

#### 核心操作

1.更改csrftoken和sessionid字段

2.把gsscut.yuketang.cn更改为自己学习的网址，如tust.yuketang.cn

3.根据登录后cookie里的university_id值，更改代码中university-id、university_id、uv_id 。

#### 具体流程

1. 下载yuketang压缩包

2. 解压后得到yuketangHelper-master

3. 使用记事本或者其他编辑软件打开videoHelper.py，我这里使用notepad++。

   ![image-20211108144258117](https://gitee.com/doubleguy/typora/raw/master/img/202111081442285.png)

   

4. 使用chrome登陆网页版雨课堂，按F12，点Application，找到Storage中的Cookies，找到https://xxx.yuketang.cn/。其中xxx代表学校，如果你是研究生，网址应该是 https://yjs.xxx.yuketang.cn/ 。找到csrftoken和sessionid字段，然后将videoHelper.py中的csrftoken和sessionid更改成自己登录后的cookie中对应的字段。

   ![image-20211108144756714](https://gitee.com/doubleguy/typora/raw/master/img/202111081447918.png)

5.由于初始代码是针对华南理工的，所以跨校的还要改一下网校网址。在notepad++中ctrl+f，把所有的**gsscut.yuketang.cn**替换成对应学校的网址，比如天津科技大学是tust.yuketang.cn。**注意：**研究生的网址是**yjs.tust.yuketang.cn**，但是我们不能替换成**yjs.tust.yuketang.cn**，否则会出现以下错误。换句话来说，不管你是不是研究生，都用**xxx.yuketang.cn**（我们学校就是**tust.yuketang.cn**）就行了,不用加上yjs前缀。

![image-20211108145428054](https://gitee.com/doubleguy/typora/raw/master/img/202111081454219.png)

6.根据登录后cookie里的university_id值，更改代码中university-id、university_id、uv_id 。改完后保存。

![image-20211108150315423](https://gitee.com/doubleguy/typora/raw/master/img/202111081503642.png)

7.使用cmd（如果你是直接下载python安到电脑里的，非计算机专业推荐直接下个python到电脑里用cmd运行代码）或者使用Anaconda Prompt(使用的conda自带的python环境)，找到你下载的代码路径，比如我的是  D:\黑科技\yuketangHelper-master

![image-20211108150807000](https://gitee.com/doubleguy/typora/raw/master/img/202111081508064.png)

就先输入 D: 进入D盘，然后输入 D:\黑科技\yuketangHelper-master 进入文件夹，然后在输入videoHelper.py执行代码。

运行界面如下：

![image-20211108151002215](https://gitee.com/doubleguy/typora/raw/master/img/202111081510400.png)

刷新一下网页，网课全部刷完，太快了！！！

![image-20211108151054105](https://gitee.com/doubleguy/typora/raw/master/img/202111081510233.png)

最后再次诚挚的感谢大佬贡献的代码！！！

## 天科专用

1.下载tust文件夹，根据cookies中的csrftoken和sessionid更改videoHelper.py中的csrftoken和sessionid字段

2.使用cmd或者Anaconda Prompt运行videoHelper.py即可。