<p align="center">
<img width="1440" height="280" alt="github_banner_white" src="https://github.com/user-attachments/assets/d88f1137-7738-487f-8ddd-bf92ce749bf9" />
</p>

## 交易栈 - 让量化交易触手可及

交易栈（Tradestack）一款原生、易用且功能强大的量化交易平台，可快速部署您的策略并投入到实战。

想立即上手？ 马上阅读 [5分钟快速入门教程 ⏱️](./QuickStart.md)!

- **简约不简单，不变应万变**

  > 复杂的理念被化繁为简，功能依然强大，但上手很轻松，无需编程。通过模块化、标准化的设计，像搭积木一样拼接可复用的操盘模块，让量化模型更快进入实战。  
  > 您可以通过 [策略定义](./StrategyDefinition.md) 自由组合来生成策略，也可以借助 [策略定义助手](./StrategyDefinition.md) 快速生成策略，即刻投入实盘或仿真环境交易。

- **投研直达交易的完整闭环**

  > 打造从数据建模、策略定义到交易执行的完整闭环。借助 [模型对象管理](./StrategyDefinition.md) 和 [模型分析](./StrategyDefinition.md) 工具进行数据建模，通过 [交易规则](./StrategyDefinition.md) 对账户进行全局规则和风险控制；  
  > 利用 [因子库设计](./StrategyDefinition.md) 创建指数或股票的买入和卖出因子库；  
  > 通过 [自选股](./StrategyDefinition.md) 和 [选股模型](./StrategyDefinition.md) 动态生成股票池，最后通过 [启动因子策略](./StrategyDefinition.md) 执行自动化交易。

- **构建企业级量化架构**

  > 策略、规则、交易与任务引擎协同运行，结合先进算法，有效降低技术门槛和效率瓶颈。  
  > 原生代码与微服务架构配合全内存管理，实现微秒级响应与高吞吐量执行。  
  > 即插即用，方便接入券商柜台系统，支持多用户、多策略，7×24 小时全天候无人值守运行。


## 系统架构

<img  alt="tactics" src="./images/arch_diagram.svg" />

- **第一步：建立交易账户**
  > 通过 [交易账户管理](./StrategyDefinition.md) 创建或关联证券账户，作为策略执行的载体。
  
- **第二步：设定交易规则**
  > 全局性的对交易账户进行交易风险的控制，包括目标仓位、交易行为、资金分配、规则开关、委托频率、无人值守等定义，提高了用户交易掌控能力。您可以在 [交易规则设定](./StrategyDefinition.md)  中设置。

- **第三步：形成交易标的**
  > 股票池的来源分为两种，一种是选股模型生成股票池，一种是高级托管任务生成；在 [自选股](./StrategyDefinition.md)  中创建股票池，对个股设置优先级、资金权重和交易行为，实现精细化控制。

- **第四步：选择因子库**
  > 因子是策略运算的核心，每一个交易账号对应两个策略，分别为买入策略和卖出策略，买入方向 → 买入因子库，卖出方向 → 卖出因子库，在 [因子库设计](./StrategyDefinition.md) 中定义，因子的底层数据来源由 [因子数据源](./StrategyDefinition.md) 中创建。
 
- **第五步：策略组装**
  > 完成上述准备后，在 [策略定义](./StrategyDefinition.md)  中创建买入/卖出方向策略，并指定交易账户、股票池、股票因子库和指数因子库。
    
- **第六步：启动策略**
  > 通过 [ 启动因子策略 ](./StrategyDefinition.md)  运行策略，系统持续匹配股票池，条件满足立即交易。

> 💡 如果您觉得操作繁琐，也可以借助 [策略定义助手](./StrategyDefinition.md) 一键生成完整的因子策略，系统默认在第一次登录时，自动创建了一项**行稳致远步步高升1号**策略，这项策略直接可以投入实际交易。


## 使用场景



## 常见问题
- 需要学习编程语言吗?

  > 无需学习编程语言，高阶用户仅需掌握SQL语句，同时绝大部分SQL脚本系统自动生成。

- 是否支持本地化部署？
  > 交易栈完全支持本地化与私有化部署，用户可在自己的服务器、局域网或个人电脑上独立运行，无需依赖第三方云端。

- 

## 捐赠

## 联系我们 

交易栈（Tradestack）作为一款独立开发者的软件，**社区版永久免费开放使用**。欢迎您通过提交反馈、贡献代码或文档的方式支持或参与；您的每一份参与，都会让交易栈（Tradestack） 变得更好。

- 微信联系：
  <img width="90" height="90" alt="wechat" src="https://github.com/user-attachments/assets/86a97b8b-eb91-49bc-9ea8-999c972f393e" />
- 文档中心：[docs.tradestack.org](http://www.tradestack.org:3000/#/README)

## License

Docusaurus is [MIT licensed](./LICENSE).
