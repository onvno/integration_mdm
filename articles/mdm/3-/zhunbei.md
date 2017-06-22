# 操作准备

## 新增帐套

登录系统管理地址：http://服务器IP（或服务器名称）:端口/portal/admin.jsp。

以超级管理员root 登录，默认密码为空。系统强制要求修改root的登录密码。登录进去之后点击【系统管理】节点，新增系统，填写系统编码、系统名称、生效日期、失效日期、数据源选择在中间件配置工具中设置的数据源、主语种、系统管理员等信息，点击〖保存〗按钮。

![](/articles/mdm/3-/images/image2.png)

图：建系统管理员

单击〖升级系统〗，进入建库向导页：

![](/articles/mdm/3-/images/image3.png)

图：建库向导

选择待安装产品，点击〖下一步〗按钮，进入数据库初始化过程，点击〖开始安装〗，开始安装数据库，安装完成后，需要重启中间件。

## 系统管理员登录

用系统管理员登录http://服务器IP（或服务器名称）:端口/portal。

→ 新增集团

点击【应用系统管理】→【系统初始化】→【集团管理】，新增集团：

![](/articles/mdm/3-/images/image4.png)

图：新增集团

→ 业务初始化

点击【应用系统管理】→【系统初始化】→【业务初始化】，选择模块进行初始化：

![](/articles/mdm/3-/images/image5.png)

图：业务初始化

→ 新增集团管理员

点击【应用系统管理】→【系统初始化】→【集团管理员】，新增集团管理员:

![](/articles/mdm/3-/images/image6.png)

图：集团管理员

## 集团管理员登录

Portal的登录地址：http://服务器IP（或服务器名称）:端口/portal

用创建的集团管理员身份登录（默认密码为yonyou00，登录时系统会强制进行修改），登录后的界面如下图所示。普通用户默认密码也是yonyou00。

![](/articles/mdm/3-/images/image7.png)

图：主数据管理首页

