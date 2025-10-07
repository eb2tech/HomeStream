# C4 Context Diagram

## System Context

```
┌──────────────────┐
│  Home Assistant  │
└────────┬─────────┘
         │
         │ MQTT
         │
┌────────▼─────────┐
│   HomeStream     │
│                  │
│  - Orleans       │
│  - MqttBridge    │
│  - Projections   │
│  - Aspire        │
└──────────────────┘
```

## Description

HomeStream acts as a processing layer between Home Assistant and various downstream systems, using Orleans for distributed processing and MQTT for reliable message delivery.
