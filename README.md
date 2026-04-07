 Actix-Web User API

A lightweight, high-performance REST API built with **Rust**. This project serves as a practical dive into Rust's ownership model and thread-safe state management using the Actix-web framework.

Key Features

* **Thread-Safe State**: Uses `Arc<Mutex<HashMap>>` to share data safely across multiple CPU cores.
* **Async/Await**: Non-blocking I/O powered by the `Tokio` runtime.
* **JSON Ready**: Automatic serialization and deserialization via `Serde`.
* **Type Safety**: Leverages Rust's strict compiler to catch bugs at compile time.

Tech Stack

- **Framework:** [Actix-web](https://actix.rs/)
- **Serialization:** [Serde](https://serde.rs/)
- **Language:** Rust 2021 Edition

📡 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/users/{id}` | Fetch a user profile by ID |
| `POST` | `/users` | Create a new user (JSON body) |

Getting Started
1. **Clone the repo**
2.Run the server
   cargo run

Lessons Learned
The Borrow Checker: Managing shared state without data races.

Extractors: How Actix-web pulls data directly from URL paths and JSON bodies.

Arc & Mutex: Understanding why we need Atomic Reference Counting for multi-threaded access.
   ```bash
   git clone [https://github.com/ManthanN75/Actix_server.git](https://github.com/ManthanN75/Actix_server.git)
