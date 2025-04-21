# 📐 Project Architecture: Flutter Riverpod Best Practices

This project follows a Clean Architecture approach for large and scalable Flutter apps using:

- 🧠 **Riverpod** – State Management
- 🌐 **Dio** – HTTP Client
- 🧊 **Freezed** – Immutable Models & Sealed Classes
- 🪝 **Flutter Hooks** – Widget Lifecycle Simplification
- 🧭 **go_router** – Declarative Routing
---

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

## 🎯 Principles Followed

- **SOLID** principles
- Feature-first modularity
- Clear separation of concerns
- Reusable components and hooks
- Type-safe API + error handling

---

## 🧠 Riverpod Structure

- `xxx_provider.dart`: Encapsulate logic, state
- `xxx_state.dart`: Represent state classes (Freezed)
- `xxx_notifier.dart`: StateNotifier/AsyncNotifier

---

This project is ideal for beginners and intermediate devs who want to learn scalable Flutter practices.
