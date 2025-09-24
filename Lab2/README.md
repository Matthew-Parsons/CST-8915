### Youtube video link:
https://youtu.be/lDVr0Q_asqE

## Reflection Questions
### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?
- Both were relegated to their own unique repositories to comply with the codebase factor
- Both changed from using hard coded values to environment variables to comply with the configuration factor
- Both have a file listing all of their dependencies to comply with the explicit dependency factor
- Both were modified to accept RabbitMQ despite it running from an outside source to comply with the Backing Services factor

### Why is it important to use environment variables instead of hard-coding configurations in your application?
Because using environment variables allows for, in the vast majority of cases, cleaner code that's easier to modify, as you can simply change the environment variables rather than sifting through all of your code and modifying each part, as well as better security, as you can hide important security details from users using environment variables while still letting the app function.

### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?
Because having separate repositories allows for each microservice to be worked on independently without compromising the integrity of the others accidentally. This also allows for each component to be upgraded and scaled as needed, rather than requiring each part to be upgraded/modified any time one of them needs to be scaled bigger.

## Repository Links to Services:
### Store Front
https://github.com/Matthew-Parsons/store-front

### Order Service
https://github.com/Matthew-Parsons/order-service

### Product Service
https://github.com/Matthew-Parsons/product-service