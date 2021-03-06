# Servlet、JSP和Spring MVC初学指南

过了一遍代码，打算将代码改造成为采用最新版Spring Boot的实现。因为Spring Boot默认自带内嵌式Tomcat，这样省去安装和配置Tomcat的步骤，上手更快。工程使用Maven多模块的方式管理，每个子模块对应原来书的代码的一个按章节区分的工程代码。顶层工程名为：servlet-jsp-springmvc-demos，避免与原来作者的示例代码目录相同，容易搞混淆。

![书籍封面](https://img1.doubanio.com/view/subject/l/public/s29287879.jpg)

本书是Servlet、JSP 和Spring MVC 的入门教程，是畅销图书《Spring MVC 学习指南》的姊妹篇。  
Servlet 和JSP 是Java Web 应用开发的底层技术，而Spring MVC 是Spring 框架中用于解决Servlet 和JSP 应用开发的常见和通用问题的一个模块。Spring MVC 是一个广泛应用于GUI 开发的设计模式，是目前业界主流的Web 开发框架，也是一种热门的开发技能。本书分两大部分，详细介绍了Servlet 和JSP 的核心技术，以及Spring MVC 的实践应用。对于期望学习如何应用Servlet、JSP 以及Spring MVC 来开发Java Web 应用的初学者来说，本书是一本非常理想的初学指南。  

**内容简介:**  
Servlet和JSP是开发Java Web应用程序的两种基本技术。Spring MVC是Spring框架中用于Web应用快速开发的一个模块，是当今流行的Web开发框架之一。本书是Servlet、JSP和Spring MVC的学习指南。全书内容分为两个部分，首部分主要介绍Servlet和JSP基础知识和技术，包括第1章至第15章；第2部分主要介绍Spring MVC，包括第16章至第24章。附录部分给出了Tomcat安装和配置指导，还介绍了Servlet and JSP注解以及SSL证书。本书内容充实、讲解清晰，非常适合Web开发者尤其是基于Java的Web应用开发者阅读。  

## 目录

### 第一部分　Servlets和JSP  

第1章　Servlets　3  
1．1　Servlet API概览　3  
1．2　Servlet　4  
1．3　编写基础的Servlet应用程序　5  
1．3．1　编写和编译Servlet类　5  
1．3．2　应用程序目录结构　7  
1．3．3　调用Servlet　8  
1．4　ServletRequest　8  
1．5　ServletResponse　9  
1．6　ServletConfig　9  
1．7　ServletContext　12  
1．8　GenericServlet　12  
1．9　Http Servlets　14  
1．9．1　HttpServlet　15  
1．9．2　HttpServletRequest　16  
1．9．3　HttpServletResponse　16  
1．10　处理HTML表单　17  
1．11　使用部署描述符　22  
1．12　小结　24  
第2章　会话管理　25  
2．1　URL重写　25  
2．2　隐藏域　30  
2．3　Cookies　34  
2．4　HttpSession对象　41  
2．5　小结　49  
第3章　JavaServer Pages(JSP)　50  
3．1　JSP概述　50  
3．2　注释　54  
3．3　隐式对象　55  
3．4　指令　58  
3．4．1　page指令　58  
3．4．2　include指令　59  
3．5　脚本元素　60  
3．5．1　表达式　61  
3．5．2　声明　61  
3．5．3　禁用脚本元素　64  
3．6　动作　65  
3．6．1　useBean　65  
3．6．2　setProperty和getProperty　66  
3．6．3　include　67  
3．6．4　forward　67  
3．7　错误处理　67  
3．8　小结　68  
第4章　表达式语言　69  
4．1　表达式语言的语法　69  
4．1．1　关键字　70  
4．1．2　[ ]和．运算符　70  
4．1．3　取值规则　71  
4．2　访问JavaBean　71  
4．3　EL隐式对象　72  
4．3．1　pageContext　72  
4．3．2　initParam　73  
4．3．3　param　73  
4．3．4　paramValues　73  
4．3．5　header　74  
4．3．6　cookie　74  
4．3．7　applicationScope、sessionScope、requestScope和pageScope　74  
4．4　使用其他EL运算符　75  
4．4．1　算术运算符　75  
4．4．2　逻辑运算符　75  
4．4．3　关系运算符　76  
4．4．4　empty运算符　76  
4．5　应用EL　76  
4．6　如何在JSP 2．0及其更高版本中配置EL　80  
4．6．1　实现免脚本的JSP页面　80  
4．6．2　禁用EL计算　80  
4．7　小结　81  
第5章　JSTL　82  
5．1　下载JSTL　82  
5．2　JSTL库　82  
5．3　一般行为　83  
5．3．1　out标签　83  
5．3．2　set标签　84  
5．3．3　remove标签　86  
5．4　条件行为　86  
5．4．1　if标签　87  
5．4．2　choose、when和otherwise标签　88  
5．5　遍历行为　89  
5．5．1　forEach标签　89  
5．5．2　forTokens标签　96  
5．6　与URL相关的行为　97  
5．6．1　url标签　97  
5．6．2　redirect标签　98  
5．7　格式化行为　99  
5．7．1　formatNumber标签　99  
5．7．2　formatDate标签　101  
5．7．3　timeZone标签　102  
5．7．4　setTimeZone标签　103  
5．7．5　parseNumber标签　104  
5．7．6　parseDate标签　104  
5．8　函数　106  
5．8．1　contains函数　106  
5．8．2　containsIgnoreCase函数　106  
5．8．3　endsWith函数　106  
5．8．4　escapeXml函数　107  
5．8．5　indexOf函数　107  
5．8．6　join函数　107  
5．8．7　length函数　107  
5．8．8　replace函数　108  
5．8．9　split函数　108  
5．8．10　startsWith函数　108  
5．8．11　substring函数　108  
5．8．12　substringAfter函数　109  
5．8．13　substringBefore函数　109  
5．8．14　toLowerCase函数　109  
5．8．15　toUpperCase函数　109  
5．8．16　trim函数　109  
5．9　小结　110  
第6章　自定义标签　111  
6．1　自定义标签概述　111  
6．2　简单标签处理器　112  
6．3　SimpleTag示例　112  
6．3．1　编写标签处理器　113  
6．3．2　注册标签　114  
6．3．3　使用标签　114  
6．4　处理属性　115  
6．5　访问标签内容　118  
6．6　编写EL函数　120  
6．7　发布自定义标签　122  
6．8　小结　124  
第7章　标签文件　125  
7．1　Tag File简介　125  
7．2　第一个Tag File　126  
7．3　Tag File指令　127  
7．3．1　tag指令　127  
7．3．2　include指令　128  
7．3．3　taglib指令　130  
7．3．4　attribute指令　131  
7．3．4　variable指令　132  
7．4　doBody　134  
7．5　invoke　137  
7．6　小结　138  
第8章　监听器　139  
8．1　监听器接口和注册　139  
8．2　Servlet Context监听器　140  
8．2．1　ServletContextListener　140  
8．2．2　ServletContextAttribute Listener　142  
8．3　Session Listeners　142  
8．3．1　HttpSessionListener　142  
8．3．2　HttpSessionAttribute Listener　145  
8．3．3　HttpSessionActivation Listener　145  
8．3．4　HttpSessionBinding Listener　146  
8．5　ServletRequest Listeners　147  
8．5．1　ServletRequest Listener　147  
8．5．2　ServletRequestAttribute Listener　149  
8．6　小结　149  
第9章　Filters　150  
9．1　Filter API　150  
9．2　Filter配置　151  
9．3　示例1：日志Filter　153  
9．4　示例2：图像文件保护Filter　156  
9．5　示例3：下载计数Filter　158  
9．6　Filter顺序　162  
9．7　小结　162  
第10章　修饰Requests及Responses　163  
10．1　Decorator模式　163  
10．2　Servlet封装类　164  
10．3　示例：AutoCorrect Filter　165  
10．4　小结　172  
第11章　异步处理　173  
11．1　概述　173  
11．2　编写异步Servlet和过滤器　173  
11．3　编写异步Servlets　174  
11．4　异步监听器　179  
11．5　小结　181  
第12章　安全　182  
12．1　身份验证和授权　182  
12．1．1　指定用户和角色　183  
12．1．2　实施安全约束　184  
12．2　身份验证方法　185  
12．2．1　基于表单的认证　189  
12．2．2　客户端证书认证　192  
12．3　安全套接层　192  
12．3．1　密码学　192  
12．3．2　加密/解密　193  
12．3．3　认证　193  
12．3．4　数据的完整性　195  
12．3．5　SSL是怎么工作的　195  
12．4　编程式安全　196  
12．4．1　安全注释类型　196  
12．4．2　Servlet的安全API　197  
12．5　总结　199  
第13章　部署　200  
13．1　概述　200  
13．1．1　核心元素　202  
13．1．2　context-param　202  
13．1．3　distributable　202  
13．1．4　error-page　202  
13．1．5　filter　203  
13．1．6　filter-mapping　204  
13．1．7　listener　204  
13．1．8　locale-encoding-mapping-list和locale-encoding-mapping　204  
13．1．9　login-config　205  
13．1．10　mime-mapping　205  
13．1．11　security-constraint　206  
13．1．12　security-role　207  
13．1．13　Servlet　207  
13．1．14　servlet-mapping　209  
13．1．15　session-config　209  
13．1．16　welcome-file-list　209  
13．1．17　JSP-Specific Elements　210  
13．1．18　taglib　210  
13．1．19　jsp-property-group　210  
13．2　部署　212  
13．3　web fragment　212  
13．4　小结　214  
  
### 第二部分　Spring mvc  

第14章　动态加载及Servlet容器加载器　217  
14．1　动态加载　217  
14．2　Servlet容器加载器　220  
14．3　小结　222  
第15章　Spring框架　223  
15．1　Spring入门　223  
15．2　依赖注入　223  
15．3　XML配置文件　226  
15．4　Spring控制反转容器的使用　226  
15．4．1　通过构造器创建一个bean实例　226  
15．4．2　通过工厂方法创建一个bean实例　227  
15．4．3　Destroy Method的  
使用　227  
15．4．4　向构造器传递参数　228  
15．4．5　setter方式依赖注入　229  
15．4．6　构造器方式依赖  
注入　231  
15．5　小结　232  
第16章　模型2和MVC模式　233  
16．1　模型1介绍　233  
16．2　模型2介绍　233  
16．3　模型2之Servlet控制器　234  
16．3．1　Product类　236  
16．3．2　ProductForm类　237  
16．3．3　ControllerServlet类　238  
16．3．4　视图　241  
16．3．5　测试应用　243  
16．4　解耦控制器代码　243  
16．5　校验器　247  
16．6　后端　251  
16．7　小结　252  
第17章　Spring MVC介绍　253  
17．1　采用Spring MVC的好处　253  
17．2　Spring MVC的DispatcherServlet　254  
17．3　Controller接口　255  
17．4　第一个Spring MVC应用　255  
17．4．1　目录结构　255  
17．4．2　部署描述符文件和SpringMVC配置文件　256  
17．4．3　Controller　257  
17．4．4　View　259  
17．4．5　测试应用　260  
17．5　View Resolver　261  
17．6　小结　263  
第18章　基于注解的控制器　264  
18．1　Spring MVC注解类型　264  
18．1．1　Controller注解类型　264  
18．1．2　RequestMapping  
注解类型　265  
18．2　编写请求处理方法　267  
18．3　应用基于注解的控制器　269  
18．3．1　目录结构　269  
18．3．2　配置文件　270  
18．3．3　Controller类　272  
18．3．4　View　273  
18．3．5　测试应用　274  
18．4　应用@Autowired和@Service进行依赖注入　275  
18．5　重定向和Flash属性　278  
18．6　请求参数和路径变量　279  
18．7　@ModelAttribute　281  
18．8　小结　282  
第19章　数据绑定和表单标签库　283  
19．1　数据绑定概览　283  
19．2　表单标签库　284  
19．2．1　form标签　284  
19．2．2　input标签　285  
19．2．3　password标签　286  
19．2．4　hidden标签　287  
19．2．5　textarea标签　287  
19．2．6　checkbox标签　287  
19．2．7　radiobutton标签　288  
19．2．8　checkboxes标签　288  
19．2．9　radiobuttons标签　289  
19．2．10　select标签　290  
19．2．11　option标签　290  
19．2．12　options标签　291  
19．2．13　errors标签　291  
19．3　数据绑定范例　292  
19．3．1　目录结构　292  
19．3．2　Domain类　293  
19．3．3　Controller类　294  
19．3．4　Service类　295  
19．3．5　配置文件　298  
19．3．6　视图　299  
19．3．7　测试应用　301  
19．4　小结　302  
第20章　转换器和格式化　303  
20．1　Converter　303  
20．2　Formatter　307  
20．3　用Registrar注册Formatter　310  
20．4　选择Converter，还是Formatter　312  
20．5　小结　312  
第21章　验证器　313  
21．1　验证概览　313  
21．2　Spring验证器　314  
21．3　ValidationUtils类　315  
21．4　Spring的Validator范例　316  
21．5　源文件　317  
21．6　Controller类　318  
21．7　测试验证器　319  
21．8　JSR 303验证　320  
21．9　JSR 303 Validator范例　322  
21．10　小结　323  
第22章　国际化　324  
22．1　语言区域　324  
22．2　国际化Spring MVC应用程序　326  
22．2．1　将文本元件隔离成属性文件　326  
22．2．2　选择和读取正确的属性文件　328  
22．3　告诉Spring MVC使用哪个语言区域　329  
22．4　使用message标签　329  
22．5　范例　330  
22．6　小结　334  
第23章　上传文件　335  
23．1　客户端编程　335  
23．2　MultipartFile接口　336  
23．3　用Commons FileUpload  
上传文件　336  
23．4　Domain类　337  
23．5　控制器　338  
23．6　配置文件　340  
23．7　JSP页面　341  
23．8　应用程序的测试　343  
23．9　用Servlet 3．0及其更高版本上传文件　344  
23．10　客户端上传　347  
23．11　小结　355  
第24章　下载文件　356  
24．1　文件下载概览　356  
24．2　范例1：隐藏资源　357  
24．3　范例2：防止交叉引用　360  
24．4　小结　363  
附录A　Tomcat　364  
A．1　下载和配置Tomcat　364  
A．2　启动和终止Tomcat　364  
A．3　定义上下文　365  
A．4　定义资源　366  
A．5　安装SSL证书　366  
附录B　Web Annotations　368  
B．1　HandlesTypes　368  
B．2　HttpConstraint　368  
B．3　HttpMethodConstraint　369  
B．4　MultipartConfig　369  
B．5　ServletSecurity　370  
B．6　WebFilter　370  
B．7　WebInitParam　371  
B．8　WebListener　371  
B．9　WebServlet　371  
附录C　SSL证书　372  
C．1　证书简介　372  
C．2　KeyTool　373  
C．2．1　生成密钥对　373  
C．2．2　获得认证　374  
C．2．3　将证书导入到密钥库　375  
C．2．4　从密钥库导出证书　375  
C．2．5　列出密钥库条目　375
