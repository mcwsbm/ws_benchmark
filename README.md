# Minecraft Websocket Benchmark

本仓库将对那些主流的Minecraft Websocket(以速建为主题的)进行基准测试.测试内容包括发包速度，错误处理，使用难易度等.



## 基础

| 名称     | Tr Func                   | FastBuilder Pro         | Ycloud           |
| -------- | ------------------------- | ----------------------- | ---------------- |
| 开发组   | xuannian/Voyage27/Mcayear | CAIMEO/Ruphane/Torrekie | Yamstrip         |
| 开发日期 | 2019-11-30                | 2018-6或更早            | 2020-1或更早     |
| 用户管理 | 论坛+白名单               | 用户中心+Telegram群     | 白名单+QQ群      |
| 价格     | 0                         | 120CNY                  | 0 - 16CNY        |
| 服务器   | 云端                      | 本地/云端               | 云端             |
| 文档完备 | Yes                       | Yes                     | No               |
| 编程语言 | NodeJs                    | NodeJS                  | NodeJS           |
| 框架     | nodejs-websocket          | ws                      | nodejs-websocket |
| 稳定性   | 良好                      | 良好                    | 一般             |
| 难易     | 简单                      | 普通                    | 简单             |
| 发包速度 | 20-30                     | 800+                    | 30-50                |
| 软件语言 | 中文                      | 英语                    | 中文             |
| 商业使用 | No                        | No                      | No               |
| 自由度   | 一般                      | 高                      | 一般             |
| 命令规范 | 无                        | Linux shell             | 无               |
| 核心开源 | No                        | Yes                     | No               |



## 功能

| 名称           | TrFunc        | FastBuilder Pro                 | Ycloud        |
| -------------- | ------------- | ------------------------------- | ------------- |
| 支持的建筑格式 | schematic/nbt | schematic/nbt/mcacblock/bdp/bdx | schematic/nbt* |
| 像素画         | Yes           | Yes                             | Yes           |
| 加密连接       | No            | Yes                             | No            |
| 圆/球/椎       | No            | Yes                             | No            |
| 数学表达式解析 | No            | Yes                             | No            |
| 文字打印       | No            | Yes                             | No            |
| 脚本加载       | No            | Yes                             | No            |
| 地形生成       | Yes           | Yes                             | No            |
| 导出建筑       | Yes           | Yes                             | Yes           |
| 迷宫生成       | Yes           | No(Soon?)                       | No            |
| 混合建造       | No            | Yes                             | No            |
| 过滤器         | No            | Yes                             | No            |
| 分块建造       | No            | Yes                             | No            |
## 用户体验
| 名称 | TrFunc | FastBuilder Pro | Ycloud |
| --- | ------- | --------------- | ----- |
| 建筑排队 | 无 | 无 | 有且长 |
| 速度真实 | Yes | Yes | No |
| 客户服务 | 较好 | 一般 | 较好 |
| 崩溃 | 较少 | 较少 | 几乎每日 |
| 维护 | 较少 | 较多 | 未知 |
| 世界聊天 | 支持 | 支持 | 支持 |
| 无用消息后缀 | 偶尔(?) | 无 | 有 |
| 繁琐登录 | 有 | 无 | 有 |
| 用户与开发组矛盾 | 较少 | 较多 | 较少 |
| 无用title | Yes | No | Yes |
| 综合情况 | 较好 | 一般 | 极差(或无?) |
## 安全性
| 名称 | TrFunc | FastBuilder Pro | Ycloud |
| --- | ------- | --------------- | ----- |
| 防护 mcwsdebugger | 不能 | 不能 | 不能 |
| 防止数字游戏名 | 可以 | 可以 | 错误直接输出至游戏(TypeError) |
