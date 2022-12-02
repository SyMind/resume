# 个人信息

* 潘聪聪 / 男 / 1996
* 本科 / 沈阳工业大学计算机科学与技术系 / 2014.09-2018.07
* Email：<dacongsama@live.com>
* Github：<https://github.com/SyMind>

---

# 技能清单

* 目前工作使用 React / Taro / TypeScript
* 曾经工作使用 React Native / Electron / Vue.js / Vuex / mpvue
* 了解编译器前端，熟悉 Babel / ESLint，开发 Babel 插件和 Eslint 规则
* 偶尔配置 Webpack / Gulp.js / Rollup.js / Vite
* 了解函数式编程，学过一点 Haskell 和范畴论
* 正在学习 Golang
* 贡献过很多开源项目 MQTT.js（物联网协议） / eslint-plugin-react（Eslint 插件） / ecomfe/react-hooks（百度 React Hooks 库），Taro（跨 h5 和小程序端的框架）技术委员会生态合作者

---

# 个人介绍

对前端充满热情，狂热的开源拥护者。正在努力学习并积极构建工具，渴望能让前端开发能变得更加愉悦。将代码视为自己的延伸，极其渺茫但永不放弃地去追求永恒。

---

# 工作经历

### 字节跳动 - 前端工程师 (2020.07-至今)

TikTok Data TnS 机器审核 B 端。

### 百度 - 前端工程师 (2020.03-2022.07)

开发与维护医美辞典的 h5、小程序、管理后台 / 医美业务医生、日记、医院等 B 端项目 / 柠檬爱美主站等 C 端项目。

### 便利蜂 - 前端工程师 (2018.07-2020.03)

开发与维护内部办公软件的 APP 和 PC 前端 / 监控报警平台前端 / 营建管理前端 / 基于 MQTT.js 消息平台的 npm 包等。

# 主要项目

* 美学辞典

医美科普平台。C 端基于 Taro3 开发，支持 h5 端、百度小程序端、微信小程序端。

为提升 h5 的页面首屏速度，利于 SEO。开发 tarojs-plugin-platform-nextjs Taro 插件，来让 Taro 支持 SSR 和 ISR。

后台用于管理词条内容。使用内部 amis 低代码平台，复杂的组件单独开发，并发布 npm 包以集成到 amis 中。打包工具选用 rollup，构建 mock 的 amis 环境用于本地测试组件。

其中在内容编辑表单方面，前后端约定用 JSON Schema 进行描述。前端基于 react-json-schema-form 生成表单，也开发相应的 JSON Schema 可视化编辑器，用于配置新词条类型的结构。

* Taro 生态

在 Taro3 建设早期，参与解决 h5 和百度小程序相关的 bug，贡献 pr 17 次。

开发 taro2-to-3 工具，帮助 taro 2.x 项目升级到 taro 3.x 项目的工具，基于 jscodeshift 构建。Taro 官网升级指南中推荐的一键升级工具。

开发 tarojs-plugin-platform-nextjs Taro 插件，用于编译为 Next.js 应用。让 Taro 在 Web 端支持 SSR 和 ISR，提升页面首屏速度，利于 SEO。Taro 官网目前唯一的服务器端渲染解决方案。

* 内部工具

主动开发埋点的可视化 Chrome 插件，使开发阶段时研发的自测更加便利，让测试阶段时产品能够更好地进行验收。

为了在开发时验证在小程序的埋点，起初基于 Electron 开发相应的客户端，然后通过在小程序开发者工具中配置代理拦截埋点请求。客户端很大，且每次配置开发者工具中的代理很麻烦。于是开发工具 swan-extension-injector，直接将 Chrome 插件直接注入到百度小程序开发工具中，来解决以上问题。

* 医美业务医生、日记、医院等 B 端项目

医美业务 B 端的几个项目在接手时已有2年的历史，存有较多技术负债，如编码规范、性能问题、redux 滥用、上线期间页面不可用等。解决项目中明显的性能问题、redux 的滥用问题。约束项目代码规范，提升开发效率。

对项目中的逻辑进行梳理，解决如登录后页面多次跳转、接口循环调用等明显的性能问题。在日常迭代中，梳理相关的 redux 状态树结构，通过状态推导的方式移除冗余状态，提取非全局或仅在单个页面生命周期中的状态等。推进 hooks 库、更新 antd 至4版本、升级 babel 至7版本以支持新的 JavaScript 语法特性，提升开发效率。使用 eslint 约束项目代码，积极参与并同步公司配置，依据公司原有规范、react-eslint-plugin 中推荐的规则与当前项目现状进行整理编写团队 wiki，并追加规则约束的详细原因。

* 柠檬爱美、医美百科等 C 端项目

承接柠檬爱美中热玛吉验真、AI 测肤，医美百科落地页等相关需求的开发，解决现有项目中的问题。

开发 postcss 插件映射 PingFangSC 字体族至字重，解决部分字重在安卓中不支持的问题。推动部分内容落地页的 SSR 落地，以提升首屏渲染速度、SEO，做框架选型、BFE 兜底策略、依靠公司现有基础设施的部署流程等工作。

* 内部 IM PC 端

内部 IM 应用 PC 端，基于 Electron 开发。

起初应用运行不稳定、性能低、功能不完善。使用错误边界隔离功能独立的组件树，避免整个应用崩溃；长列表性能优化；优化应用的更新策略，提高用户对新版本的更新率；使用 asar 对 node_modules 进行打包以提高应用的启动速度。增加大搜索功能、合并消息转发、消息回复、音视频聊天等，优化群/用户信息管理、增强工作台配置扩展能力等。引入 react-hot-loader 提高开发效率。

直接反馈软件崩溃、严重卡顿的用户基本消失，JS 端的崩溃接入报警。为用户提供更多提高办公效率的功能，以用户行为的埋点驱动需求迭代。

* 内部 IM iOS、Android 端

内部 IM 应用 iOS、Android 端，基于 React Native 拥有工作流、即时通信等功能，面向总部、店员。

维护“我的”、“工作台”、登陆 / 登出等主包页面和逻辑，工作流相关的逻辑和页面的开发与维护。

* 内部消息平台前端包

搭建高性能，并支持 Web 端、微信小程序端、支付宝小程序、react-native 端的通用消息平台。 

基于 MQTT.js 开发，封装相关业务逻辑为一个独立的 npm 包。修改底层 mqtt-packet 包，在报文头中添加 messageId 作消息的唯一标示，添加 returnCode 封装业务相关的状态码等。使用 typescript 开发，添加必要的单元测试。
