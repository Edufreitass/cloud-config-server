# Spring Cloud Config Server

### This repository is linked to [spring-cloud-gateway-hystrix](https://github.com/Edufreitass/spring-cloud-gateway-hystrix)

- **application.yml** file configuration

```yml
eureka:
  client:
    register-with-eureka: true
    fetch-registry: true
    service-url:
      defaultZone: http://localhost:8761/eureka/
  instance:
    hostname: localhost
microservice:
  payment-service:
    endpoints:
      endpoint:
        uri: http://PAYMENT-SERVICE/payment/doPayment
  order-service:
    endpoints:
      endpoint:
        uri: http://ORDER-SERVICE/order/bookOrder
```
