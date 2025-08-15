# MathWorks Minidrone Competition Entry - [Your Team Name]

A fully autonomous navigation and landing system for a Parrot Minidrone, developed in MATLAB and Simulink for the [Year] competition. This project demonstrates a complete control system pipeline, from vision processing to high-level state machine logic.

## Simulation Demo

![WhatsAppVideo2025-08-15at16 41 25-ezgif com-video-to-gif-converter(1)](https://github.com/user-attachments/assets/1195d681-0249-42e4-af46-91ecb5c3d417)

## Key Features

- **9-State Finite State Machine:** Manages the entire mission logic from takeoff to landing, including complex state transitions.
- **Robust Vision System:** Utilizes the Computer Vision Toolbox to create a reliable pipeline. It uses image cropping (region of interest) to isolate the path ahead, and blob analysis to extract centroid, orientation, and eccentricity.
- **Hybrid Position/Attitude Controller:** Employs Position Control for stable, waypoint-based flight and Attitude Control for precise, on-the-spot turns.
- **P-Controller for Line Tracking:** A tuned Proportional controller ensures the drone stays centered on the line during forward flight.
- **Advanced Maneuvers:** The controller successfully handles corner detection, deceleration with braking distance anticipation, and post-turn re-centering.
- **Safe Landing Sequence:** Includes a terminal guidance phase to precisely center over the landing pad before executing a controlled descent.

## Technologies Used

- MATLAB
- Simulink
- Stateflow (logic implemented in a MATLAB Function block)
- Computer Vision Toolbox

## How to Run

1. Ensure all required toolboxes are installed (as per the competition PDF).
2. Open the `MinidroneCompetition.prj` file in MATLAB. This will set up the necessary project paths.
3. Open the main Simulink model: `asbQuadcopter.slx` (or the correct name of the main model file).
4. Run the simulation.
