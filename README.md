# Dubbo Spring Boot Sample CD

This repo demonstrates how to continuos deploy a service consists of multiple versioned microservices.

The application consists of 2 microservices: `provider` and `consumer`, both are implemented using [zhuohao.li/dubbo-spring-boot-samples-upgrade](https://gitlab.daocloud.cn/zhuohao.li/dubbo-spring-boot-samples-upgrade).

They talk in following way:

client -> gateway -> consumer -> provider

We have 2 branches:

1. `release-v1.0`: the initial version of the service, with `provider` version `1.0` and `consumer` version `1.0`.
2. `release-v2.0`: the upgraded version of the service, with `provider` version `2.0` and `consumer` version `2.0`.