# Extracting Waiting Times from Free‑Text Messages

## Problem
Patients sometimes describe waiting times in free‑text. We need to extract all mentions of waiting time **in weeks** from a collection of messages.

## Data
A list of messages from patients (provided below).

## Method
Use Python's `re` module with a regular expression that finds a number (1‑2 digits) followed by the word "weeks".
