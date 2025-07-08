# Perfana

**Perfana** is an open source performance observability platform designed to automate the validation, visualization, and reporting of performance test results. It empowers teams to continuously monitor performance trends and enforce performance goals during the software delivery lifecycle.

Perfana integrates seamlessly with popular test tools (like Gatling, JMeter, and k6), CI/CD pipelines, and monitoring systems (such as Grafana and Dynatrace), making it easy to shift performance testing left and catch regressions early.

## Key Features
* Automated validation of performance metrics using configurable thresholds
* Rich visualization and dashboards for test runs using Grafana
* Time series comparison between test runs
* Integration with CI pipelines: Use Perfana as quality gate
* Automated configuration of Grafana dashboards base on profiles / metric discovery


---

## Core Repositories

| Repository | Description |
|------------|-------------|
| [**perfana-fe**](https://github.com/perfana/perfana-fe) | The front-end of Perfana, used to manage test runs, visualize performance test results and configure settings. |
| [**perfana-grafana**](https://github.com/perfana/perfana-grafana) | Handles Grafana dashboards integration and automated configuration. |
| [**perfana-snapshot**](https://github.com/perfana/perfana-snapshot) | Creates Grafana dashboard snapshots to save performance test result dashboards beyond data retention. |
| [**perfana-ds**](https://github.com/perfana/perfana-ds) | Services for statistical regression detection and automated service level objectives checks. |

## Other Repositories

| Repository | Description |
|------------|-------------|
| [**helm-charts**](https://github.com/perfana/helm-charts) | Perfana Helm charts. |
| [**events-jmeter-maven-plugin**](https://github.com/perfana/events-jmeter-maven-plugin) | Maven plugin to integrate JMeter script with Perfana. |
| [**events-gatling-maven-plugin**](https://github.com/perfana/events-gatling-maven-plugin) | Maven plugin to integrate Gatling script with Perfana. |
| [**event-scheduler-maven-plugin**](https://github.com/perfana/event-scheduler-maven-plugin) | Maven plugin to integrate several test events  with Perfana. |
| [**test-events-neoload**](https://github.com/perfana/test-events-neoload) | Test event to integrate Neoload SAAS with Perfana. |
| [**test-events-command-runner**](https://github.com/perfana/test-events-command-runner) | Test event to run commandline commands in sync with Perfana. |
| [**test-events-test-run-config-command**](https://github.com/perfana/test-events-neoload) | Test event to capture test run configuration items to store in Perfana. |

---

## 🚀 Demo Environment

To try out Perfana locally with all components and a sample application under test, visit the [**perfana-demo** repository](https://github.com/perfana/perfana-demo).

---

## 📘 License

All repositories are released under the Apache 2.0 license unless otherwise specified.
