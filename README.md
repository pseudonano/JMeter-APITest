# JMeter-APITest

A simple project containing a JMeter test plan to test API endpoints.  
This repository currently includes a JMeter `.jmx` file (`ExploreJMeter.jmx`) as the main test definition.

## Table of Contents

- [Overview](#overview)  
- [Prerequisites](#prerequisites)  
- [Usage](#usage)  
  - [Run via GUI](#run-via-gui)  
  - [Run in Non-GUI / CLI Mode](#run-in-non-gui--cli-mode)  
- [Test Structure](#test-structure)  
- [Extending / Customizing](#extending--customizing)  
- [Troubleshooting](#troubleshooting)  
- [Contributing](#contributing)  
- [License](#license)

## Overview

This repository hosts a JMeter test plan for API testing. Use it as a starting point to build your own API performance or functional tests using JMeter.

Currently included:

- `ExploreJMeter.jmx` — a sample JMeter test plan.  
  :contentReference[oaicite:0]{index=0}

## Prerequisites

Before running the tests, make sure you have:

- Java (JDK or JRE) installed (version ≥ 8 recommended)  
- Apache JMeter (download from [jmeter.apache.org](https://jmeter.apache.org))  
- (Optional) Additional HTTP libraries, plugins, or dependencies if your test plan uses them

## Usage

### Run via GUI

1. Launch JMeter (`jmeter` command or via GUI executable).  
2. Open the `ExploreJMeter.jmx` file.  
3. Edit or configure endpoints, assertions, variables as needed.  
4. Run the test (via **Run → Start**).  

   > Note: GUI mode is good for test development and debugging, but not recommended for large-scale or long-running load tests.  
   :contentReference[oaicite:1]{index=1}  

### Run in Non-GUI / CLI Mode

To run the test in non-GUI (headless) mode, use:

```bash
jmeter -n -t ExploreJMeter.jmx -l results.jtl -e -o report-output-dir
