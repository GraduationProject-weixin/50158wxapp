# [首页查询更多项目](https://github.com/GraduationProject-weixin) 包安装运行


# 50158wxapp停车场管理

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)]()


# 第1章 绪论
## 1.1 课题背景
随着移动互联形式的不断发展，各行各业都在摸索移动互联对本行业的改变，不断的尝试开发出适合于本行业或者本公司的APP。但是这样一来用户的手机上就需要安装各种软件，但是APP作为一个只为某个公司服务的一个软件，是一种闭环的生态，从用户获取和保持用户的粘性都变成了一个难题，并且在维护上面也需要考虑成本，慢慢的变成了不开发APP跟不上潮流，开发APP则运营上面步履维艰。如何获取一个新的客户来源通道以及转换通道，变成了管理者都需要面对的一个问题。如何让一个用户从已经习惯的应用里跳转到希望用户访问的应用里，这是一个问题，而微信小程序就解决了这样的难题。微信拥有庞大的用户基础，可以不用更换APP直接在微信上就可以访问用户想要访问的资源。因此微信小程序相对于APP来讲更受欢迎，本次课题就运用了微信小程序技术开发一个基于微信小程序的停车场管理系统。
## 1.2 课题意义 
背靠微信庞大用户群体的微信小程序，变成了当前解决用户访问应用程序入口方案的一种选择，用户的手机里面只要有微信，不需要安装新的软件，就可以直接访问指定目标，获取指定内容，解决了管理者的痛点，并且微信作为一个聊天工具，在微信里有支持的各种各样的生活服务，也为微信的用户提供了粘性，微信小程序不管是针对用户或者管理者都是一个双赢的存在。目前，传统电商及零售行业因为小程序的出现而获得了新生。本次课题针对停车场方面的信息，借助于微信小程序这样的平台，可以更加方便用户停放车辆，驶出车辆，支付停车费用。
## 1.3 研究内容
对基于微信小程序的停车场管理系统设计制作，不仅需要技术支撑，也需要大量的理论研究。本文在对基于微信小程序的停车场管理系统进行介绍时，将按照如下内容进行。

第一部分：介绍基于微信小程序的停车场管理系统研究的背景意义，便于用户了解系统；

第二部分：介绍开发基于微信小程序的停车场管理系统需要搭建的环境，包括技术和工具；

第三部分：介绍用户对基于微信小程序的停车场管理系统的功能要求，以及对基于微信小程序的停车场管理系统的性能要求等；

第四部分：介绍数据库的设计方案，以及根据功能要求设计的功能结构；

第五部分：介绍通过编码最终实现的系统功能运行效果；

第六部分：介绍系统的功能测试，对系统进行综合检测，并及时解决系统出现的问题，直至系统运行正常。
# 第2章 开发环境与技术
基于微信小程序的停车场管理系统的编码实现需要搭建一定的环境和使用相应的技术，接下来的内容就是对基于微信小程序的停车场管理系统用到的技术和工具进行介绍。
## 2.1 MYSQL数据库
本课题所开发的应用程序在数据操作方面是不可预知的，是经常变动的，没有办法直接把数据写在文档里，这样不仅仅不安全，也不能实现应用程序的功能。如果要能实现应用程序所需要的数据存储功能，就避免不了要进行专业数据库存储软件的选择。基本上应用程序实现的功能不算太复杂，市面上任何一个关系型数据库软件都可以实现。参考自己的学习进度和操作习惯来讲，Oracle数据库是适合的，但是所需要的的安装软件很大，并且有好多不需要的功能都是开启的状态，十分消耗电脑资源，所以没有选择Oracle数据库，而SQL Server数据库虽然学过，但是安装的时候因为电脑上可能有其他的软件存在，经常性的出问题，而安装问题不好解决就需要重新安装操作系统，这样对已经存在的软件来讲又是一种时间上的浪费。只有MySQL数据库，安装包小，安装速度快，操作简单，哪怕安装出问题也好解决，不用重装操作系统，也不影响电脑上运行的其他软件，消耗资源也少，最重要的是在功能方面完全的符合设计需要，所以最后选择了MySQL数据库作为应用软件开发需要的数据库。
## 2.2 JSP技术  
在动态网站的兴起之初，作为高级编程语言的Java自然不会放弃这个领域的蛋糕。Sun公司推出了Servlet作为输出动态网站的一种技术标准，虽然不怎么受当时程序员的喜爱，但是当初也没有太多的选择，随后几个月PHP语言问世，不考虑性能和效率如何，起码在书写网页所需要的动态代码块和静态代码块方面进行了区分，让书写效率和可读效率大大的提升，所以很多Java程序员以及刚入行的初级程序员都选择了PHP语言作为自己职业的发展方向，Sun公司为了维护Java语言在高级编程语言上的江湖地位，防止PHP继续抢走市场份额占有率，Sun公司联合Apache基金会研发了一个关于Java动态网页的一个新型的技术标准，这就是JSP技术。JSP吸取了PHP语言在页面书写上面的所有优点，但是又背靠Java EE的庞大后台，又能实现很多通过Java组件就能实现的功能，在JSP页面上可以直接引用那些组件，让JSP更加的强壮丰富。保证了Java技术纵向的可持续发展，并且在动态网站开发领域终于站稳了脚跟，其他PHP开发人员可以很快的转移到JSP进行开发，不考虑一些特殊组件或者功能的开发，只从动态页面的开发上来讲，完全实现了PHP程序和JSP程序的几乎无成本的转换，JSP技术就这样的发展了起来。
## 2.3 SSM框架
SSM框架不是一个框架的名称，而是三个框架的首字母缩写，分别是Spring框架、SpringMVC框架、MyBatis框架。是目前Java开发者中学习的首选框架。

Spring框架继承了JavaEE和EJB框架的优点，在依赖注入方面去掉了臃肿的配置，在面向切面方面也简化了代码数量，提高了代码品质。依赖注解进行配置，让所有的依赖都可以通过程序的自动配置和寻找，减少了代码写作数量，提高了代码阅读性。

SpringMVC框架与Spring只是一个公司的，在底层代码结构上可以复用，但是最主要的功能是对数据提交请求进行过滤，并且对数据的返回进行过滤，不限于页面是JSP技术，也可以是其他的技术，更容易大型开发的集合技术。

MyBatis框架摒弃了Hibernate框架的配置臃肿方面，有时候Hibernate框架业务比较复杂的时候，代码量反而增加，性能下降，无法对底层的数据库语句优化，而MyBatis框架则有效的解决了这个方面，可以通过Java语句，对数据库操作语句进行优化，代码更简洁，执行效率更高，并且可以生产一些模块化代码，解决了开发过程中容易出现的实体映射方面的操作。
## 2.4 微信开发者工具
微信web开发者工具是国内腾讯公司开发的专门用来开发微信小程序的一个工具。开发过程中如果是项目团队开发，可以设置多个开发和测试成员，管理员可以在小程序管理后台添加成员并且设置所需的权限。微信web开发者工具可以开发小程序项目以及微信公众号网页项目，小程序项目如果不部署到服务器上只做开发测试的话，AppID可以点击测试生成，否则需要在微信公众平台上申请微信公共号和微信小程序。用微信web开发者工具可以对程序与页面，组件和API进行调用，发布之前可以生成好几个小程序版本，并可以在后台查看运营相关数据。微信开发者工具是微信小程序开发的必备利器！


# 第3章 系统分析
面对即将开发的系统，进行提前的分析是必要的。这也是开发流程中必须有的环节。通常分析系统期间，主要涉及的内容包括系统开发可行性问题，对系统功能和性能的分析等问题。
## 3.1 可行性分析
在正式对需要建设的项目进行投资前，有一个比较关键的步骤是不能缺少的，那就是可行性分析。它主要从当前技术，经济等角度去评估系统的可行性，在投资决策中常常采用这种科学的方法来论证项目。
### 3.1.1 技术可行性
当前，系统开发的技术已经发展成熟，而且通过计算机网络可以获取开发工具的使用方法，以及规范化编写的模块化代码，这些知识可以帮助开发者顺利完成本系统的编码工作。
### 3.1.2 经济可行性
本系统开发期间需要配置的软件环境，可以免费通过开发类官网下载安装，需要配置的硬件设备也不需要具备很高的性能，通常网吧电脑，或学校计算机机房的电脑都符合要求。因此，从经济方面考虑，基于微信小程序的停车场管理系统开发可行。
### 3.1.3 操作可行性
基于微信小程序的停车场管理系统根据用户使用习惯进行开发，设计的界面具有统一性，并具备优秀的导航功能。所以，操作人员可以无压力操作基于微信小程序的停车场管理系统。

总之，从上述的论证来看，本系统可以开发。
## 3.2 系统流程
流程图这样的工具可以直观反映出系统内部的操作逻辑，可以帮助用户更好的理解系统。
### 3.2.1 操作流程
进入本系统需要访问者提供验证信息。验证合格的访问者才能获取访问资格。其具体的操作流程见下图。访问者根据登录界面设置的信息项如实填写，待信息通过验证后，访问者可以进入指定的页面享受本系统提供的服务和阅读本系统的相关信息。

![](/md/blog.001.png)

图3.1 操作流程图
### 3.2.2 登录流程
本系统的登录模块，其内部的流程见下图。主要对访问本系统的人员提供的验证信息进行逐个判断，系统面对录入错误的信息会给出提示，比如，提示账号不对，或提示密码不匹配等提示信息。总之，在登录页面填写的所有信息都符合要求，访问者就登录成功了。

![](/md/blog.002.png)

图3.2 登录流程图
### 3.2.3 删除信息流程
本系统在经常性的使用后，会产生很多失去价值的信息，因此就需要及时清理数据，腾出系统的空间。对这些数据进行清理时，其对应的流程见下图。先选中要清理的数据，通过反复确认需要清理的数据，避免操作人员误删。已经删除的数据就不会出现在系统里面。

![](/md/blog.003.png)

图3.3 删除信息流程图
### 3.2.4 添加信息流程
本系统主要用于显示信息，提供服务，其中，数据添加功能就是其中的服务之一，具体流程见下图。让操作者在信息添加的页面录入数据，待这些数据被提交检验合格后，就会在系统指定页面显示出来。

![](/md/blog.004.png)

图3.4 添加信息流程图
## 3.3 性能需求
进行需求分析，包括了根据用户实际需求制定功能，也涵盖了对即将设计的系统进行性能上的需求分析。所以一般分析系统时，一方面要分析系统功能，另一方面也要分析系统的性能。毕竟设计开发出一个好性能的系统可以确保系统的质量可靠。

接下来分析系统的性能，还要从界面友好性，系统的时间特性，系统的可靠性等方面来分析说明。

（1）系统的容量要求：对本系统完成数据处理的容量最大化进行确定。也就是确定系统处理数据的容量临界值，超过这个临界值，可能系统就运行不正常了。

（2）系统精度的要求：确定数据传输需要达到的精度值，也包括了数值计算的精度值，数据的精度值的设置等。

（3）时间特性要求：系统处理数据都有时间要求，这也是系统的时间特性。通常都会把数据处理的时间进行分析，也会设置用户请求的响应时间，还有系统在满负荷运行时可以偏离的范围数值等都需要提前分析确定。

（4）适应性要求：系统在面对系统环境的改变时，其自身适应这种变化的能力，也需要通过参数信息体现。比如说，在面对变化的需求，系统就要去适应这种变化，通过指出需要设计的过程或者是需要设计的软件来体现系统的适应性。

（5）界面友好性：除了功能上需要考虑用户需求外，在人机交互界面的设计上，也需要考虑用户的使用习惯，包括界面的布局，界面基调选择以及颜色搭配等。尽量做到用户在接受简单的培训之后，可以对系统进行独立操作。

（6）系统可靠性：对于初学者而言，很容易出现一个问题，就是设计开发的系统，因为人为的误操作出现崩溃，有些也会导致电脑死机。这样的现象也说明这种容错能力低下的系统是不可靠的。完全不能作为生活中处理信息的系统。当下，系统开发要保证可靠性，设计时，把模块化和结构化的设计理念也考虑进来。如果遇到对时效性要求比较严格的系统，也需要采取其它的措施，比如双机系统，还有磁盘阵列等方式。还有就是一个可靠性的系统，对设备的供电能力也有要求。

运行在计算机上的系统大都担负着信息处理的任务，对于它们而言，其性能要求有：完成信息查询，需要的响应时间；对终端设备的连接数量的确定；对存储数据的容量的安排；以及存储数据的可扩充的容量的设置，比如说系统存放近几个月，或者存放近几年的数据；完成报表打印数量的设置，也包括报表打印种类的设置等。
## 3.4 功能需求
不同的系统提供的服务也不相同，其对应的功能也不相同，所以，系统开工前，需要明确其用途，确定其功能。由此，才可以进行各个任务的开展。

基于微信小程序的停车场管理系统经过分析，确定了其需要设置管理员的角色，其操作的功能通过用例图展示（见下图）。管理员管理车位，审核车辆停放，车辆驶出以及停车费用信息。

![](/md/blog.005.png)

图3.5 管理员用例图

基于微信小程序的停车场管理系统经过分析，确定了其需要设置用户的角色，其操作的功能通过用例图展示（见下图）。用户查看车位，登记车辆停放信息以及车辆驶出信息，对停车费用进行支付。

![](/md/blog.006.png)

图3.6 用户用例图

# 第4章 系统设计
一个成功设计的系统在内容上必定是丰富的，在系统外观或系统功能上必定是对用户友好的。所以为了提升系统的价值，吸引更多的访问者访问系统，以及让来访用户可以花费更多时间停留在系统上，则表明该系统设计得比较专业。
## 4.1 设计原则
本系统在设计过程中需要依照一定的设计原则进行，目的就是为了让开发的系统具备高质量，齐全完备的功能，方便简单的操作，如此才可以最大限度的满足使用者的要求。系统设计原则除了基本的易操作原则，安全性原则外，还有准确性原则，实用性原则，可维护性原则。

第一个设计原则：易操作原则，针对本系统设计的功能要完备齐全，编码时，设计的各个接口要具备友好性，使用者一旦使用本系统时，要能够轻松上手，操作本系统处理数据时，要具备便利性。此外，也需要设计一些必要提示，引导使用者操作系统。

第二个设计原则：安全性原则，本系统在登录模块要对各个访问者进行身份验证，系统会通过访问者输入的信息进行判断，使用提前编写的安全验证代码进行数据比对，引导匹配成功的访问者进入指定的操作界面。这样可以避免无关性访问者窃取系统的数据。

第三个设计原则：准确性原则，为了保证使用者登记的数据是正确的，需要提前设计数据纠错机制，让使用者可以通过系统的报错提示，仔细检查登记的错误信息，并及时纠正错误，填写规范正确的信息。比如设置密码时，要求密码的长度不能低于6个字符，且数据类型要求不能全部是数字等都能进行规范。

第四个设计原则：实用性原则，本系统主要用于处理信息，在实际工作中，要帮助使用者完成信息处理任务，同时本系统在面对特殊情况时，也要能够满足信息处理的需要。另外，为了后期便于在本系统中进行功能的扩充，也需要提前预留好空间。

第五个设计原则：可维护性原则，本系统在实际使用期间，难免会遇到一些故障，因此，本系统在应对故障时，要能够进行诊断并弱化故障，可以在短时间内进行自维护。
## 4.2 功能结构设计
在前面分析的管理员功能的基础上，进行接下来的设计工作，最终展示设计的管理员结构图（见下图）。管理员管理车位，审核车辆停放，车辆驶出以及停车费用信息。

![](/md/blog.007.png)

图4.1 管理员功能结构图

在前面分析的用户功能的基础上，进行接下来的设计工作，最终展示设计的用户结构图（见下图）。用户查看车位，登记车辆停放信息以及车辆驶出信息，对停车费用进行支付。

![](/md/blog.008.png)

图4.2 用户功能结构图
## 4.3 数据库设计
开发一个系统也需要提前设计数据库。这里的数据库是相关数据的集合，存储在一起的这些数据也是按照一定的组织方式进行的。目前，数据库能够服务于多种应用程序，则是源于它存储方式最佳，具备数据冗余率低的优势。虽然数据库为程序提供信息存储服务，但它与程序之间也可以保持较高的独立性。总而言之，数据库经历了很长一段时间的发展，从最初的不为人知，到现在的人尽皆知，其相关技术也越发成熟，同时也拥有着坚实的理论基础。
### 4.3.1 数据库概念设计
这部分内容需要借助数据库关系图来完成，也需要使用专门绘制数据库关系图的工具，比如Visio工具就可以设计E-R图（数据库关系图）。设计数据库，也需要按照设计的流程进行，首先还是要根据需求完成实体的确定，分析实体具有的特征，还有对实体间的关联关系进行确定。最后才是使用E-R模型的表示方法，绘制本系统的E-R图。不管是使用亿图软件，还是Visio工具，对于E-R模型的表示符号都一样，通常矩形代表实体，实体间存在的关系用菱形符号表示，实体的属性也就是实体的特征用符号椭圆表示。最后使用直线将矩形，菱形和椭圆等符号连接起来。接下来就开始对本系统的E-R图进行绘制。

（1）下图是停车费用实体和其具备的属性。

![](/md/blog.009.png)

图4.4 停车费用实体属性图

（2）下图是车位实体和其具备的属性。

![](/md/blog.010.png)

图4.5 车位实体属性图

（3）下图是用户实体和其具备的属性。

![](/md/blog.011.png)

图4.6 用户实体属性图

4. 下图是管理员实体和其具备的属性。

![](/md/blog.012.png)

图4.7 管理员实体属性图

4. 下图为上述各实体间相互之间的关系。

![](/md/blog.013.png)

图4.8 实体间关系E-R图
### 4.3.2 数据库物理设计
本数据库是关系型数据库，因此对二维表的结构设计也比较关键。毕竟二维表格模型就是关系型数据库中的关系模型。而一些常用的关系模型中的概念也需要了解，才可以对关系模型进行设计。下面就简单介绍关系，元组，属性，域，关键字等常用概念的含义。

关系：关系就是数据库中的一张数据表，每张数据表都有命名，也就是每个关系也有名字，那就是数据表名；

元组：元组就是数据表中的一行记录；

属性：属性就是数据表中的字段，也就是数据表中的一列；

域：域就是对数据表中属性的取值进行限定；

关键字：关键字就是数据表中的主键；

在了解了表结构设计的常用概念后，接下来就需要使用前面绘制的E-R模型完成表结构的设计工作，并在数据库中创建数据表，并为各个数据表进行命名。以下就对设计的结果通过表格形式进行展示。

表4.1 车辆驶出信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|cheweibianhao|varchar(200)|是|NULL|车位编号|
|cheweimingcheng|varchar(200)|是|NULL|车位名称|
|xiaoshidanjia|int(11)|是|NULL|小时单价|
|likaishijian|date|是|NULL|离开时间|
|tupian|varchar(200)|是|NULL|图片|
|zhanghao|varchar(200)|是|NULL|账号|
|shouji|varchar(200)|是|NULL|手机|
|sfsh|varchar(200)|是|否|是否审核|
|shhf|longtext|是|NULL|审核回复|
|userid|bigint(20)|是|NULL|用户id|
表4.2 车辆停放信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|cheweibianhao|varchar(200)|是|NULL|车位编号|
|cheweimingcheng|varchar(200)|是|NULL|车位名称|
|xiaoshidanjia|int(11)|是|NULL|小时单价|
|tingfangshijian|date|是|NULL|停放时间|
|beizhu|longtext|是|NULL|备注|
|tupian|varchar(200)|是|NULL|图片|
|zhanghao|varchar(200)|是|NULL|账号|
|shouji|varchar(200)|是|NULL|手机|
|sfsh|varchar(200)|是|否|是否审核|
|shhf|longtext|是|NULL|审核回复|
|userid|bigint(20)|是|NULL|用户id|




表4.3 车位信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|cheweibianhao|varchar(200)|是|NULL|车位编号|
|cheweimingcheng|varchar(200)|否||车位名称|
|weizhi|varchar(200)|是|NULL|位置|
|cheweizhuangtai|varchar(200)|是|NULL|车位状态|
|xiaoshidanjia|int(11)|是|NULL|小时单价|
|tingfangxuzhi|longtext|是|NULL|停放须知|
|beizhu|longtext|是|NULL|备注|
|tupian|varchar(200)|是|NULL|图片|
表4.4 停车场公告信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|biaoti|varchar(200)|是|NULL|标题|
|gonggaoneirong|longtext|是|NULL|公告内容|
|faburen|varchar(200)|是|NULL|发布人|
|fabushijian|date|是|NULL|发布时间|
|tupian|varchar(200)|是|NULL|图片|
表4.5 停车费用信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|chepaihao|varchar(200)|是|NULL|车牌号|
|cheliangpinpai|varchar(200)|是|NULL|车辆品牌|
|cheweibianhao|varchar(200)|是|NULL|车位编号|
|jinrushijian|datetime|是|NULL|进入时间|
|likaishijian|datetime|是|NULL|离开时间|
|tingcheshizhang|int(11)|是|NULL|停车时长|
|xiaoshidanjia|int(11)|是|NULL|小时单价|
|zongjia|varchar(200)|是|NULL|总价|
|beizhu|longtext|是|NULL|备注|
|tupian|varchar(200)|是|NULL|图片|
|zhanghao|varchar(200)|是|NULL|账号|
|shouji|varchar(200)|是|NULL|手机|
|sfsh|varchar(200)|是|否|是否审核|
|shhf|longtext|是|NULL|审核回复|
|ispay|varchar(200)|是|未支付|是否支付|
|userid|bigint(20)|是|NULL|用户id|
表4.6 管理员信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|username|varchar(100)|否||用户名|
|password|varchar(100)|否||密码|
|role|varchar(100)|是|管理员|角色|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|新增时间|
表4.7 用户信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|创建时间|
|zhanghao|varchar(200)|否||账号|
|mima|varchar(200)|否||密码|
|xingming|varchar(200)|否||姓名|
|xingbie|varchar(200)|是|NULL|性别|
|shouji|varchar(200)|是|NULL|手机|
|youxiang|varchar(200)|是|NULL|邮箱|
|shenfenzheng|varchar(200)|是|NULL|身份证|
|tupian|varchar(200)|是|NULL|图片|
![打开新的 phpMyAdmin 窗口](/md/blog.014.png "打开新的 phpMyAdmin 窗口")


# 第5章 系统实现
进入到这个环节，也就可以及时检查出前面设计的需求是否可靠了。一个设计良好的方案在运用于系统实现中，是会帮助系统编制人员节省时间，并提升开发效率的。所以在系统的编程阶段，也就是系统实现阶段，对于一些不合理的设计需求，也是可以及时发现。因为设计的方案是完全指导系统的编码过程的。
## 5.1 管理员功能实现
### 5.1.1 车辆停放管理
管理员进入指定功能操作区之后可以管理车辆停放信息。其页面见下图。管理员审核车辆停放信息，查询车辆停放信息。

![](/md/blog.015.png)

图5.1 车辆停放管理页面
### 5.1.2 车辆驶出管理
管理员进入指定功能操作区之后可以管理车辆驶出信息。其页面见下图。管理员审核车辆驶出信息，查询车辆驶出信息。

![](/md/blog.016.png)

图5.2 车辆驶出管理页面
### 5.1.3 停车费用管理
管理员进入指定功能操作区之后可以管理停车费用信息。其页面见下图。管理员审核停车费用信息，修改，删除停车费用信息。

![](/md/blog.017.png)

图5.3 停车费用管理页面
### 5.1.4 车位信息管理
管理员进入指定功能操作区之后可以管理车位信息。其页面见下图。管理员增删改查车位信息，查看车位目前状态是否为空闲状态。

![](/md/blog.018.png)

图5.4 车位信息管理页面
## 5.2 用户功能实现
### 5.2.1 车位信息
用户进入指定功能操作区之后可以查看车位信息。其页面见下图。用户查看车位信息，可以在页面右下角点击停放登记按钮登记车辆停放信息。

![](/md/blog.019.png)

图5.6 车位信息页面
### 5.2.2 车辆停放
用户进入指定功能操作区之后可以查看车辆停放信息。其页面见下图。用户查看车辆停放，查看管理员审核信息，可以点击页面右下角的驶出登记按钮登记车辆驶出信息。

![](/md/blog.020.png)

图5.7 车辆停放页面
### 5.2.3 停车费用
用户进入指定功能操作区之后可以查看停车费用信息。其页面见下图。用户查看停车费用信息，对停车费用进行支付。

![](/md/blog.021.png)

图5.8 停车费用页面


# 










