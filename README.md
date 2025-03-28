# Intelligent Ladle Car Traffic Management System

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) <!-- Replace with your actual license -->

## Description

This project implements an intelligent traffic management system for ladle cars in industrial settings, particularly steel plants. It leverages real-time detection of ladle cars using a custom-trained neural network and dynamic monitoring of load/unload points to optimize traffic flow and prevent congestion. The system prioritizes safety by implementing a real-time, responsive control mechanism.

## Features

*   **Real-time Ladle Car Detection:** Utilizes a custom-trained neural network for accurate detection of ladle cars.
*   **Dynamic Load/Unload Point Monitoring:** Tracks the number of ladle cars entering and exiting each load/unload point.
*   **Intelligent Traffic Signal Control:** Automatically adjusts traffic signals based on real-time ladle car counts, preventing congestion.
    *   **Red Signal Trigger:** Sets all signals to RED when the difference between exit and entry counts at a point exceeds a threshold, preventing potential collisions.
    *   **Green Signal Enablement:** Returns signals to GREEN when the difference falls below or equals the threshold, resuming normal traffic flow.
*   **Scalable Architecture:** Designed to accommodate a large number of ladle cars without performance degradation.

## Philosophy

*   **Safety-First:** Prioritizes the safe and efficient movement of molten metal.
*   **Real-Time Responsiveness:** Operates in real-time, adjusting traffic flow based on current conditions.
*   **Data-Driven Decisions:** Relies on accurate data from the neural network and count monitoring.

## Assumptions

*   Multiple ladle cars can exit/enter a load/unload point simultaneously.
*   Idle ladle cars will not be present on the road.

## Getting Started

### Prerequisites

*   Python 3.x
*   TensorFlow / PyTorch 


### Installation

1.  Clone the repository:
    ```
    git clone (copy the url)
    cd (inside the repo)
    ```
2.  Install dependencies:
    ```
    pip install -r requirements.txt

    ```
3.  Download the pre-trained weights for the Ladle car detection model from repo.

4.  Configure the system by updating the necessary configuration parameters such as the IP addresses of the industrial camera and the load-unload points in the "config.ini" file

### Usage

1.  Run the main script:
    ```
    python main.py
    ```


## Contributing

Contributions are welcome! Please feel free to submit pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

*   Credit any individuals, organizations, or resources that contributed to the project.

## Contact

Prashant Kumar - kumarprashant0797@gmail.com

https://kumarprashant0797.github.io
