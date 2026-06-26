# Unitree Robot SDK Version 2
Unitree Robot SDK Version 2 is a comprehensive software development kit designed to provide a seamless and efficient way to interact with Unitree robots. This SDK is built on top of a robust architecture, allowing developers to create a wide range of applications, from simple robotic tasks to complex autonomous systems.

## Project Description
The Unitree Robot SDK Version 2 is designed to provide a unified interface for controlling and interacting with Unitree robots. The SDK includes a set of APIs, libraries, and tools that enable developers to create custom applications, integrate with existing systems, and leverage the capabilities of Unitree robots. With this SDK, developers can focus on building innovative solutions, rather than spending time on low-level details.

### Tech Stack
The Unitree Robot SDK Version 2 is built using a combination of cutting-edge technologies, including:
* **Programming Languages:** C++, Python
* **Frameworks:** CMake, Eigen, Boost
* **Libraries:** YAML, SPDLog, Fmt
* **Operating Systems:** Ubuntu 20.04 LTS (aarch64 and x86_64)

## Installation and Startup
To get started with the Unitree Robot SDK Version 2, follow these steps:

### Prerequisites
* Install the required dependencies: `apt-get update` and `apt-get install -y cmake g++ build-essential libyaml-cpp-dev libeigen3-dev libboost-all-dev libspdlog-dev libfmt-dev`

### Building the SDK
1. Create a build directory: `mkdir build`
2. Navigate to the build directory: `cd build`
3. Run CMake: `cmake ..`
4. Build the SDK: `make`

### Installing the SDK
To install the SDK system-wide, run: `sudo make install`
Alternatively, to install the SDK to a custom directory, run: `cmake .. -DCMAKE_INSTALL_PREFIX=/opt/unitree_robotics` and then `sudo make install`

## Basic Usage
The Unitree Robot SDK Version 2 provides a simple and intuitive API for interacting with Unitree robots. Here are some basic examples:

### State Machine Example
The `example/state_machine` directory contains a sample state machine implementation. To use this example, create a `params.json` file with the following contents:
```json
{
    "dt": 0.01,
    "kp": 40.0,
    "kd": 1.0,
    "init_pos": [
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8,
        0.0,
        0.9,
        -1.8
    ]
}
```
Then, build and run the example using: `mkdir build`, `cd build`, `cmake ..`, `make`, and `./state_machine`

### H1 Parallel Mechanism Control Example
The `example/h1` directory contains a sample implementation of the H1 parallel mechanism control interface. This example demonstrates how to control the ankle joints of the H1 robot using the `PR Mode` interface.

## Contributing
The Unitree Robot SDK Version 2 is an open-source project, and we welcome contributions from the community. To contribute, please fork the repository, make your changes, and submit a pull request.

## Licensing
The Unitree Robot SDK Version 2 is licensed under the [MIT License](https://opensource.org/licenses/MIT). By using this SDK, you agree to the terms and conditions of the license.

## Additional Resources
For more information about the Unitree Robot SDK Version 2, please visit the [Unitree Document Center](https://support.unitree.com/home/zh/developer).