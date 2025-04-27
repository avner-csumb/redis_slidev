---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Redis
info: CST 363
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
# seoMeta:
#  ogImage: https://cover.sli.dev
---

# Redis

CST 363


---
transition: fade-out
---

# What is Redis?

Redis is the archetype of in-memory key–value stores.

- Virtually every production system uses Redis (or an equivalent) for caching, sessions, rate-limiting, real-time messaging, and lightweight queues. It's a staple of "database adjacencies."
- Redis's persistence modes (RDB snapshots vs. AOF logs) highlight trade-offs between durability, performance, and recovery 
- Powerful Pub/Sub mechanism
<br>
<br>


---

## Core Data Structures  

- **String**: arbitrary byte values  
- **Hash**: maps of fields → values  
- **List**: ordered collections  
- **Set**: unique, unordered collections  
- **Sorted Set**: scored, ordered collections  

---

## Atomic Operators --- KV Store

<br>
Strings - O(1) 

- GET key
- SET key value 
- EXISTS key 
- DEL key