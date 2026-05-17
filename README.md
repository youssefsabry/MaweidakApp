# MaweidakApp
# Maweidak (مواعيدك) — Medical Appointments App:  A bilingual (Arabic / English) medical appointment booking platform.  > Patients discover clinics and doctors, book appointments, receive reminders, and manage their visit history. Clinics and doctors manage their calendars, services, and bookings.

## 1. Architecture Overview

```
┌────────────────────────┐      HTTPS / JSON      ┌──────────────────────────┐
│   Flutter Mobile App   │  ───────────────────▶  │   FastAPI Backend (v1)   │
│  (Arabic + English RTL)│                        │  Repository + Service    │
└────────────────────────┘                        │  JWT Auth + Validation   │
                                                  └──────────┬───────────────┘
                                                             │ SQLAlchemy ORM
                                                  ┌──────────▼───────────────┐
                                                  │   PostgreSQL Database    │
                                                  └──────────────────────────┘
```
