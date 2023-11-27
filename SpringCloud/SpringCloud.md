# Spring Cloud

## 微服务

## 注册中心

## Ribbon 负载均衡
### 自旋锁

## Http 请求
### Rest Template
### Feign(整合了Ribbon)

## Hystrix 熔断器
### 服务降级 fallback
### 服务熔断 break
### 服务限流 flowlimit

## Gateway 网关
### 路由 Routes
### 断言 Predicate
### 过滤器 Filter

## Bus 消息总线

### 全局通知
curl -X POST "http://localhost:3344/actuator/bus-refresh"

### 定点通知
curl -X POST "http://localhost:3344/actuator/bus-refresh/config-client:port"
不加端口时为整个集群

### 结构图
![结构图](/Users/hanwenhao/Cloud/笔记/并发与分布式/SpringCloud/消息总线.png)

