---
title: Redis Hashses
created: 2022-08-06
keywords: [Redis, Backend, Python, Programming]
---

## [[8jzn-untitled]] Hashses

- `hset` and `hget`
- You can only acces the _keys_, but not the _values_
- Cool feature -- saving to disk is smart by default (saves the database every 60 seconds if 1000+ keys were changed, all the way to 15 minutes if 9 changed). Untill written to disk, everything is kept in RAM
- _Append-only_ means that you can only add(_insert_) data
- **Page 16 has a good tip about using hashing, but I don't quite understand it yet**
