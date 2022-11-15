## 一、下载与安装：
- 官网：[https://jmeter.apache.org/](https://jmeter.apache.org/)
- 下载：[https://jmeter.apache.org/download_jmeter.cgi](https://jmeter.apache.org/download_jmeter.cgi)

下载之后解压缩，通过 `bin/ApacheJMeter.jar` 启动。
#1024程序员节｜用代码，改变世界#

## 二、测试流程
1. 添加线程组
  - 设置名称、线程数、循环次数等
![image.png](https://img-blog.csdnimg.cn/img_convert/d7b5ba3f8634994a8a8f28fff88ae8b2.png)
![image.png](https://img-blog.csdnimg.cn/img_convert/0aa7d3ff175631ccdb0bcc63c8de85cb.png)

2. 添加http请求默认值
  - 如：协议、域名、端口、固定参数等
![image.png](https://img-blog.csdnimg.cn/img_convert/088193f85af09903e482ca4d8a8b16ed.png)
![image.png](https://img-blog.csdnimg.cn/img_convert/467a6c1f23493b4763cdb5029b1916b3.png)

3. 添加http请求默认header
  - cookie也可以通过**配置原件HTTP Cookie管理器**添加
![image.png](https://img-blog.csdnimg.cn/img_convert/6de0aa81e0366b557535b94c24743e4c.png)
![image.png](https://img-blog.csdnimg.cn/img_convert/c44383cb0a2e88090f5b8a8179786314.png)

4. 添加取样器Sampler
  - 在取样器设置需要测试的接口
  - 可以添加插件以支持其他类型的请求，比如dubbo
![image.png](https://img-blog.csdnimg.cn/img_convert/8dac198f095aff54002c15db723e8cf4.png)
![image.png](https://img-blog.csdnimg.cn/img_convert/cd8d39a94be34bc404364aa7d76247ba.png)

5. 查看结果
  - 监听器  
    - 查看结果树
    ![image.png](https://img-blog.csdnimg.cn/img_convert/9715290b49c9cc65f6f43b9ec6c82418.png)

6. 启动测试
  - 点击启动按钮
  - 查看结果树
![image.png](https://img-blog.csdnimg.cn/img_convert/b65388a289ab5b8c31178c093fad08d6.png)
- 可以看到我们设置的http请求默认值已经生效
- 可以看到运行了10次，这跟线程组的设置有关
- 可以查看每次请求的结果
![image.png](https://img-blog.csdnimg.cn/img_convert/422e32723a9e40f530b22917aa6c7997.png)
![image.png](https://img-blog.csdnimg.cn/img_convert/9adae1384ced5b592dfe1dcc0076385f.png)