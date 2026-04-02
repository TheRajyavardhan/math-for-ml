# Day 7.1 — Laplace Smoothing

## Problem
Naive Bayes fails when a feature has zero probability.

If any P(x_i | C) = 0 → entire probability becomes 0.

## Solution
Laplace Smoothing (Add-1 Smoothing)

## Formula
P(x_i | C) = (count(x_i, C) + 1) / (total words in C + V)

Where:
- +1 avoids zero probability
- V = vocabulary size

## Why Needed
- Prevents zero probability
- Improves model robustness
- Handles unseen data

## Insight
Never assume something is impossible just because it hasn't been seen before.

## Use Cases
- Spam detection
- NLP models
- Text classification

