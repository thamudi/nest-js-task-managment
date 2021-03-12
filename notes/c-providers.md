# NestJS Providers

- Providers can be injected into a constructor if decorated as an **@Injectable**, via **dependency injection**.

- Can be a plain value, classes, sync/async factory ...etc.

- Providers must be provided to a module for them to be usable.

- Can be exported from a module - and then be available to other modules that import it.

---

## What is a Service?

- Defined as providers. **Not all providers are services**.

- Singleton when wrapped with **@Injectable()** and provided to a module. That means, the same instance will be shared across the application - acting as a single source of truth.

- They are the main source of business logic. For example, a service will be called from a controller to validate data, create an item in the database and return a response.
