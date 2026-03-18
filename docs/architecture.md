# Architecture

GameChanger App
        ↓
Phone Companion App (State Engine)
        ↓
Wear OS Watch App (Dashboard)

## Key Principle
The system is state-driven, not event-driven.

The phone maintains a single GameState object that is continuously updated and synced to the watch.
