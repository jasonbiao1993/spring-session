# Spring Session 源码解析
* [Spring Session redis 缓存设计过期设计](http://www.iocoder.cn/Spring-Session/laoxu/spring-session-4//)
* [Spring-Session实现Session共享实现原理以及源码解析](https://www.cnblogs.com/aflyun/p/8532230.html)


### 注意
Spring Session + Redis实现分布式Session共享 有个非常大的缺陷, 无法实现跨域名共享session , 只能在单台服务器上共享session , 因为是依赖cookie做的 , cookie 无法跨域 pring Session一般是用于多台服务器负载均衡时共享Session的，都是同一个域名，不会跨域。你想要的跨域的登录，可能需要SSO单点登录
