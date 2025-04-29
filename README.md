# aw08

Please extend your MicroPOS system by adding a delivery service shown as the following figure (it's not necessary that your MicroPOS system has a same layout of microservices as in this figure).

![](10-pos.svg)

When an order is placed by a user, the order serivce sends out an event into some AMQP MOM (such as RabbitMQ). The delivery service will be notified and a new delivery entry will be generated automatically. User can query the delivery status for his orders.

You can refer to the [guide project](https://github.com/spring-guides/gs-spring-cloud-stream) for technical details.
