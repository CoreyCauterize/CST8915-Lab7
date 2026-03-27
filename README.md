# CST8915-Lab7

[Demo Video](https://youtu.be/rifPawKQHmk)


*   Whether RabbitMQ is a stateless or stateful application
    *   Right now, RabbitMQ is a stateless application
*   The implications of running RabbitMQ without persistent storage
    *   With RabbitMQ being stateless and without a persistent storage, means that any messages in the queue can be loss whenever RabbitMQ
*   What happens when the RabbitMQ pod is deleted or restarted
    *   What happens that the order-service is unable to process and orders, potentially losing orders.
*   Potential solutions to this problem (research-based)
    *   StatefulSet, Persistent Volume Clains, and RabbitMQ Cluster with persistent storage, and Azure Service Bus
*   Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
    *   Yes it does, since it is a managed service and is built to handle pressistence for mesaages in the queue.
