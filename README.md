# FelixRPC
一个自制的简易RPC框架

# 项目依赖
| name         | 定义         | 功能                                                         |
| ------------ | ------------ | ------------------------------------------------------------ |
| rpc-provider | 服务提供者   | 负责发布RPC服务，接收和处理RPC请求                           |
| rpc-consumer | 服务消费者   | 使用动态代理发起RPC远程调用，帮助使用者来屏蔽底层网络通信的细节 |
| rpc-registry | 注册中心模块 | 提供服务注册、服务发现、负载均衡的基本功能                   |
| rpc-protocol | 网络通信模块 | 包含RPC协议的解编码器、序列化和反序列化工具等                |
| rpc-core     | 基础类库     | 提供通用的工具类以及模型定义，例如RPC请求和响应类、RPC服务元数据等 |
| rpc-facade   | RPC服务接口  | 包好服务提供者需要对外暴露的接口。本模块主要用于模拟真实RPC调用的测试 |