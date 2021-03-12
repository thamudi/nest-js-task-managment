# Data transfer Objects

> "A Data transfer object (DTO) is an object that carries data between processes." - ["Data Transfer Object", Wikipedia](https://en.wikipedia.org/wiki/Data_transfer_object)

---

> "A Data Transfer Object is an object that is used to encapsulate data, and send it from one subsystem of an application to another." - ["What is Data Transfer Object", StackOverflow](https://stackoverflow.com/a/1058186)

---

> "A DTO is an object that defines how the data will be sent over the network." - [NestJS Documentation](https://docs.nestjs.com/controllers#request-payloads)

---

## More about DTOs

- Common concept in Software development that is not specific to NestJS.

- Result in more bulletproof code, as it can be used as a TypeScript type.

- Do not have any behavior except for storage, retrieval, serialization and deserialization of its own data.

- Result in increased performance (although negligible in small applications).

- Can be useful for data validation.

- A DTO is **NOT** a model definition. It defines the shape of the data for a specific case, for example - creating a task.

- Can be defined using an **interface** or a **class**.
  - The recommended approach is to use classes, also clearly documented in the NestJS documentation.
  - The reason is that interfaces are a part of Typescript and therefore are not preserved post-compilation.
  - Classes allow us to do more, and since they are part of Javascript, they will be preserved post-compilation.
  - NestJs cannot refer to interfaces in run-time, but can refer to classes.
