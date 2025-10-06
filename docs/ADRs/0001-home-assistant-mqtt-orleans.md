# ADR 0001: Home Assistant MQTT Orleans Architecture

## Status

Proposed

## Context

We need to design a system that integrates Home Assistant with Orleans using MQTT as the message broker.

## Decision

We will use the following architecture:
- Orleans for distributed actor-based processing
- MQTT as the message broker for Home Assistant integration
- Aspire for orchestration and service discovery

## Consequences

### Positive
- Scalable distributed processing with Orleans
- Reliable message delivery with MQTT
- Easy integration with Home Assistant

### Negative
- Additional complexity from distributed system
- Need to manage Orleans cluster
