# 📱 Maestro Demo: Android Virtual Device Testing

[![Maestro](https://img.shields.io/badge/Tested_with-Maestro-blue.svg)](https://maestro.mobile.dev/)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)]()

Welcome to the **Maestro Test** repository! This project serves as a simply demonstration of automating mobile UI tests on Android Virtual Devices (AVDs) using the [Maestro](https://maestro.mobile.dev/) test framework.

## 🎯 Overview

This repository provides practical examples of End-to-End (E2E) mobile testing. It includes a sample Android application (`techshop.apk`) and a suite of Maestro test flows that cover various user scenarios, such as authentication, product browsing, and cart management. The project also features automated HTML test report generation and CI/CD integration setups.

## 📂 Repository Structure

Here is a high-level overview of the project's structure:

```text
maestro-demo/
├── .github/                 # GitHub Actions workflows for CI/CD
├── flows/                   # Maestro test scenarios
│   ├── elements/            # Reusable UI element definitions
│   ├── subflows/            # Reusable subflows (e.g., setup, login)
│   ├── 01-login-success.yaml
│   ├── 02-login-fail.yaml
│   └── ...                  # Other E2E test scenarios (cart, products)
├── generate-report.js       # Node.js script to generate visual HTML reports
├── techshop.apk             # Sample Android application under test (AUT)
└── README.md                # Project documentation (this file)
```

## 🚀 Getting Started

1. **Install Maestro**: Follow the [official Maestro installation guide](https://maestro.mobile.dev/getting-started/installing-maestro).
2. **Start an Emulator**: Launch your preferred Android Virtual Device.
3. **Install the App**: Install the provided `techshop.apk` on your running emulator.
4. **Run Tests**: Execute this command:
   ```bash
   maestro test flows
   ```
4. **Run Tests with Tes Report**: Execute this command:
   ```bash
   maestro test flows --format junit --output report.html
   ```

---
*Happy Testing!* 🚀
