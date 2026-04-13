---
title: What Runs On Data-Centre CPUs
type: evergreen
status: draft
tags:
  - compute
  - software
  - data-centres
---

# What Runs On Data-Centre CPUs

[[AI Infrastructure Hub]]

## Core idea

Most people associate data centres with websites and AI models, but CPUs still do a huge amount of the general-purpose work that keeps those systems alive.

## Typical workloads

- web servers and APIs
- databases
- storage controllers
- virtualization and hypervisors
- Kubernetes control planes
- monitoring, logging, and security agents
- business applications and internal enterprise systems

## Relationship to GPUs

GPUs handle highly parallel numerical workloads well. CPUs still orchestrate, schedule, preprocess, serve, manage storage, and run most of the surrounding platform software.

## Why this note matters

It is easy to reduce modern infrastructure to "GPUs for AI." In practice, the full system still depends on a broad software estate running on CPUs.
