# Youtube video link
https://youtu.be/pgYAehRmCDw

# Analysis of RabbitMQ config issues
### - Whether RabbitMQ is a stateless or stateful application
RabbitMQ is a stateful application as its data needs to persist between sessions.

### - The implications of running RabbitMQ without persistent storage
Without a persistent storage, rabbitmq lacks the ability to retain data from previous sessions.

### - What happens when the RabbitMQ pod is deleted or restarted
Since rabbitmq lacks persistent storage, any data present before a restart or deletion will be permanently lost.

### - Potential solutions to this problem (research-based)
One solution to this problem would be to use another service similar to rabbitmq that has easy access to persistant storage, like azure service bus.

### - Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
Yes it does, as azure service bus is essentially azure's version of rabbitmq, meaning that we could replace our rabbitmq with it, and see the same if not better results, as azure service bus would have the ability to easily use persistant storage.