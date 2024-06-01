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

git clone https://github.com/yourusername/5G-AKA-simulation-in-C.git
cd 5G-AKA-simulation-in-C
## usage
-i: Input file for simulation parameters.
-o: Output file for simulation results.


./aka_simulation

./aka_simulation -i input.txt -o output.txt

## project-structure

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
