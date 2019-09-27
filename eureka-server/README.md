

## SpringCloud Eureka

- 基于NetFlix Eureka做了二次封装
- 两个组件构成（Eureka Server和Eureka Client）

### Eureka Server（注册中心）
- 相当于老师手中的名单，应用叫什么名字，在哪台服务器上，现在有没有在工作
- Eureka单词意为找到了

步骤：
- 1.创建SpringBoot项目，勾选Eureka Server选项（导入依赖）
- 2.注意SpringBoot和SpringCloud对应的版本
- 3.在启动类上添加注解@EnableEurekaServer
- 4.在yml文件中配置端口号和不把自己注册到注册中心
### Eureka Server集群
- Eureka Server互相注册
- 当另一个Client注册到其中的一个Eureka Server中去的时候，另外一个Eureka Server注册中心中也会有这个Client的数据
