<p align="center">
<img width="1440" height="280" alt="github_banner_white" src="https://github.com/user-attachments/assets/d88f1137-7738-487f-8ddd-bf92ce749bf9" />
</p>

## 概述

Tradestack（交易栈）一款原生、易用且功能强大的量化交易平台，可快速部署您的策略并投入到实战。

想立即上手？ 马上阅读 [5分钟教程 ⏱️](./QuickStart.md)!

交易栈的设计理念是：**“让量化交易触手可及”**，降低量化交易使用门槛、将量化交易核心理念简单化，实用化。

- **简约不简单，不变应万变**

> 将复杂功能化繁为简，既功能强大又易上手，无需编程。通过组件化、标准化的设计，像搭积木一样构建可复用的操盘模块，加速量化模型投入实战。您可以

- **投研直达交易的完整闭环**

> 打造从数据建模、策略定义到交易执行的完整闭环, [localization support](https://docusaurus.io/docs/i18n/introduction) via CrowdIn. Empower and grow your international community by translating your documentation.

- **企业级量化架构**

> While Docusaurus ships with the key pages and sections you need to get started, including a home page, a docs section, a [blog](https://docusaurus.io/docs/blog), and additional support pages, it is also [customizable](https://docusaurus.io/docs/creating-pages) as well to ensure you have a site that is [uniquely yours](https://docusaurus.io/docs/styling-layout).




想快速了解系统的主要模块和功能 -> [ 功能预览 ](Preview.md)

## 快速部署

- **数据库准备**

1. 确认您已安装并能正常使用 **MySQL**。
2. 准备一个 MySQL 账户（建议为专门账户，避免使用 root）。  
3. 新建数据库，执行以下命令：
```bash
# 使用 root 或已有账户登录 MySQL
mysql -u root -p

# 创建数据库
CREATE DATABASE tradestack DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;

# 创建专用用户（替换 your_password 为自定义密码）
CREATE USER 'tradeuser'@'%' IDENTIFIED BY 'your_password';

# 授权用户访问新数据库
GRANT ALL PRIVILEGES ON tradestack.* TO 'tradeuser'@'%';

# 刷新权限
FLUSH PRIVILEGES;
```

- **服务器端部署**

1. 双击运行安装程序，按照提示点击 [ 下一步 ]完成安装，打开服务器端程序。
2. 在程序界面，点击：[ v ] - [ 安装 - 运行环境 ]，系统将自动初始化环境，耐心等待完成。
3. 当出现以下信息，则说明服务器端安装成功。 
```bash
2025-09-26 08:04:07：√ 完成处理基本板块及概念块板框架架
2025-09-26 08:04:07：√ 运行环境预处理、初始化成功，系统准备就绪...
--------------------------------------------------------------------------------
2025-09-26 08:04:07：实盘与仿真环境 - 交易数据服务 - 已连接
2025-09-26 08:04:07：实盘与仿真环境 - 全局任务计划 - 启动中
```
4. 部署成功后，请保持Tradestack Server持续运行，客户端将通过它进行通信并执行所有操作。

- **客户端部署**

1. 双击运行安装程序，按照提示 一直点击 [ 下一步 ]，直至安装完成。
2. 安装完成后，打开客户端程序。
3. 使用默认用户名和密码，即可进入软件主界面。

- **客户端连接**

> ⚠️ **问题：网络通讯错误，请稍后再试**  
> **原因**：客户端配置文件 `Connection.xml` 未正确生成。  
>  
> **解决办法：**  
> 1. 在服务器端，打开 [ 菜单 ]-> [ 生成客户端链接文件 ]
> 2. 输入Tradestack server运行所在服务器的IP地址，点击 [ 生成链接配置文件 ]： 
> 3. 将生成的 `Connection.xml` 拷贝至客户端安装目录的根目录。  
> 4. 重新启动客户端，即可正常登录。  


[安装文档](http://www.tradestack.org:3000/#/installation) 获取更多信息。

## 联系我们 

Tradestack（交易栈）作为一款独立开发者的软件，**社区版永久免费开放使用**。欢迎您通过以下方式支持或参与：  
- **提交反馈**：在使用过程中发现问题或有改进建议，欢迎提出；  
- **贡献代码/文档**：任何 PR 或文档优化，都是对项目的巨大帮助；  
- **交流探讨**：一起探索更高效、更稳健的量化交易实践。  

您的每一份参与，都会让 Tradestack（交易栈） 变得更好。

- 微信联系：
  <img width="90" height="90" alt="wechat" src="https://github.com/user-attachments/assets/86a97b8b-eb91-49bc-9ea8-999c972f393e" />
- 文档中心：[docs.tradestack.org](http://www.tradestack.org:3000/#/README)

## License

Docusaurus is [MIT licensed](./LICENSE).
