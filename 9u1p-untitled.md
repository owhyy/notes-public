---
title: WebSocket vs HTTP
created: 2022-08-17
keywords: [Programming, Backend]
---

# HTTP

- Flow: user creates request -> [[r2i1-tcp]]# connection is created -> server gives response -> TCP connection is closed

# WebSocket

- Flow: connection is created and kept alive untill either server or user closes it
- Used when changes need to be displayed in real-time
