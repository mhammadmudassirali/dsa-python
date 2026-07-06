# Two Sum

## Problem

Given an array and a target, return the indices of two numbers that add up to the target.

---

## Brute Force

### Idea

Compare every pair.

### Algorithm

Use two nested loops.

### Time Complexity

O(n²)

### Space Complexity

O(1)

### Why is it slow?

We repeatedly scan the array looking for the complement.

---

## Optimized

### Observation

For every number,

complement = target - current_number

Instead of searching again,
store previously seen numbers.

### Data Structure

Dictionary

value -> index

### Algorithm

1. Create empty dictionary
2. Compute complement
3. If complement exists return answer
4. Otherwise store current number

### Time Complexity

O(n)

### Space Complexity

O(n)

---

## Pattern

Hash Map

---

## What I Learned

Instead of searching repeatedly,
remember previous values.

Hash Maps convert repeated searching
into constant-time lookup.
