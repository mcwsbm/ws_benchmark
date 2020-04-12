# Minecraft Websocket Benchmark

本仓库将对那些主流的Minecraft Websocket(以速建为主题的)进行基准测试.测试内容包括发包速度，错误处理，使用难易度等.

如果您需要对某个不在列表中的WS服务进行测试，欢迎电邮me@torrekie.dev


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
| 使用难度 | 简单                      | 普通                    | 简单             |
| 速度(秒) | 25-50                     | 650-1500                    | 30-50                |
| 软件语言 | 中文                      | 英语                    | 中文             |
| 商业使用 | No                        | No                      | No               |
| 自由度   | 一般                      | 高                      | 一般             |
| 操控方式 | 聊天命令            | 聊天命令                  | 聊天命令            |
| 命令规范 |                        | Linux shell             |                |
| 核心开源 | No                        | Yes                     | No               |
| 加密连接       | No            | Yes                             | No            |

注：

1. 上列表中“速度”最大值为最大速度，即不考虑游戏本身处理数据包所消耗时间等影响因素的速度
2. “聊天命令(ChatCommand)”是Mojang制定的一种称谓，即通过发送消息的形式进行控制的操作


## 功能

(与建筑有关的)

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 支持的结构格式 | schematic/nbt | schematic/nbt/mcacblock/bdp/bdx | schematic/nbt |
| 像素画         | Yes           | Yes                             | Yes           |
| 几何       | Yes            | Yes                             | No            |
| 数学表达式解析 | No            | Yes                             | No            |
| 文字打印       | Yes            | Yes                             | No            |
| 开放API       | Yes            | Yes                             | No            |
| 地形生成       | No           | Yes                             | Yes            |
| 导出建筑       | Yes           | Yes                             | Yes           |
| 迷宫生成       | Yes           | No                       | Yes            |
| 混合建造       | No            | Yes                             | No            |
| 过滤器         | No            | Yes                             | No            |
| 分块建造       | Yes            | Yes                             | No              |
| 合并算法       | Yes     | No                            | No          |
| 宣传真实性     | 高             | 极高                              | 低         |
| 备注     | 1、几何功能介绍较为模糊<br />2、合并算法缺乏优化 | 1、“mcacblock”是《我的世界》中国版资源开发者 无维 制作的应用于Mod的结构格式<br />2、“bdp/bdx”是FastBuilder Pro的结构格式                             | 1、在合并算法功能上进行虚假宣传，并未真正实现<br />2、过分夸大性质的宣传 |

## 其他评判标准

### 用户体验

| 名称 | Tr-Func | FastBuilder Pro | YCloud |
| :-: | :-----: | :-------------: | :---: |
| 建筑排队 | No | No | 有且耗时长 |
| 报速准确 | Yes | Yes | No |
| 客户服务 | 较好 | 一般 | 较好 |
| 崩溃 | 较少 | 较少 | 几乎每日 |
| 维护工作 | 正常 | 较多 | 较多 |
| 世界聊天 | Yes | Yes | Yes |
| 无用提示语 | 有 | 无 | 有 |
| 繁琐登录 | 有 | 无 | 有 |
| 用户与开发组矛盾 | 较多 | 较多 | 较少 |
| 无用title | Yes | No | Yes |
| 综合情况 | 较好 | 一般 | 极差 |
| 备注 | | | 存在严重虚报速度的情况 |

注：

1. “崩溃”指由于各种可能的原因造成的服务异常中断
2. “世界聊天”指用户间可以借助WebSocket进行异服聊天的操作
3. “无用提示语”指无实际意义或以装饰为主要作用的提示语
4. “无用title”同上，但其显示为游戏界面中的标题

### 安全性

本项目测试不同产品对机器用户/虚假用户的防控能力

| 名称 | Tr-Func | FastBuilder Pro | YCloud |
| :-: | :-----: | :-------------: | :---: |
| 调试器 | Yes | Yes | No |
| 处理数字游戏名 | Yes | Yes | 错误，直接输出至游戏(TypeError) |
| 防止错误类型的游戏名 | Yes | No | No |

1. “调试器”指用于模拟Minecraft客户端的WebSocket客户端调试工具
2. “处理数字游戏名”可以用于验证服务端是否正确处理用户信息
3. “防止错误类型的游戏名”即防止通过一切非常规手段实现的非字符串类型的用户名称，这种用户名称可能导致服务端崩溃

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
| 备注 | Tr-Func目前有一定几率支持基岩版/教育版 | | |

注：

1. “平台可访问性”中“默认全部”指默认兼容iOS、Android、Windows UWP等可以运行Minecraft的系统
2. “信息变更方式”指用户为确保正常使用而需要更改信息时可采用的方式
3. 对于在云端运行的WS服务可能涉及读取用户文件的操作，由于云端无法读取用户本地文件，因此可能需要用户上传文件到服务器以便读取，但WS提供商可以根据自身需要来决定是否开放上传文件功能
4. “安装方式”指本地安装对应WS服务的方法

### 用户信息/隐私权的历史记录

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 用户信息丢失记录 | 由于管理原因曾清理用户信息 | 服务器调试故障导致部分用户信息丢失 | 创建者主动移除 |
| 用户设备文件损失记录 |  | 2019.4发布的FBPro v3p3版本中的一项错误导致用户数据被清空 |  |
| 用户隐私泄露记录 | 程序设计问题导致玩家的信息可以被他人访问 |  | 程序设计问题导致玩家的信息可以被他人访问 |
| 模糊的用户协议 |  |  | 没有用户协议，仅依靠群公告 |
| 服务器被破坏记录 | 群内一次被假玩家刷屏 | | 群内多次刷屏开发者未作为|
|    |
| 截至本评测发布前<br />该列表提及问题已经修复 | Yes | Yes | No |

### 不端行为的历史记录

| 名称           | Tr-Func        | FastBuilder Pro                 | YCloud        |
| :------------: | :-----------: | :-----------------------------: | :-----------: |
| 著作权 | 2019.6发布的版本抄袭了于2019.3发布的FBPro v2.9<br />使用或参照了其他遵循GPL协议的项目源码但并未公开原作者信息及修改部分<br />2020.4发布的本地版本使用了[Meowslib](https://github.com/CAIMEOX/meowslib)，但未遵守协议 |  | 2020.1发布的版本抄袭了于2019.8发布的Tr-func(彼时名为Tr&&ws&&sch&&pixe3.0) |
| 宣传真实性 |  |  | 严重的虚标速度欺骗用户，以建造速度为噱头诱导消费 |
| 消费者权益 |  |  |  |
| 目的可疑的命令使用 |  |  | /execute<br />/scoreboard<br />/tag |
| 不安全行为记录 | | | 向客户端发送包含错误UUID的数据包 |
|  |  |  |  |
| 截至本评测发布前<br />该列表提及问题已经修复 | No |  | No |
