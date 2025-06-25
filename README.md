# 🦀 Basic TCP Server in Rust

This is a simple TCP server built in Rust for learning and experimentation. It accepts incoming connections and handles them concurrently using threads. The project serves as a minimal and clean example of low-level network programming in Rust.

## 🚀 Features

- Listens on a TCP port and accepts incoming client connections
- Handles each client connection in a separate thread
- Gracefully handles socket read/write
- Written in safe, idiomatic Rust

## 📦 Dependencies

- [Rust](https://www.rust-lang.org/tools/install)
- No external crates — uses the standard library only

## 📁 Project Structure

```
.
├── Cargo.toml
└── src
    └── main.rs
```

## 🔧 Usage

### 1. Clone the repository

```bash
git clone https://github.com/Aditaya08/basic_rust_tcp.git
cd basic_rust_tcp
```

### 2. Build the project

```bash
cargo build --release
```

### 3. Run the server

```bash
cargo run
```

By default, it listens on `127.0.0.1:8080`. You can connect using `telnet`, `nc`, or your own TCP client:

```bash
telnet 127.0.0.1 8080
```

## 🧠 Concepts Covered

- Rust's `std::net::TcpListener` and `TcpStream`
- Thread-based concurrency
- Handling client input/output
- Basic error handling in networking

## 📜 Example Output

```text
Server listening on 127.0.0.1:8080
Incoming connection from 127.0.0.1:53926
Message received: Hello server!
```

## 🛠️ TODO

- Add support for configurable port and address via CLI
- Graceful shutdown handling
- Thread pool for better concurrency management

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Made by [Aditaya08](https://github.com/Aditaya08)
