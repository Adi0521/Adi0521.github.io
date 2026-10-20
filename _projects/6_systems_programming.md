---
layout: page
title: Linux Systems Programming
description: Shell, allocator, servers, and OS internals in C (CS 341)
importance: 6
category: more
---

**Stack:** C, POSIX, pthreads, sockets, epoll

Systems work built for UIUC's CS 341.

- **Shell:** a Unix shell with fork/exec process management, background jobs, signal handling, I/O redirection, command history, and a /proc-based `ps`
- **Memory:** a custom heap allocator (malloc/calloc/realloc/free) and a memory-leak checker
- **Networking:** a TCP chat server and an epoll-based, non-blocking file server with a custom client-server protocol
- **Concurrency:** a dependency-graph parallel make and a parallel password cracker with pthreads, plus barriers, semaphores, and deadlock detection
- **OS internals:** CPU scheduling policies (FCFS, SJF, round robin, priority), virtual memory (MMU/TLB), a MINIX-style file system, and MapReduce
