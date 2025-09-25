
[![Build Status](https://travis-ci.org/tainacan/tainacan.svg?branch=develop)](https://travis-ci.org/tainacan/tainacan)

# 交易栈 - 极速策略交易平台

一款能够迅速将量化产品投入实战应用的快速部署平台；旨在降低量化交易使用门槛、将量化交易核心理念简单化，实用化；
无论你的角色是个人投资者、还是机构，风格是短线、还是中长线，均可在该平台寻找到价值并提升投资赢率。  

## ✨ 谁适合使用交易栈？

- 对策略执行效率有高要求的 **量化交易从业者**
- 希望将选股逻辑转化为可自动执行模型的 **专业投资者**
- 不具备编程能力，但熟悉投资逻辑的 **投研人员**
- 需要部署多账户、多策略、全天候监控的 **私募或机构团队**
- 有多源数据管理与个性化因子建模需求的 **高阶策略研究者**

## 🌟 平台亮点

- 🧠 **无代码建模**：可视化策略搭建，0 编程经验也能构建专业模型
- 🔁 **策略执行闭环**：从因子 → 股票池 → 仓位调整 → 实时交易，流程可全自动
- ⚙️ **策略自演化能力**：借助任务与计划引擎，实时更新选股模型与因子条件
- 🧩 **模块积木式组合**：因子库、规则、股票池、账户均可自由组合与继承
- 📈 **T+0、智能拆单机制**：精细化控制下单行为，满足高频或稳健操作
- 🗃️ **多数据源接入**：支持接入本地、局域网、互联网数据库作为因子源
- 🖥️ **仿真与实盘环境切换**：策略部署前可在仿真环境反复测试评估

## 🚀 快速开始

```bash
# 克隆项目
git clone https://github.com/yourname/yourproject.git

# 进入目录
cd yourproject

# 安装依赖
npm install   # 或者其他方式

# 启动项目
npm run start

---
id: 'storage'
title: 'Storage'
description: 'Use Supabase to store and serve files.'
subtitle: 'Use Supabase to store and serve files.'
sidebar_label: 'Overview'
hideToc: true
---

Supabase Storage makes it simple to upload and serve files of any size, providing a robust framework for file access controls.

## Features

You can use Supabase Storage to store images, videos, documents, and any other file type. Serve your assets with a global CDN to reduce latency from over 285 cities globally. Supabase Storage includes a built-in image optimizer, so you can resize and compress your media files on the fly.

## Examples

Check out all of the Storage [templates and examples](https://github.com/supabase/supabase/tree/master/examples/storage) in our GitHub repository.

<div className="grid md:grid-cols-12 gap-4 not-prose">
  {examples.map((x) => (
    <div className="col-span-12" key={x.href}>
      <Link href={x.href} passHref>
        <GlassPanel icon={'/docs/img/icons/github-icon'} hasLightIcon={true} title={x.name}>
          {x.description}
        </GlassPanel>
      </Link>
    </div>
  ))}
</div>

export const examples = [
  {
    name: 'Resumable Uploads with Uppy',
    description:
      'Use Uppy to upload files to Supabase Storage using the TUS protocol (resumable uploads).',
    href: 'https://github.com/supabase/supabase/tree/master/examples/storage/resumable-upload-uppy',
  },
]

## Resources

Find the source code and documentation in the Supabase GitHub repository.

<div className="grid md:grid-cols-12 gap-4 not-prose">
  {[
    {
      name: 'Supabase Storage API',
      description: 'View the source code.',
      href: 'https://github.com/supabase/storage-api',
    },
    {
      name: 'OpenAPI Spec',
      description: 'See the Swagger Documentation for Supabase Storage.',
      href: 'https://supabase.github.io/storage/',
    },
  ].map((x) => (
    <div className="col-span-6" key={x.href}>
      <Link href={x.href} passHref>
        <GlassPanel title={x.name}>{x.description}</GlassPanel>
      </Link>
    </div>
  ))}
</div>
