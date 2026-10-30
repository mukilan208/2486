# 2486

**Smart Traffic Management System** — a fully interactive, zero-dependency web prototype that demonstrates how AI-driven signal control reduces congestion and gives emergency vehicles an automatic green corridor.

## Features

- **Dashboard** — live KPIs: vehicles detected, current congestion level, active signals, emergency vehicles detected, average wait time, overall traffic status (Low / Medium / High)
- **Live Traffic Map** — animated city grid with 8 signalized intersections, moving vehicles that queue at red lights, real-time density indicators (green / yellow / red), click any intersection for details
- **Adaptive Signal Control** — green durations auto-tuned to live density (busier approach → longer green, up to 55s); per-signal countdowns; manual override per signal (force NS/EW green, +5s, auto/manual mode, repair)
- **Emergency Vehicle Priority** — ambulance / fire truck / police simulation with automatic green-corridor preemption along the route, live ETA, route progress, cancel control, and response-time-saved statistics
- **Traffic Analytics** — vehicles-per-hour bar chart, congestion distribution doughnut chart, 7-day average-wait-time comparison (fixed timers vs AI adaptive), improvement KPIs
- **Alerts & Notifications** — congestion, emergency, signal-fault and anomaly alerts with toast popups, severity filters and acknowledge actions
- **Dark / Light mode** (persisted) and fully responsive layout — desktop, tablet and mobile

## Run

No build step and no dependencies — open `index.html` directly in any modern browser, or serve it:

```bash
python3 -m http.server 8080
# → http://localhost:8080
```

## Tech

Single-file vanilla HTML + CSS + JavaScript. All charts, icons and the animated city map are hand-rolled SVG — works fully offline.

## Files

| File | Description |
|---|---|
| `index.html` | Complete Smart Traffic Management System prototype |

---

*Demo data is simulated in the browser for demonstration purposes.*
