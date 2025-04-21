[![Stand With Palestine](https://raw.githubusercontent.com/TheBSD/StandWithPalestine/main/banner-no-action.svg)](https://thebsd.github.io/StandWithPalestine)



# Flutter Riverpod Best Practices

This repository serves as a sample Flutter project demonstrating best practices in Flutter development. It is structured to showcase modular architecture, state management with Riverpod, API handling with Dio, routing with `go_router`, and more. 

## Project Structure

This project follows a layered folder structure:

- **core**: Contains shared resources like common entities, services, and utilities.
- **features**: Modular features like authentication, dashboard, and home, each with its data, domain, and presentation layers.
- **di**: Dependency injection setup.
- **config**: Configuration and router setup.

## Key Features

- **Riverpod for State Management**: Efficient and scalable state management.
- **Dio for API Calls**: Handles HTTP requests and error handling.
- **Modular Architecture**: Easy to scale with a clean separation of concerns.
- **GoRouter for Routing**: Simplifies navigation across the app.


## 🧱 Layered Folder Structure

```
lib/
├── config/                        # Configuration files, including the router setup and global configuration
│   └── router/                    # Router configuration for navigation management
├── core/                          # Core utilities and shared resources
│   ├── common/                    # Common functionality shared across the app
│   │   ├── entities/              # Common data entities used throughout the app
│   │   ├── providers/             # Common providers used across features
│   │   ├── services/              # Shared services like logging, caching, etc.
│   │   └── widgets/               # Reusable widgets used throughout the app
│   ├── constants/                 # Constant values like strings, numbers, etc.
│   ├── error/                     # Error handling, custom error types, and utilities
│   ├── network/                   # Network-related utilities, e.g., API client, request handling
│   ├── usecase/                   # Business logic use cases or interactor classes
│   └── utils/                     # Helper functions and utilities for general tasks
├── di/                            # Dependency injection setup to manage dependencies
├── features/                      # Feature-based modular structure
│   ├── auth/                      # Authentication-related files and logic
│   │   ├── data/                  # Data layer for authentication (APIs, data models)
│   │   │   ├── datasources/       # Data sources for authentication (API calls, local storage)
│   │   │   ├── models/            # Models specific to authentication
│   │   │   └── repositories_impl/ # Implementation of repositories for authentication
│   │   ├── domain/                # Domain layer containing entities and business logic for authentication
│   │   │   ├── entities/          # Entities related to authentication (user, roles, etc.)
│   │   │   ├── repositories/      # Interfaces for repositories (e.g., user repo)
│   │   │   └── usecases/          # Use cases for authentication (login, register, etc.)
│   │   └── presentation/          # Presentation layer (UI and providers for authentication)
│   │       ├── providers/         # Riverpod providers related to authentication
│   │       ├── screens/           # Screens for login, signup, etc.
│   │       └── widgets/           # Widgets used in authentication screens
│   ├── dashboard/                 # Dashboard feature files and logic
│   ├── home/                      # Home feature files and logic
└── services/                      # Global services for the app (e.g., API service, storage)

```

## Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/kh1amirhamza/flutter_riverpod_best_practices.git
cd flutter_riverpod_best_practices
flutter pub get
```

Run the app:

```bash
flutter run
```

## Contributing

Feel free to contribute by submitting pull requests or opening issues.


## About Me

**Khandakar Amir Hamza**  
👨‍💻 Mobile App Developer (Flutter)  
📍 Dhaka, Bangladesh  
🔗 [LinkedIn](https://www.linkedin.com/in/kh1amirhamza)  
🔗 [GitHub](https://github.com/kh1amirhamza)

I specialize in building scalable, maintainable, and performance-optimized mobile applications using Flutter. Passionate about writing clean code and sharing knowledge with the community. Always open to collaboration and learning new technologies.

