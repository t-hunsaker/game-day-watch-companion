# Data Flow

## Goal
Display current baseball game state on a Samsung smartwatch dashboard.

## Flow
1. GameChanger provides live game updates on the phone.
2. The phone companion app receives or derives current game state.
3. The phone app stores a single canonical GameState object.
4. The phone app syncs GameState to the watch.
5. The watch displays the latest state in a glanceable dashboard.

## Notes
- The system is state-based, not notification-based.
- The watch should show the latest known state, not a stream of events.
- If some fields are unavailable from the source, the app may support fallback/manual correction later.
