# Contributing to ToolBox Robotics

First off, thank you for considering contributing to ToolBox Robotics! It's people like you that make the open-source community such an amazing place to learn, inspire, and create.

Whether you're fixing a bug, porting to a new ROS version (like ROS2), improving documentation, or designing new end-effectors, we welcome your help.

## Table of Contents

1.  [How to Contribute](#how-to-contribute)
2.  [Reporting Bugs](#reporting-bugs)
3.  [Suggesting Enhancements](#suggesting-enhancements)
4.  [Pull Request Process](#pull-request-process)
5.  [Coding Standards](#coding-standards)
6.  [Hardware Safety & Testing](#hardware-safety--testing)

---

## How to Contribute

There are many ways to contribute:

* **Software:** Improvements to the ROS packages, MoveIt configurations, or control scripts.
* **Firmware:** Updates to the microcontroller code (Arduino/Teensy/ESP32).
* **Documentation:** Fixing typos, adding setup guides, or translating instructions.
* **Hardware/CAD:** Suggestions for mechanical improvements (please open an Issue to discuss these first).

## Reporting Bugs

This section guides you through submitting a bug report.

* **Check existing issues** to see if the bug has already been reported.
* **Open a new Issue** using the provided template.
* **Include details:**
    * Which arm model are you using? (e.g., EB-65, EB-15)
    * Which ROS distribution? (e.g., Noetic, Humble)
    * Are you running in Simulation (Gazebo) or Real Hardware?
    * Steps to reproduce the error.

## Suggesting Enhancements

If you have an idea for a new feature (like ROS2 support) or a change in architecture:

* **Start a Discussion** or open an Issue titled "Proposal: [Feature Name]" before writing code. This allows us to discuss the implementation and ensures your work aligns with the project roadmap.

## Pull Request Process

1.  **Fork the repo** and create your branch from `main`.
2.  **Test your code.** If you are modifying control logic, please verify it in simulation first.
3.  **Update documentation.** If you changed APIs or setup procedures, update the `README.md` accordingly.
4.  **Submit the PR.** Provide a clear description of what you changed and why.

## Coding Standards

* **Python:** Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/).
* **C++:** Follow standard ROS C++ style guides.
* **Commits:** Write clear, concise commit messages (e.g., "Fix IK solver convergence issue" rather than "fixed bug").

## Hardware Safety & Testing

**CRITICAL:** Because this software controls physical robotic hardware, safety is paramount.

1.  **Simulation First:** All control changes *must* be tested in Gazebo/RViz before being attempted on real hardware.
2.  **Warning Labels:** If your PR involves changes to motor currents, velocity limits, or safety stops, explicitly state this in the PR description.
3.  **Disclaimer:** Code merged into this repository is provided "as is". Contributors are expected to verify that their changes do not cause physical damage to the actuators or structural components.

---

Thank you for helping us make robotics accessible to everyone!

– The ToolBox Robotics Team
