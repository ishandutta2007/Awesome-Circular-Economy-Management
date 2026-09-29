# Awesome-Circular-Economy-Management

# 顶级循环经济管理平台生态系统



**精选 SaaS 产品与开源 GitHub 项目列表**

*聚焦循环供应链、逆向物流、数字产品护照与二手交易*

**最后更新：2026 年 9 月**



本仓库追踪**循环经济管理**领域的知名 **SaaS 平台**与**开源项目**。这些工具帮助企业管理产品生命周期、优化逆向物流、实现供应链溯源，并支持数字产品护照 (DPP) 合规。



**示例**包括 Circularise、Worldly、EON、Optoro、ReverseLogix、Loop Returns、Reflaunt、Cycle Platform、Trace For Good 和 Reconomy（该领域的领先者）。



**开源重点**：循环经济的开源生态**正在快速成熟**。**RELOG**（阿贡国家实验室）提供逆向物流网络的 MILP 优化 。**DPP01** 是面向食品生产商的开源 DPP 框架 。**open-dpp-registry** 实现了基于 URN 的区块链产品护照发现机制 。**Dolibarr 退货模块**为中小企业提供免费的逆向物流工作流 。本列表重点收录这些可自托管的生产级方案。



欢迎贡献！提交 PR 以添加/更新条目。保持描述事实性，并链接到官方网站。



## 目录



- [SaaS/托管平台](#saas托管平台)

- [开源 GitHub 项目](#开源github项目)

- [如何贡献](#如何贡献)

- [免责声明](#免责声明)



## SaaS/托管平台



- **[Circularise](https://www.circularise.com/)**

  基于区块链的供应链可追溯性和数字产品护照平台。ISO 27001:2022 认证。支持从原材料到成品的全链路追踪，通过专有的选择性数据共享技术，供应商可在保护机密信息的同时满足客户和监管要求 。服务汽车、塑料、化学品等行业，客户包括 Porsche 和 Teijin 。



- **[EON](https://www.eon.xyz/)**

  企业数字 ID 技术领导者，通过 **EON Product Cloud** 为产品创建序列化数字身份。与 Inspectorio 合作，将供应链数据直接流入 EON，帮助品牌从 DPP 试点过渡到可支持数百万产品的规模化运营 。2026 年 9 月合作发布，目标市场为零售和服装品牌。



- **[Worldly](https://worldly.io/)**

  可持续性数据平台，前身为 Higg。为服装和消费品行业提供供应链环境和社会影响测量。



- **[Optoro](https://www.optoro.com/)**

  逆向物流和退货管理平台。通过 AI 驱动的处置路由和价值回收优化，帮助零售商最大化退回商品的价值。



- **[ReverseLogix](https://www.reverselogix.com/)**

  端到端逆向物流管理平台。提供退货、维修、召回和处置工作流。



- **[Loop Returns](https://loopreturns.com/)**

  电商退货管理平台。专注于 Shopify 生态，提供退货门户、换货激励和退款自动化。



- **[Reflaunt](https://www.reflaunt.com/)**

  二手转售和循环商务平台。帮助时尚品牌推出转售计划，连接买家和卖家。



- **[Cycle Platform](https://www.cycle.app/)**

  循环经济软件平台。管理可重复使用包装和容器的押金返还系统。



- **[Trace For Good](https://traceforgood.com/)**

  供应链可追溯性平台。提供产品溯源、材料追踪和合规报告。



- **[Reconomy](https://www.reconomy.com/)**

  循环经济服务提供商。管理废弃物、资源和合规性，为企业提供循环经济解决方案。



## 开源 GitHub 项目



### 数字产品护照 (DPP) 与溯源



- **[DPP01](https://github.com/arcticscihub/DPP01)**

  **面向食品生产商的开源 DPP 框架。** 提供数据采集和组织平台，支持 Digital Product Passport 的管理和创建 。功能包括：结构化数字记录生成（材料成分、采购、使用）、EU DPP 合规支持、价值链可追溯性和透明度、可持续性报告数据复用、循环性和资源管理。部署方式灵活：联系仓库所有者支持、AWS DevOps 部署、或内部团队部署。**开源**。



- **[open-dpp-registry](https://pkg.go.dev/git.nilu.no/ce-rise-is/utils/open-dpp-registry)**

  **基于 URN 的区块链产品护照发现注册表。** 解决 DPP 生态中的关键问题：如何发现产品 DPP 的维护者 。使用 RFC 8141 兼容的斜杠分隔 URN 结构（`/lot/...`、`/serial/...`），支持 GTIN14 + 批次 + 序列号的精确识别。区块链类型：内存、文件、以太坊。REST API 端点包括记录发现、记录管理和区块链操作。**Go 1.22+**。支持产品认证、历史追踪和跨提供商连续性的用例。



- **[mycelix-supplychain](https://github.com/Luminous-Dynamics/mycelix-supplychain)**

  **去中心化供应链溯源系统，带拜占庭容错共识。** 将 ERP/IoT 事件转换为签名的 DKG 声明和可移植 VC，带哈希链接的 lineage 证明 。功能包括：事件→VC→DKG 声明流程、CSV/MQTT 适配器、验证器 UI + CLI、**产品护照导出**、选择性披露（SD-JWT/BBS+ 密码学）。用例：追踪溯源、合规审计、防伪、召回影响分析。**Rust 核心 + TypeScript SDK**。**Apache-2.0**。状态：Alpha（试点参考实现）。



- **[TraceFlow](https://github.com/Cao150702/traceflow)**

  **去中心化商品溯源系统，为实体商品提供区块链验证的数字护照。** 为每件商品颁发唯一 ID + 二维码 + 可选 NFT 护照 。功能包括：商品注册、流转追踪（每次交接上链）、扫码验证、**AI 异常检测**（规则引擎 + GPT-4o-mini）、真实性评分。技术栈：Next.js 14、Supabase、Polygon、ethers.js。用例：限量版商品、精品咖啡、电子产品防伪、二手市场所有权验证。



### 逆向物流与退货管理



- **[RELOG](https://github.com/ANL-CEEESA/RELOG)**

  **阿贡国家实验室开发的开源逆向物流优化包。** 使用混合整数线性规划，帮助用户确定战略性决策：制造和回收工厂的位置和建设时间、工厂规模、扩建时机和幅度、每个工厂的输入材料来源和输出目的地、立即处理还是储存 。已成功应用于关键材料回收（废 NiMH 和锂离子电池）、生物质制氢、电子产品/塑料/太阳能 PV 回收等研究。**开源**。



- **[Dolibarr 退货与 RMA 模块](https://github.com/zacharymelo/doli-returns)**

  **中小企业逆向物流免费模块套件。** 包括四个协同工作的模块 ：**Doli-Returns**（接收退货入库、发放信用）、**RMA/Warranty**（保修和 RMA 跟踪、自动生成保修记录）、**Customer Inventory**（客户已购产品和服务视图）、**Box Label**（从 MRP 生成唯一标签）。V1.0.4（2026 年 4 月发布）修复了重复行和空行 bug。**免费开源**。



- **[ROBOSTAPLE](https://github.com/pacobaco/robostable)**

  **分布式逆向物流操作系统**，将家庭变为可编程库存节点，由事件驱动路由和 AI 需求预测协调 。早期项目。



### 循环商务与二手市场



- **[Phoenix Project](https://github.com/The-PhoenixProject/The-Phoenix-Project-Front-end)**

  **开源二手交易平台，连接环保买家和卖家。** 支持回收、升级再造和转售 。功能：用户注册/登录、产品浏览/创建/编辑/删除、社交帖子（点赞/评论）、Socket.IO 实时聊天和通知、文件/图片上传、生态积分。技术栈：React、Socket.IO、JWT 认证。**ISC License**。



- **[openmagpie / AgentMarket](https://socket.dev/npm/package/openmagpie)**

  **AI 代理原生的二手市场框架。** 为 AI 代理自动列出、匹配、谈判和结算二手交易而构建 。核心协议：list、search、offer、settle。匹配引擎可插拔（精确/模糊/LLM）。存储适配器可插拔（SQLite/PostgreSQL）。支持 MCP Server 和 REST API。**npm 包**，早期版本（v0.1.0）。



- **[ZeroWaste](https://github.com/jessem8/zerowaste)**

  **社区循环经济平台。** 支持分享升级再造项目、物品交换市场和生态社区论坛 。功能：用户管理、社区论坛、共享交换平台（分类筛选、Google Maps 集成、消息系统）、升级再造目录（PDF 导出）。技术栈：PHP 7.4+、MySQL、Tailwind CSS、Alpine.js。符合 **UN SDG 12**（负责任消费和生产）。教育用途。



### 其他强开源选项



- **数字产品护照**：**DPP01**（食品生产商）、**open-dpp-registry**（区块链发现）、**mycelix-supplychain**（去中心化溯源）、**TraceFlow**（AI 风险分析）。

- **逆向物流**：**RELOG**（MILP 优化）、**Dolibarr 模块**（中小企业免费）、**ROBOSTAPLE**（分布式 OS）。

- **循环商务**：**Phoenix Project**（二手市场）、**openmagpie**（AI 代理市场）、**ZeroWaste**（社区平台）。



**构建自定义系统的框架**：结合 **DPP01** 或 **open-dpp-registry** 用于 DPP 生成和发现，**RELOG** 用于逆向物流网络优化，**Dolibarr 退货模块** 用于中小企业逆向物流工作流，**Phoenix Project** 或 **ZeroWaste** 用于二手交易平台。添加 **PostgreSQL** 和 **区块链**（以太坊/Polygon）用于溯源持久化。



## 如何贡献



1. Fork 仓库。

2. 在 `README.md` 中添加/编辑条目（遵循现有格式）。

3. 包含：名称、链接、1-2 句描述，以及是 SaaS 还是开源。

4. 提交 PR 并附简短说明。



如果你觉得这个仓库有用，请点星！



## 免责声明



- 这是一个**社区精选**列表——并非详尽无遗，也不构成认可。

- 循环经济平台处理供应链和产品数据；确保符合 EU DPP 法规、ESPR 和相关可持续发展披露要求。

- **开源现实**：循环经济的开源生态在 **DPP 框架**（DPP01、open-dpp-registry）和 **逆向物流优化**（RELOG）层面**已经可用**，但完整的商业循环经济平台（Circularise、EON、Optoro）在**企业级供应链集成**、**选择性数据共享**和**规模化部署**方面仍具有显著优势。开源方案适合试点项目和学术研究，生产级部署需要大量定制开发。



---



**为可持续发展经理、循环经济工程师、供应链分析师和逆向物流团队打造。**

让循环经济管理更开放、透明、可追溯。
