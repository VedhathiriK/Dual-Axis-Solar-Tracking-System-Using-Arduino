Dual Axis Solar Tracking System Using Arduino UNO


This project implements a Dual Axis Solar Tracker that automatically adjusts a solar panel in both horizontal and vertical directions to maintain maximum exposure to sunlight. The system uses an Arduino UNO, LDR sensors, and servo motors to detect the brightest light source and position the panel accordingly.

📌 Features:


Tracks sunlight along two independent axes

Uses four LDR sensors for directional light detection

Smooth servo adjustments for accurate panel positioning

Auto standby mode during low-light or night conditions

Compact, efficient, and beginner-friendly design


📦 Components Required:

Hardware:

Component	Quantity
Arduino UNO	1
LDR Sensor (5mm)	4
Micro Servo Motor	2
10kΩ Resistor	4
Breadboard	1
Jumper Wires	—
Solar Panel (optional)	1

Software:

Arduino IDE

⚡ Circuit Overview:

The system uses four LDR sensors arranged in a cross pattern:
Top-Left, Top-Right, Bottom-Left, Bottom-Right

Each LDR is paired with a 10kΩ resistor to form a voltage divider. The Arduino reads the changing voltage values to determine sunlight intensity from different directions.

Two servo motors manage movement:

Horizontal Servo → East/West movement

Vertical Servo → Up/Down movement

Based on the brightness difference between LDR pairs, the Arduino adjusts the servos to align the solar panel with the brightest spot.

🛠 Working Principle:

LDR sensors continuously measure light from four directions.

Readings are averaged to determine top vs. bottom and left vs. right light intensity.

When the difference crosses a predefined threshold, the corresponding servo rotates slightly.

When overall light is too low (evening/night), the system stops tracking and enters standby mode.

During the day, the tracker keeps adjusting smoothly to follow the sun’s movement.

🔧 Mechanical Assembly

LDRs are placed at four corners around a divider for precise detection.

A dual-axis frame (3D printed or acrylic/wood) holds the solar panel.

One servo rotates the entire frame horizontally.

Another servo tilts the panel vertically.

📜 Source Code





🏁 Conclusion

The Dual Axis Solar Tracking System ensures maximum solar energy harvesting by dynamically adjusting the panel to face the sun throughout the day. Using simple components and an Arduino controller, this project offers a practical and effective solution for improving solar efficiency.
