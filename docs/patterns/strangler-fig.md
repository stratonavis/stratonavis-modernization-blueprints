# Strangler Fig Pattern

## Overview

The Strangler Fig pattern enables gradual replacement of legacy systems by building new functionality around the existing system.

---

## Why It Matters

Enterprise systems cannot afford:
- Downtime
- High-risk rewrites
- Business disruption

This pattern allows safe, incremental evolution.

---

## When to Use

- Legacy systems with high business dependency
- Systems with unclear internal structure
- Situations requiring zero downtime migration

---

## Implementation Steps

1. Identify bounded context within legacy system
2. Build new service outside the legacy system
3. Route specific functionality to new service
4. Gradually reduce dependency on legacy system
5. Decommission legacy components

---

## Benefits

- Reduced risk
- Continuous delivery
- Business continuity

---

## Common Mistakes

- No domain boundaries defined
- Mixing old and new logic
- Lack of observability

---

## Real-World Example

A financial transaction system gradually migrated to an event-driven architecture using Kafka and microservices while maintaining existing operations.

---

## Key Insight

> The goal is not to replace the system.  
> The goal is to **outgrow it**.
