# Nestjs Controller

- Responsible for handling incoming **requests** and returning **responses** to the client.

- Bound to a specific **path** (for example, "/tasks" for the task resources).

- Contains **handlers**, which handle **endpoints** and **request methods** (GET, POST, DELETE ...etc).

- Can take advantage of **dependency injection**
  to consume providers within the same module.

---

## Defining a controller

- A controller is defined by annotating a class with the _**@Controller**_ decorator.

- The decorator accepts a string, which is the **path** to be handled by the controller.

## Defining a Handler

- Handlers are simply methods within the controller class, decorated with decorators such as **@Get, @Post, @Delete** ...etc.
