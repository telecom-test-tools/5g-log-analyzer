# 5G Log Analyzer

A Python script that parses 5G gNodeB logs to detect attach flows, RRC failures, and setup failures. It calculates attach success rates and provides a summarized report of the events found in the log file.

## Features

- Parses gNodeB logs for specific 3GPP messages:
  - Attach Requests, Accepts, and Rejects
  - RRC Rejects / RRCConnectionReject
  - Setup Failures
- Calculates Attach Success Rate.
- Provides a high-level test summary and detailed statistics.

## Prerequisites

- Python 3.x

## Usage

Run the analyzer script by passing the path to the log file as an argument:

```bash
python analyzer.py <path_to_log_file>
```

For example, if you have a `sample_logs.txt` file:

```bash
python analyzer.py sample_logs.txt
```

## Example Output

```text
Test Summary:
  Attach Success Rate: 98%
  RRC Failures: 2
  Setup Failures: 1

Detailed Stats:
  Total Attach Attempts: 100
  Total Attach Successes: 98
  Total Attach Rejects: 2
```

## Installation

```bash
pip install .
```

## Usage

Run the analyzer on a gNodeB log file:

```bash
5g-log-analyzer <path_to_log_file>
```

## 🌐 Part of Telecom Test Toolkit

This project is part of the **Telecom Test Toolkit ecosystem**.

Other tools:
- [telecom-test-toolkit](https://github.com/telecom-test-tools/telecom-test-toolkit) (Orchestrator)
- [testwatch](https://github.com/telecom-test-tools/testwatch)
- [5gtestscope](https://github.com/telecom-test-tools/5gtestscope)
- [Regression-Flakiness-Scorer](https://github.com/telecom-test-tools/Regression-Flakiness-Heatmap-Scorer)
- [test-report-gen](https://github.com/telecom-test-tools/test-report-gen)
- [test-monitor-dashboard](https://github.com/telecom-test-tools/test-monitor-dashboard)

🔗 Main project:
https://github.com/telecom-test-tools/telecom-test-toolkit
