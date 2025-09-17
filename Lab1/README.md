## youtube video link

## Technical explanations

### Store Front
The store front written in Vue.js, and is the responsible for the UI; providing the customer with clear visuals of what is being offered and what they're buying. It also checks to see if a customer is submitting a valid order.

### Product Service
The product service is written in Rust, responsible for communicating to the store front what is being offered. It sends the store front the store items currently available for purchase in a json format, and the store front converts those jsons into UI elements that the customer can interact with.

### Order Service
The order service is written in Node.js, and is responsible for handling customer transactions. when someone submits a valid order, the store front sends the order info to order service, which sends the data to RabbitMQ to process the transaction.

