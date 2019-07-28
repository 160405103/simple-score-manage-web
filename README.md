# simple-score-manage-web
Mini Web网站设计与实现 
1.实现用户注册和登录功能，注册或登录成功，则返回成绩管理页面
2.登录成功写入session，注销、退出或session过期则删除该session 
3.完善成绩管理页面，可以修改或删除成绩记录
页面布局：主要使用BootStrap的CSS布局。
工程名字: jsp
主要页面：index.jsp   regist.jsp   gradetable.jsp
服务端处理：Table  Userbean  TableDaoImpl     DataBaseUtil
LoginServlet  LogoutServlet
TableAddServlet  TableDeleteServlet  TableMoifyServlet   TableSerchServlet
设计思想：MVC    domain建立User ,Table的用户模型，同时Dao层实现对用户模型的数据库操作；controller实现后台逻辑，比如登陆成功跳转首页、登陆失败跳转失败页面等逻辑过程的具体实现，最后jsp文件作为展示页面。其中成绩的显示这块用了jstl的sql标签。
功能：用户注册登陆，进入成绩表页面，可以删除，修改，增加，查询成绩。修改成绩会出现模态框。通过session判断当前是否已经是登陆状态。
