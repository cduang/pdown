# pdown
---
PDown下载器
> PDown是个人项目，开始是作为毕业设计立项，为了方便宿舍下载试验资料。 现在分享出来希望可以帮助到更多的人

![demo](down600.gif)


#### [蓝奏云 4-4 22:21 下载地址  https://pdown.lanzous.com/ib00pof](https://pdown.lanzous.com/ib00pof)
---
### 0.项目刚发布有不少BUG，请参阅 [更新日志.md](更新日志.md)  
最新更新时间：2020-4-4 22:21  
如果遇到各种不能下载/无限拉取，请多包容，过一天再试BUG可能就被修复了，请留意我们的版本更新<br/>

#### 单个文件体积最大100MB，链接内所有文件的总体积最大500MB
请见谅，PDown只是方便大家临时应急。大文件会导致其他人长时间的等待
<br/>  
  
### 1.安装使用

软件是单文件.exe(**15MB**) 无需安装,下载后双击直接运行<br/>
直接粘贴  **完整的**  分享链接和**提取码**，就可以下载了。不需要登录你的bd账号<br/>
像这样粘贴完整的链接+提取码：<br/>
```
https://pan.bxxdu.com/s/1jxP5vznx3_XvHrPKv1yhKg 提取码：97zc 
```

### 2.加速原理

你提交链接  -->  我去下载  -->  我传给你<br/><br/>
所以可能你的任务会长时间一直在拉取（当时人太多要排队），请耐心等着

### 3.加速效果

个人免费项目，所以有限制，不要期望太高<br/>
* 单文件体积=1MB时，下载速度=600kb/s   -->  单文件体积=100MB时，下载速度=120kb/s<br/>
* 单文件的下载速度 会随文件体积增加<b>线性减少</b>，但速度十分稳定（比如一直是600kb/s）<b>不会</b>下载到90%就没速度了<br/>
* 最多三个文件同时下载，所以总速度=单文件速度 x 3<br/>
  
例如你同时下载3个文件（体积都是10MB），下载速度是500kb/s x 3 = 1.5MB/s<br/><br/>
  
<b>有特殊情况:</b><br/>
* 同时使用的人很多时，要排队拉取，你需要等待很长时间，才能拉取成功 ( 尤其是晚上10点左右 )<br/>
* 有的文件本身下载就很慢，甚至不能下载，应该是CDN调度问题 ( 比较常见 )<br/>

<br/>
<br/>

#### （投票调查）是否需要自己部署后台服务器？

理论上大家可以自己搭建后台服务器，这样就不需要等待排队拉取了，下载速度完全取决于你自己的服务器的宽带<br/>
* 你需要有一个BD超级VIP账号
* 你需要有一个稳定运行的服务器并且硬盘够大，网速够快（包括下载和上传速度都要快）
* 服务器需要配置IIS(.net api),安装mssql数据库，安装监控程序，安装下载程序，修改程序的配置文件
* 不换IP的话，在解析数十个链接后，每解析一个链接都需要你手动输入验证码
* 发布了教程后，一切配置问题我都没时间帮助你，遇到问题需要自行摸索（ 每个人系统环境+配置都不太一样 ）

[![](https://api.gh-polls.com/poll/01E63G20EVMP01VAS3573J490T/%E6%88%91%E6%83%B3%E6%88%91%E5%8F%AF%E4%BB%A5%E8%87%AA%E5%B7%B1%E6%90%AD%E5%BB%BA)](https://api.gh-polls.com/poll/01E63G20EVMP01VAS3573J490T/%E6%88%91%E6%83%B3%E6%88%91%E5%8F%AF%E4%BB%A5%E8%87%AA%E5%B7%B1%E6%90%AD%E5%BB%BA/vote)
[![](https://api.gh-polls.com/poll/01E63G20EVMP01VAS3573J490T/%E4%B8%8D%E9%9C%80%E8%A6%81%E5%A4%AA%E9%BA%BB%E7%83%A6BUG%E4%B9%9F%E5%A4%9A)](https://api.gh-polls.com/poll/01E63G20EVMP01VAS3573J490T/%E4%B8%8D%E9%9C%80%E8%A6%81%E5%A4%AA%E9%BA%BB%E7%83%A6BUG%E4%B9%9F%E5%A4%9A/vote)
  
<br/><br/>

---

#### Q:什么时候会收费？
个人项目，永久免费。实在没钱我会关掉项目。所以永远免费。
#### Q:文件版权纠纷?
我一直在监管版权问题，并且提供了醒目的举报入口，欢迎大家和我们一起维护版权。只要举报无条件封杀<br/>
因为只有小文件，加上是个人项目并没有很多人在用。实际上也很难有所谓版权纠纷。<br/>
但如果确实涉及到您的版权请及时联系我。我会立即清理<br/>
#### Q:有问题怎么联系？
github上发Issue吧，我会不定时的来看看的，看到了就会回复你
#### Q:会开源吗？用的什么技术？
客户端是c++，用到了SOUI3，SQLite，Curl，等等，界面都是我自己设计后用PS贴图<br/>
具体的代码因为是个人项目，比较杂乱还有一堆BUG。实在羞于出手。<br/>
等以后项目稳定了会考虑开源客户端的部分代码<br/>

