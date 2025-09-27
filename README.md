<p align="center">
<img width="1440" height="280" alt="github_banner_white" src="https://github.com/user-attachments/assets/d88f1137-7738-487f-8ddd-bf92ce749bf9" />
</p>

## 交易栈 - 让量化交易触手可及

Tradestack（交易栈）一款原生、易用且功能强大的量化交易平台，可快速部署您的策略并投入到实战。

想立即上手？ 马上阅读 [5分钟快速入门教程 ⏱️](./QuickStart.md)!

- **简约不简单，不变应万变**

  > 将复杂功能化繁为简，既功能强大又易上手，无需编程。通过组件化、标准化的设计，像搭积木一样构建可复用的操盘模块，加速量化模型投入实战。  
  > 您可以通过 [策略定义](./StrategyDefinition.md) 自由组合策略，也可以借助 [策略助手](./StrategyDefinition.md) 生成专业的买卖方向策略，即刻投入实盘或仿真环境交易。

- **投研直达交易的完整闭环**

  > 打造从数据建模、策略定义到交易执行的完整闭环。借助 [模型对象管理](./StrategyDefinition.md) 和 [模型分析](./StrategyDefinition.md) 工具进行数据建模，通过 [交易规则](./StrategyDefinition.md) 对账户进行全局规则和风险控制；  
  > 利用 [因子库设计](./StrategyDefinition.md) 创建指数或股票的买入和卖出因子库；  
  > 通过 [自选股](./StrategyDefinition.md) 和 [选股模型](./StrategyDefinition.md) 动态生成股票池，最后通过 [启动因子策略](./StrategyDefinition.md) 执行自动交易。

- **企业级量化架构**

  > 策略引擎、规则引擎、交易引擎与任务引擎协同运行，采用先进算法，降低技术门槛和效率瓶颈。  
  > 原生代码加微服务设计，配合全内存管理，实现微秒级响应和高吞吐量策略执行。  
  > 即插即用，方便接入券商柜台系统，支持多用户、多策略，7×24 小时全天候无人值守运行。


## 逻辑概览

```mermaid
flowchart TD
    A[交易账户] -->|绑定| B[买入策略]
    A -->|绑定| C[卖出策略]
    A --> D[全局交易规则]

    B --> E[股票池]
    C --> E[股票池]

    E --> F[因子库匹配]
    F --> G[交易执行]

    subgraph 高级托管任务
        H[动态修改参数和数据]
    end

    subgraph 任务与计划模块
        I[盘前/盘中/午休/集合竞价/盘后数据生成]
    end

    G --> H
    G --> I
```


## 使用场景


## 社区

## 捐赠

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
