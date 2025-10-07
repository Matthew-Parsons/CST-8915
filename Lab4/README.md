# Youtube Video Link
https://youtu.be/o0B_LFmYWJI

# Reflection Questions
## 1. What are the main differences between a Docker image and a Docker container?
The difference between the two is that an image is essentially an immutable snapshot of a container. Images cannot be changed, but can be used by anyone to create a container, like a blueprint. Containers are instances of an image. they can be modified from the original image, and you can create as many instances from an image as you want, provided your machine can handle it, as unlike images, containers cost computing resources.

## 2. Explain how Docker's layered architecture improves efficiency.
It improves efficiency, as when you push out a new build, any layer that has not been modified will use the previously cached layer rather to save time and resources rather than rerunning everything again. this leads to faster builds with more efficient space storage across different images, as multiple images can make use of the same layer rather than each having their own individual layer.

## 3. Why does each container get its own writable layer?
Containers get their own writable layer in order to allow them to make changes to their filesystem without modifying the underlying image layers, which are read-only.

## 4. What are the benefits of using Docker Compose over running containers individually?
Using compose streamlines the setup of multi-container applications, allowing for everything to be defined and run using a single YAML file. It allows for the documentation and configuration of all of your application's dependencies in a single file. It also allows you to set up automated testing environments that you can create and destroy with just a few commands.