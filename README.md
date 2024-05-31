# JMeter Testing Framework

## Overview

This framework allows you to run JMeter tests dynamically based on configuration files. It includes scripts to run tests, archive reports, and generate HTML reports.

## Directory Structure

```plaintext
jmetr/
├── .github/
│   └── workflows/
│       └── action.yml
├── jmeter/
│   ├── tests/
│   │   ├── smoke/
│   │   │   ├── smoke_test1.jmx
│   │   │   ├── smoke_test2.jmx
│   │   │   └── ...
│   │   ├── regression/
│   │   │   ├── regression_test1.jmx
│   │   │   ├── regression_test2.jmx
│   │   │   └── ...
│   │   └── performance/
│   │       ├── perf_test1.jmx
│   │       ├── perf_test2.jmx
│   │       └── ...
│   ├── functions/
│   │   ├── test_setup.jmx
│   │   ├── test_teardown.jmx
│   │   ├── common_functions.jmx
│   │   └── custom_assertions.jmx
│   └── config/
│       ├── environments/
│       │   ├── dev.properties
│       │   ├── staging.properties
│       │   └── prod.properties
│       ├── config.properties
│       ├── user.properties
│       └── test_execution.properties
├── taurus/
│   ├── configs/
│   │   ├── smoke.yml
│   │   ├── regression.yml
│   │   └── performance.yml
│   ├── global.yml
│   └── extensions/
│       └── custom_extensions.py
├── reports/
│   ├── latest/
│   │   ├── index.html
│   │   ├── jmeter/
│   │   └── taurus/
│   └── archive/
│       ├── 2024-05-31/
│       │   ├── index.html
│       │   ├── jmeter/
│       │   └── taurus/
│       └── ...
├── scripts/
│   ├── run_tests.sh
│   ├── archive_reports.sh
│   └── generate_reports.sh
├── version.txt
└── README.md
