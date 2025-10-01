## Youtube link: 
https://youtu.be/beXzSFzslqs

## Reflection Questions
### 1. What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?
I encountered some issues with getting the Web apps to build, due to either accidentally missing a step, or for the fact that my repositories from lab 2 had the lab 1 code for some reason, which i promptly fixed.

### 2. How does deploying microservices on Azure Web App Service differ from running them locally?
It differs as they must be accessed and hosted in different ways, as the way they build is different to the vm's we used for rabbitMQ and the store front, making use of github's build and deploy rather than any native tools in their language, and their hosting differs as well, being more of an actual website link rather than just a public IP.

### 3. Why is it important to use environment variables for configurations in a cloud environment?
As I said in lab 2, the reason for this is because using environment variables allows for, in the vast majority of cases, cleaner code that's easier to modify, as you can simply change the environment variables rather than sifting through all of your code and modifying each part, as well as better security, as you can hide important security details from users using environment variables while still letting the app function.