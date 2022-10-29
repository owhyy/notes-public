---
title: Statelessness
created: 2022-08-17
keywords: [Backend, Programming]
---

> The API server shouldn't rely on information from previous requests in order to work correctly.

# Application state vs Resource state

- Application -- what the server shouldn't depend on (aka information about the client, what he did on a site, authentication credentials, everything stored on the server to "help him understand a request")
- Resource -- what you save in the database (aka what is returned from a GET request)

- For a [[9u1p-untitled|Websocket]], the server depends on previous information, because the connection lasts longer that for a HTTP request
