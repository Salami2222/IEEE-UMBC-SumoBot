# IEEE UMBC Sumobot — Creatine Crackheads 🤖

**IEEE Region 1 & Region 2 Joint Student Activities Conference — Spring 2026**
**🏆 1st Place — Finished ahead of 15 competing teams**

---

## Team

| Name | Role |
|------|------|
| Tommy Pham | Hardware + Software + Strategy | 
| Jacob Lontoc | Hardware + Firmware |
| Isaac Boteler | Software 

---

## Project Overview

Our robot was built on the **Zumo 32U4** platform, competing on a 30-inch sumo ring. The software stack combines fast opponent detection, boundary awareness, aggressive cross-ring movement, and a tuned close-range attack routine — all of which contributed to our first-place finish.

### Repository Structure

```
IEEE-UMBC-sumobot/
├── sumobot-starter-code/   # Arduino sketch + sensor header
├── documentation/          # Project write-up, hardware notes, media
├── meeting-notes/          # Dated planning & research notes
└── README.md
```

---

## Robot Behavior

The sketch implements a **state-driven competition loop**:

1. **Countdown + Opening Scan** — brief delay followed by a directional sweep to locate the opponent
2. **Cross-Ring Drive** — aggressive forward push to force early contact
3. **Bounce Search** — oscillating search pattern when no opponent is detected
4. **Attack + Reacquire** — multi-phase attack routine that re-locks onto the opponent after evasion
5. **Boundary Detection** — reflectance-based edge detection to keep the robot inside the ring

---

## Hardware

- **Platform:** Pololu Zumo 32U4
- **Ring Size:** 30-inch diameter sumo ring
- **Sensors:** IR proximity (opponent detection), reflectance array (boundary detection)
- **Motors:** Built-in dual gear motors via Zumo motor driver

---

## Development Timeline

### Meeting Schedule
**Every Friday, 1:00 – 3:00 PM | UMBC Library**

| # | Date | Status |
|---|------|--------|
| Pre-meeting | Jan 28, 2026 | ✅ |
| Meeting 1 | Feb 6, 2026 | ✅ |
| Meeting 2 | Feb 13, 2026 | ✅ |
| Meeting 3 | Feb 20, 2026 | ✅ |
| Meeting 4 | Feb 27, 2026 | ✅ |
| Meeting 5 | Mar 6, 2026 | ✅ |
| Meeting 6 | Mar 13, 2026 | ✅ |
| Meeting 7 | Mar 20, 2026 | ✅ |

### Key Dates
- **Build Deadline:** March 19, 2026
- **Competition Day:** March 20, 2026

---

## Development Checklist

- [x] Solder & assemble robot
- [x] Design state machine architecture
- [x] Implement basic states (idle, search, drive)
- [x] Implement attack state
- [x] Implement search state
- [x] Boundary detection & avoidance

---

## Documentation

- [Project Documentation](documentation/project-documentation.md)
- [Meeting Note 01 — Jan 28](meeting-notes/meeting-01-2026-01-28.md)
- [Meeting Note 02 — Feb 6](meeting-notes/meeting-02-2026-02-06.md)
- [Meeting Note 03 — Feb 13](meeting-notes/meeting-03-2026-02-13.md)

---

## Getting Started

1. Install the [Arduino IDE](https://www.arduino.cc/en/software)
2. Install the [Pololu Zumo 32U4 library](https://github.com/pololu/zumo-32u4-arduino-library)
3. Open `sumobot-starter-code/sumobot-starter-code.ino`
4. Connect your Zumo 32U4 via USB and upload

---

*Built  by Team Creatine Crackheads — IEEE UMBC, Spring 2026*
