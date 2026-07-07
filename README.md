## Hardware & Setup Notes

Pin Connections: Please refer to the pin_connections.txt file for the exact wiring layout.

Circuit Diagram: The included circuit_diagram(for reference only).png is provided for visual context and general knowledge. Always verify your specific board's pinout before powering the system.

Interface: Check Adafruit UI.png to see the intended dashboard layout.

## Machine Learning Integration

While this repository currently focuses on the hardware foundation and sensor data collection, the system architecture is designed to support advanced predictive analytics.

Here is how Machine Learning can be integrated into this pipeline in upcoming versions:

Behavioral Baseline Modeling: The current sensors can gather continuous, time-series data on movement and room presence. This data can be used to train an unsupervised learning model to establish a "normal" behavioral baseline for a patient.

Anomaly Detection: Once a baseline is established, the ML model can monitor live sensor feeds to flag unusual patterns (e.g., increased nighttime wandering, irregular pacing, or prolonged inactivity) that may indicate a decline in cognitive state or an immediate safety risk.

Edge Machine Learning: To ensure patient privacy and reduce system latency, future updates will focus on deploying lightweight, optimized models directly to the microcontrollers. Processing the data locally on the edge means sensitive behavioral data does not need to be continuously streamed to a cloud server.

Implementation Steps:

Export raw sensor data to CSV logs.

Label datasets based on standard behavioral metrics.

Train a lightweight neural network or decision tree model.

Compile the model for edge deployment and flash it to the hardware alongside the existing control logic.
## Project Resources & Roadmap

Datasheets: Included PDF datasheets for the main components used in this build for technical reference.

Future Enhancements: Check the future_enhancements file to see the planned upgrades, upcoming features, and roadmap for this project.
