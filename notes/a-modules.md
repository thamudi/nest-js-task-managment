# NestJS modules

- Each app has at least one module - the root module.

- This is the starting point of the application.

- Modules are an effective way to organize components by closely related set of capabilities(e.g. per features)

- Modules are **singletons**, therefor a module can be imported by multiple other modules.

---

## Defining a module

- A module is defined by annotating a class with the _**@Module**_ decorator.

- The decorator provides metadata that NEST uses to organize the application structure.

---

## @Module Decorator Properties

- **providers**: Array of providers to be available within the module via dependency injection.

- **controllers**: Array of controllers to be instantiated within the module.

- **exports**: Array of providers to export to other modules.

- **imports**: List of modules required by the module. An exported provider by these modules will now be available in our module via dependency injection.

---
