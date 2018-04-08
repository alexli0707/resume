# 联系方式
- 手机：  	18650775717
- Email：	lixinforlove@gmail.com
- QQ：   	451398240

---

# 个人信息

 - 李歆/男/1988 07 07
 - 教育:本科/集美大学 数学与应用数学(2006-2010)
 - 工作年限：7年
 - Github：https://github.com/alexli0707
 - 期望职位：服务端工程师/架构人员
 - 技能语言: Java,PHP, Python


---

# 工作经历
- 福州新游互联(2016年1月-至今) : 服务端负责人(Python，PHP),负责项目架构,后台,客户端API接口开发.
- 福州新游互联(2014年3月-2015年10月) : Android应用开发工作，负责Push和IM的客户端sdk开发以及新游部落社区开发.
- 中国网龙(2012年7月-2014年3月) : Android应用开发.

# 技能清单
- 熟练善于带领团队完成服务端项目以及对整体技术架构有一定的把控经验,能够完成一般规模项目的基础架构与设计.
- Java Spring Boot套餐服务端研发,对于微服务有一定了解以及兴趣.
- 熟悉使用python,熟悉使用flask + Nginx + uWSGI+gevent的后端开发.熟悉使用Scrapy 完成一般爬虫业务.能使用Redis完成一般场景业务(cache,运算等等).
- 熟悉使用PHP + Laravel + Nginx 进行服务端项目开发.
- 能完成一般功能的后端前台开发.用过的构建方式有seajs,requirejs,基于AdminLTE以及bootstrap上与jinja2模板的共同前台开发.html,css,js 技能水平一般.
- 熟练掌握Android常规应用开发中所需技能
- 对于面向对象程序开发以及设计模式有充分的实践以及继续学习的热情，良好的编码风格以及文档编写能力
- 熟悉Android手机软件的一般开发模式、开发步骤、模块划分及集成
- 良好的单元测试编写能力以及热衷于对项目开发可持续交付的实践
- 掌握项目代码静态审查 以及Android CI 实践
- 对于敏捷开发有一定的学习和实践
- 对于产品体验性能优化有较为丰富的实践经验以及热情

# 自我评价

- 热爱coding,热爱工作,热爱生活.

---

# 项目经验
### 微信多功能红包小程序(PHP):
- 项目描述: 微信红包小程序,有4种发红包的玩法
- 运行平台：Centos6.6 +PHP7.1 +Laravel + swoole
- 工作内容：
			负责项目设计架构以及框架搭建,红包种类逻辑与流程的扩展.抢红包以及语音红包识别的流程设计优化.后台内容大约在一个半月内从开发到性能调优到上架.
- 技术要点:
		
		1.抢红包操作的原子性问题以及幂等设计原则的考虑,利用redis与lua脚本实现用户抢红包场景的速度与一致性优化.
		2.redis哨兵模式以及采用zabbix进行线上服务监控.
		3.语音识别调用百度api时本地转码以及等待反馈时长问题导致接口耗时约为3s-5s的情况下为避免拖垮php-fpm采用swoole协程的方式尽可能hold住更多的链接,如果线上语音识别服务被拖垮也不会导致红包主服务被拖垮.	
			
			
- IDE以及版本控制：PhpStorm + Git.


### 电竞助手&新游部落(Python):
- 项目描述: 官网(http://www.newgamer.com/),为移动端提供api接口以及为项目提供管理后台.
- 运行平台：Centos6.6 +python2.7+ virtualenv+ uWSGI + Flask + Nginx + Mysql + Redis
- 工作内容：
			负责该项目版本开发业务实现,通过Sentry为项目提供线上状态实时监控,以及使用goaccess分析优化慢接口并进行后续优化.同时也负责业务需求与任务拆分工作.通过多分支并行的方式对之前项目做着部分优化以及新业务的开发.使用爬虫爬取热门游戏的攻略文章内容,为编辑运营人员提供便捷的信息资源.由于线上有两台机器以及存储使用独立的rds,暂时没有遇到业务的bottleneck所以很遗憾准备了一些优化方案没有实施.搭建Pypi私有库抽象工具库方便各个项目统一调用. 将oss从原先自建实例上转移到阿里云oss,为公司节约两台大容量存储的线上实例成本.
			
- IDE以及版本控制：PyCharm + Git.

### 八爪鱼(Python):
- 项目描述: 为与个推联运提供支持的项目,预先在后台通过模板填入相关数据,产生游戏或者应用的推广模板,比如这个(https://bzy.newgamer.com/m/themes/10000000000055),提供游戏相关攻略以及下载
- 运行平台：Centos6.6 +python2.7+ virtualenv+ uWSGI + Flask + Nginx + Mysql + Redis
- 技术要点：
			
			1.用户场景比一般场景特殊一些,个推的活动都是在高峰时段大量的进行推送,往往在半个小时的时间片内,会产生几万到十几万次的请求.第一次进行ab压测的时候暴露出生成模板的一些问题,比如图片动态处理,cdn预热,以及内部执行mysql的业务逻辑等等,通过优化调整后上线满足业务压力.
			2.发现各大手机浏览器以及运营商存在对下载包的劫持问题,然后通过与cdn厂商的协作来解决.
			
			
- IDE以及版本控制：PyCharm + Git.

### 新游游戏中心(PHP):
- 项目描述: 提供联运服务,为android以及h5应用与游戏商提供接入的入口以及指导,同时根据权限暴露对应数据(http://open.newgame.com/)
- 运行平台：Centos6.6  + php5.6 + laravel 5.3 + mysql +redis +apache +docker + composer+ gulp
- 工作内容：通过自学比对yii2以及laravel还有几个主流框架之后选型Laravel后进行功能的实现.亮点几乎没有,不过在使用中发现一些laravel框架上的亮点后在flask现有框架上进行了实现.
			
			
- IDE以及版本控制：PhpStorm + Git.

### 新游部落(Android):
- 项目描述: 移动门户应用,提供最新最热游戏资讯动态,可供用户下载以及预约	       游戏.还包括游戏社区功能.
- 运行平台： Android 4.0及以上
- 技术要点：
			
			1.RecycleView SwipeRefreshLayout CardView等Android Material Design的使用
			2.便捷性开发框架的搭建（Retrofit+Rxjava+ lambda）
  	        3.下载与更新
			4.动画效果运用以及UI表现优化
			
- IDE以及版本控制：AndroidStudio + Git.

### GameService SmartPush(智能推送,Android):
- 项目描述: 通过用户数据分析挖掘，为开发者定义用户群体。根据实际运营目的，做真正意义上的精确化推送；通过图表清晰对比每一次的推送的效果，每一个节点游戏数据的变化尽在掌控之中。推送（数据指标）、游戏内IM、玩家P2P社交等，紧紧围绕游戏而设计，增强游戏黏性.
- 运行平台： Android 2.2及以上
- 技术要点：
			
			1.TCP长连接的维护
			2.私有协议的设计
			3.本地数据采集缓存策略以及上报策略
			4.Android后台Service维护
            5.SDK动态升级功能

- IDE以及版本控制：AndroidStudio + Git.

### GameService IM SDK(Android):
- 项目描述: 提供开放式Api的IM SDK
- 运行平台： Android 2.2及以上
- 技术要点：
			
			1.用户在线和离线之间的连接通道切换维护

### 91UP系列(Android):
- 项目描述: 教育项目，满足用户移动端线上做题的需求，包含公务员考试、会计从业、司法考试、建造师考试等等热门教育应用，一次开发，多版本打包，目前已累积千万用户量.
- 运行平台： Android 2.2及以上
- 技术要点：
			
			1.Android UI控件的扩展和自定义
		    2.Fragments之间的通信
	        3.多版本打包发布
            4.缓存优化以及本地数据存储与展示策略

### 非学历教育应用App(Android):
- 项目描述: 国家教育部指定项目-全国非学历教育项目手机端Android版本，帮助用户利用移动端完成学历教育，有课程做题练习，文档阅读以及视频学习.
- 运行平台： Android 2.2及以上
- 技术要点：
			
			1.Sonartype Nexus + Maven内部代码服务器部署，有效解决项目依赖问题
            2.SonarQube 代码审查，保证代码质量
			3.Jenkins 持续集成保证
			4.Android应用性能优化以及后台被强制结束后恢复应用场景相关
			5.本地和在线视频播放
			6.PDF文档阅读
		    7.下载中心
			8.离线模式的开发



---



# 个人相关
Github:[https://github.com/alexli0707](https://github.com/alexli0707)

掘金:[https://juejin.im/user/5848f66ea22b9d0058c79a09](https://juejin.im/user/5848f66ea22b9d0058c79a09)

简书:[http://www.jianshu.com/u/7ec88af44b3b](http://www.jianshu.com/u/7ec88af44b3b)

 
 ---

# 致谢
感谢您花时间阅读我的简历,期待能有机会和您共事.
