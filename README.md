```markdown
# 5G-AKA Simulation in C

This project provides a simulation of the 5G Authentication and Key Agreement (AKA) protocol implemented in C. The 5G-AKA protocol is used for secure communication in 5G networks, ensuring mutual authentication between the user equipment and the network.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Key Features](#key-features)

## Introduction

The 5G-AKA protocol is a critical component in the 5G security architecture. This project simulates the 5G-AKA protocol, demonstrating how mutual authentication and key agreement are achieved between the user equipment (UE) and the network. This simulation can be used for educational purposes, research, and testing.

## Installation

### Prerequisites

Before you begin, ensure you have the following tools installed:
- **GCC**: GNU Compiler Collection
- **Make**: Build automation tool

### Libraries Required

The project requires the following libraries:
- **libnm**: Network management library
- **OpenSSL**: Library for SSL and TLS

You can install these libraries on a Debian-based system using:
```sh
sudo apt-get update
sudo apt-get install build-essential libssl-dev libnm-dev
```

### Steps to Install

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/5G-AKA-simulation-in-C.git
    cd 5G-AKA-simulation-in-C
    ```

2. **Build the project**:
    ```sh
    make
    ```

## Usage

After building the project, you can run the simulation using the following command:
```sh
./aka_simulation
```

### Command Line Options

You can customize the simulation by using the following command line options:
- `-i`: Input file for simulation parameters.
- `-o`: Output file for simulation results.

Example:
```sh
./aka_simulation -i input.txt -o output.txt
```

### Configuration

The input file should contain the necessary parameters for the 5G-AKA simulation, such as user credentials and network settings. An example of the input file format is as follows:

```plaintext
UE_ID: user1
K: 1234567890abcdef1234567890abcdef
OPC: 1234567890abcdef1234567890abcdef
SQN: 000000000001
AMF: 8000
```

### Running the Simulation

1. Prepare an input file with the required parameters.
2. Run the simulation:
    ```sh
    ./aka_simulation -i input.txt -o output.txt
    ```
3. Check the output file for the results of the simulation, which will include the authentication vectors and keys generated during the simulation.

## Project Structure

Here is an overview of the project's structure:

```
5G-AKA-simulation-in-C/
├── SEAF/
│   └── NetworkManager-master/
│       ├── libnm/
│       ├── libnm-core/
│       ├── libnm-glib/
│       ├── libnm-util/
│       ├── introspection/
│       ├── man/
│       ├── m4/
│       ├── po/
│       ├── src/
│       ├── test/
│       └── tools/
├── LICENSE
└── README.md
```

### Key Components

- **SEAF/NetworkManager-master/**: Contains various modules and utilities related to network management required for the simulation.
- **libnm**: Network management library.
- **src/**: Source files for the 5G-AKA simulation.
- **test/**: Test files for the simulation.

#### src/

This directory contains the main source code for the simulation. Key files include:
- `aka_simulation.c`: The main program that runs the 5G-AKA simulation.
- `aka_functions.c`: Functions implementing the 5G-AKA protocol.
- `aka_utils.c`: Utility functions used in the simulation.

#### test/

This directory contains test cases and scripts used to verify the correctness of the simulation. Key files include:
- `test_aka_simulation.c`: Test cases for the 5G-AKA simulation.
- `test_vectors/`: Directory containing predefined test vectors for verification.

## Key Features

- **Mutual Authentication**: Ensures both the user and the network authenticate each other.
- **Secure Communication**: Utilizes encryption for secure data transmission.
- **Configurable Simulation**: Allows customization of simulation parameters through input files.
- **Educational Tool**: Provides a practical example of the 5G-AKA protocol for learning and research purposes.

---
```
