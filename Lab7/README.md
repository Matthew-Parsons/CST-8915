# Youtube video link

# Analysis of RabbitMQ config issues
- Whether RabbitMQ is a stateless or stateful application
RabbitMQ is a stateful application as its data needs to persist between sessions.

- The implications of running RabbitMQ without persistent storage
Without a persistent storage, rabbitmq lacks the ability to retain data from previous sessions.

- What happens when the RabbitMQ pod is deleted or restarted
Since rabbitmq lacks persistent storage, any data present before a restart or deletion will be permanently lost.

- Potential solutions to this problem (research-based)


- Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
