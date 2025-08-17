# Computer Science Project — Web Server in C

This repository contains a minimal web server implemented in C for a public computer science class. The server is designed for learning systems and networking fundamentals (sockets, HTTP parsing, concurrency) and to be extended with features such as TLS, caching, and benchmarking.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Progress Tracker](#progress-tracker)
- [Build and Run](#build-and-run)
- [Usage Examples](#usage-examples)
- [Testing](#testing)
- [Roadmap / Stretch Goals](#roadmap--stretch-goals)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Notes](#notes)

## Overview

A compact, single-process or multi-threaded HTTP server implemented for learning:

- Accepts TCP connections and parses simple HTTP requests.
- Serves static files from a configurable document root.
- Demonstrates concurrency strategies (thread pool or event loop).
- Simple logging and error handling for educational purposes.

## Features

- Serve static files with correct MIME types.
- Support for HTTP/1.0 and basic HTTP/1.1 request handling.
- Concurrent request handling (select/poll/epoll or thread pool — configurable).
- Simple request logging and configurable document root.
- Small, well-commented C codebase intended for modification and extension.

## Progress Tracker

- [ ] Project scaffold and README
- [ ] Basic TCP listener and accept loop
- [ ] Simple request parsing and response (GET)
- [ ] Static file serving with Content-Type
- [ ] Basic error responses (404, 400, 500)
- [ ] Concurrency: thread pool implementation
- [ ] Concurrency: event-driven (epoll/kqueue) implementation
- [ ] Support persistent connections and chunked responses
- [ ] Range requests / partial content
- [ ] Graceful shutdown and signal handling
- [ ] Unit and integration tests for handlers
- [ ] HTTPS (TLS) support via OpenSSL or mbedTLS
- [ ] Reverse proxy / load balancing example
- [ ] Benchmarking against nginx/Apache for simple workloads
