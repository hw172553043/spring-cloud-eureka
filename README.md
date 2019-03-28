##  SpringCloud入门实例    

eureka是一个高可用的组件，它没有后端缓存，每一个实例注册之后需要向注册中心发送心跳，在默认情况下erureka server也是一个eureka client，必须要指定一个 server。      

当client向server注册时，它会提供一些元数据，例如主机和端口，URL，主页等。Eureka server 从每个client实例接收心跳消息。 如果心跳超时，则通常将该实例从注册server中删除。     

注解@EnableEurekaClient 表明自己是一个eurekaclient（注册客户端）.          
注解@EnableEurekaServer 表明自己是一个eurekaserver (注册服务端)   

