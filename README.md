# Service Taximeter

A small desktop application built with Python and Tkinter to track the duration of a task and estimate its cost based on an hourly rate.

The project was created as a simple utility for service-based work, where it can be useful to monitor time and get an immediate cost estimate without manual calculations.

## Demo

Here is the application in action:

**1. Start Screen**  
Ready to accept the hourly rate.  
![Start Screen](Start.png)

**2. Running**  
The timer updates both elapsed time and current cost in real time.  
![Running](Running.png)

**3. Stop & Result**  
Final cost shown when the session is stopped.  
![Stop Screen](Stop.png)

---

## Project idea

This application works like a very simple service timer:
- the user enters an hourly rate,
- starts the timer,
- lets it run during the activity,
- and stops it to get the final cost.

It is not meant to be a complete invoicing or task management system.  
The goal is to provide a small, clear, and usable desktop tool for basic time-and-cost tracking.

## Features

- **Elapsed time tracking** with a simple stopwatch-style interface
- **Real-time cost calculation** while the timer is running
- **Hourly rate input** with support for both `.` and `,` decimal formats
- **Basic state management** for Start, Stop, and Reset actions
- **Immediate feedback** through a clean Tkinter GUI

## How it works

The application uses:
- the Python `time` module to measure elapsed time,
- Tkinter's event loop to refresh the interface,
- and a simple formula to calculate the total cost:

```text
cost = (elapsed_seconds / 3600) * hourly_rate
```

The displayed value is updated continuously while the timer is active.

## Tech stack

- **Python 3**
- **Tkinter**

No external libraries are required beyond the Python standard library.

## Run the project

Make sure Python is installed, then run:

```bash
python taximeter.py
```

## File structure

- `taximeter.py` → main application file
- `Start.png` → screenshot of the initial state
- `Running.png` → screenshot while the timer is active
- `Stop.png` → screenshot of the final result

## Notes

This is a small standalone GUI project focused on:
- basic event-driven programming,
- interface state handling,
- and simple real-time calculation.

It is intentionally lightweight and does not include features such as:
- session history,
- file export,
- client management,
- or persistent storage.

## Possible improvements

Some possible next steps would be:
- saving completed sessions,
- adding a session description or client name,
- exporting results to CSV,
- packaging the app as an executable,
- and improving the interface styling.

---

**Author:** Andrea Melissari
