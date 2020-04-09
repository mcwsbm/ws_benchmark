# Minecraft Websocket Benchmark

本仓库将对那些主流的Minecraft Websocket(以速建为主题的)进行基准测试.测试内容包括发包速度，错误处理，使用难易度等.



## 基本信息

| 名称     | Tr-Func                   | FastBuilder Pro         | YCloud           |
| :--------: | :-------------------------: | :----------------: | :---------------: |
| 开发组   | xuannian/Voyage27/Mcayear | CAIMEO/Ruphane/Torrekie | Yamstrip         |
| 开发日期 | 2019-11-30                | 2018-6或更早            | 2020-1或更早     |
| 官网主页       | [tr-func.com](tr-func.com)            | [fastbuilder.pro](fastbuilder.pro)                             | [ycloud.ws](ycloud.ws)            |
| 用户管理 | 论坛/QQ群               | 用户中心/QQ群/Telegram群     | QQ群      |
| 权限       | 白名单            | 白名单                             | 白名单            |
| 价格     | CNY 0                         | CNY 120                  | CNY 0 - 16       |
| 服务器   | 云端                      | 本地/云端               | 云端             |
| 文档完备 | Yes                       | Yes                     | No               |
| 编程语言 | Node.js                    | Node.js                  | Node.js           |
| 框架     | nodejs-websocket          | ws                      | nodejs-websocket |
| 稳定性   | 良好                      | 良好                    | 差             |
| 难易     | 简单                      | 普通                    | 简单             |
| 发包速度 | 20-30                     | 800+                    | 30-50                |
| 软件语言 | 中文                      | 英语                    | 中文             |
| 商业使用 | No                        | No                      | No               |
| 自由度   | 一般                      | 高                      | 一般             |
| 操控方式 | 聊天命令            | 聊天命令                  | 聊天命令            |
| 命令规范 | /                        | Linux shell             | /               |
| 核心开源 | No                        | Yes                     | No               |
| 加密连接       | No            | Yes                             | No            |




## 功能

(与建筑有关的)

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 支持的建筑格式 | schematic/nbt | schematic/nbt/mcacblock/bdp/bdx | schematic/nbt |
| 像素画         | Yes           | Yes                             | Yes           |
| 几何       | No            | Yes                             | No            |
| 数学表达式解析 | No            | Yes                             | No            |
| 文字打印       | No            | Yes                             | No            |
| 开放API       | No            | Yes                             | No            |
| 地形生成       | Yes           | Yes                             | No            |
| 导出建筑       | Yes           | Yes                             | Yes           |
| 迷宫生成       | Yes           | No                       | No            |
| 混合建造       | No            | Yes                             | No            |
| 过滤器         | No            | Yes                             | No            |
| 分块建造       | No            | Yes                             | No            |

## 其他评判标准

### 用户体验

| 名称 | Tr-Func | FastBuilder Pro | YCloud |
| :-: | :-----: | :-------------: | :---: |
| 建筑排队 | 无 | 无 | 有且耗时长 |
| 报速准确 | Yes | Yes | No |
| 客户服务 | 较好 | 一般 | 较好 |
| 崩溃 | 较少 | 较少 | 几乎每日 |
| 维护 | 较少 | 较多 | 未知 |
| 世界聊天 | 支持 | 支持 | 支持 |
| 无用消息后缀 | 偶尔(?) | 无 | 有 |
| 繁琐登录 | 有 | 无 | 有 |
| 用户与开发组矛盾 | 较少 | 较多 | 较少 |
| 无用title | Yes | No | Yes |
| 综合情况 | 较好 | 一般 | 极差(或无?) |

### 安全性

| 名称 | Tr-Func | FastBuilder Pro | YCloud |
| :-: | :-----: | :-------------: | :---: |
| 防护 mcwsdebugger | 不能 | 不能 | 不能 |
| 防止数字游戏名 | 可以 | 可以 | 错误直接输出至游戏(TypeError) |

### 用户可访问性

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 验证方式 | 用户名/用户群机器人确认 | 用户名/Xbox Live/用户中心账号 | 用户名 |
| 版本可访问性 | 中国版 | 中国版/基岩版/教育版 | 中国版/基岩版/教育版 |
| 平台可访问性 | 默认全部 | 默认全部 | 默认全部 |
| 信息变更方式 | 开发者/用户群机器人处理 | 用户中心/密保邮箱 | 开发者人工处理 |
| 可向开发者捐赠 | Yes | Yes | Yes |
| 上传文件 | Yes | Yes | Yes |
| 安装方式 |  | 在线安装器 |  |

### 用户信息/隐私权的历史记录

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 用户信息丢失记录 | 由于管理原因曾清理用户信息 | 服务器调试故障导致部分用户信息丢失 | 创建者主动移除 |
| 用户设备文件损失记录 |  | 2019.4发布的FBPro v3p3版本中的一项错误导致用户数据被清空 |  |
| 用户隐私泄露记录 | 程序设计问题导致玩家的信息可以被他人访问 |  | 程序设计问题导致玩家的信息可以被他人访问 |
| 模糊的用户协议 |  |  | 没有用户协议，仅依靠群公告 |
|    |
| 截至本评测发布前<br />该列表提及问题已经修复 | Yes | Yes | No |
