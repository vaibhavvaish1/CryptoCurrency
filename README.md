Cryptocurrency App - README

Overview

This is a cryptocurrency application built using Clean Architecture principles in Kotlin. The app provides features such as real-time cryptocurrency price tracking, detailed coin information, and market analysis.

The application is structured into the following layers:

1. Domain Layer

Purpose: Contains the core business logic and use cases.

Components:

Entities: Plain Kotlin data classes representing core data structures.

Use Cases: Business logic as reusable, testable, and independent units.

Interfaces: Abstract definitions for repositories.

2. Data Layer

Purpose: Handles data sources and implements repository interfaces.

Components:

Repository Implementations: Acts as a bridge between data sources and domain layer.

Local Data Source: Room database for caching data offline.

Remote Data Source: Retrofit-based implementation for fetching data from a cryptocurrency API.

3. Presentation Layer

Purpose: Manages the UI and user interactions.

Components:

ViewModels: Expose data to the UI and handle user actions.

UI Components: Jetpack Compose-based screens.
