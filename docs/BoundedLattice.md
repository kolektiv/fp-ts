---
id: BoundedLattice
title: Module BoundedLattice
---

[← Back](.)

[Source](https://github.com/gcanti/fp-ts/blob/master/src/BoundedLattice.ts)

# BoundedLattice

```ts
interface BoundedLattice<A> extends BoundedJoinSemilattice<A>, BoundedMeetSemilattice<A> {}
```

Added in v1.4.0 (type class)

A `BoundedLattice` must satisfy the following in addition to [BoundedMeetSemilattice](./BoundedMeetSemilattice.md) and [BoundedJoinSemilattice](./BoundedJoinSemilattice.md) laws:

- Absorbtion law for meet: `a ∧ (a ∨ b) == a`
- Absorbtion law for join: `a ∨ (a ∧ b) == a`
