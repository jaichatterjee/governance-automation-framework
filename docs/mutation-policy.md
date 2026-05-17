# Mutation Policy

## Purpose

Mutation controls changes to authoritative artifacts and prevents uncontrolled modification.

---

## Baseline States

| State | Description |
|---|---|
| READ-ONLY | Analysis permitted, modification prohibited |
| MUTABLE | Explicit updates allowed |
| LOCKED | Immutable reference |
| DEPRECATED | Historical reference |

---

## Allowed Actions

| Action | Allowed |
|---|---|
| Explicit approved update | ✅ |
| Silent modification | ❌ |
| Implicit normalization | ❌ |
| Version overwrite | ❌ |

---

## Principles

- Mutation must be intentional
- Changes must remain traceable
- Historical states should be preserved
