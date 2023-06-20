# The Clean API Template 

## Introduction to Project
This project is a sample application that follows the principles of Clean Architecture in .NET Core. It provides a modular structure with separate layers for the API, application logic, domain entities, and infrastructure. The project incorporates popular frameworks and libraries such as ASP.NET Core, Entity Framework Core, MediatR, AutoMapper, FluentValidation, Serilog, and Swagger. With Docker support, the application can be easily containerized and deployed in a Docker environment.

## Introduction to Clean Architecture
Clean Architecture is an architectural pattern that emphasizes the separation of concerns and the independence of an application's business rules from the external frameworks and technologies it utilizes. It provides a structured approach to software development, promoting code maintainability, testability, and scalability.

Developed by Robert C. Martin (also known as Uncle Bob), Clean Architecture focuses on designing systems that are flexible, adaptable, and resistant to changes in requirements or technology choices. It encourages developers to create software that can evolve independently, with minimal impact on other parts of the system.

Each layer in Clean Architecture has a specific responsibility and encapsulates a different aspect of the application. The layers are organized in a way that allows for modularity, maintainability, and flexibility. The separation of concerns ensures that changes made to one layer have minimal impact on other layers.

<img width="400" alt="clean-removebg-preview" src="https://github.com/edinSahbaz/clean-api-template/assets/47791892/5d3afb3b-042e-417f-a7fd-75f6647d5118">

### Presentation Layer:
The Presentation Layer is responsible for handling the user interface and interaction. It includes components like web APIs, user interfaces, or command-line interfaces. This layer is primarily concerned with receiving user input, displaying information, and coordinating the flow of data between the user and the application.

### Application Layer:
The Application Layer contains the application-specific business logic and use cases. It acts as an intermediary between the Presentation Layer and the Domain Layer. This layer orchestrates the execution of use cases by coordinating the interactions between different components and applying business rules. It does not contain any infrastructure-related or implementation-specific details.

### Domain Layer:
The Domain Layer encapsulates the core business logic and entities of the application. It represents the heart of the system and contains business rules, entities, value objects, and domain-specific logic. The Domain Layer is independent of any external frameworks or technologies and should be the most stable and reusable part of the architecture.

### Infrastructure Layer:
The Infrastructure Layer handles external concerns and provides implementations for data access, external services, frameworks, and other infrastructure-related code. It includes components like databases, file systems, third-party APIs, and external integrations. The Infrastructure Layer interacts with the external world, enabling the application to store and retrieve data, communicate with external systems, and handle cross-cutting concerns like logging or caching.

### Persistence Layer:
The Persistence Layer is a specific type of infrastructure layer that deals with data persistence and storage. It includes implementations of repositories, data mappers, or Object-Relational Mapping (ORM) frameworks. This layer provides the necessary mechanisms to persist and retrieve domain entities and data from a database or other storage systems.

## Benefits Using of Clean Architecture
### Maintainability: 
Clean Architecture separates concerns and reduces code dependencies, making it easier to understand and modify individual components without impacting the entire system.

### Testability: 
Clean Architecture promotes thorough unit testing by isolating business logic from external dependencies, allowing for focused and reliable testing of core application functionality.

### Scalability: 
The modular structure of Clean Architecture enables independent scaling of specific components or layers, ensuring optimal performance and resource allocation.

### Technology Independence: 
Clean Architecture decouples the core business logic from implementation details, enabling flexibility in adopting new technologies or frameworks without extensive code changes.

### Flexibility and Adaptability:
Clean Architecture allows for easier modification and evolution of the system as requirements change, thanks to the separation of concerns and minimal ripple effects across the codebase.

### Code Reusability: 
Clean Architecture promotes the creation of reusable code by keeping core business logic separate, reducing duplication, and improving development efficiency.
