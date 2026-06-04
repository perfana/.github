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

## Core Repository

| Repository | Description |
|------------|-------------|
| [**perfana**](https://github.com/perfana/perfana) | The Perfana platform monorepo — NestJS API, Next.js web app, BullMQ workers (ADAPT regression detection & SLO checks), Grafana sync, MCP server, and shared TypeORM entities. **This is the home of active development.** |

## Integrations & Tooling

| Repository | Description |
|------------|-------------|
| [**perfana-cli**](https://github.com/perfana/perfana-cli) | Command line interface to Perfana. |
| [**helm-charts**](https://github.com/perfana/helm-charts) | Perfana Helm charts. |
| [**perfana-jmeter-timescaledb**](https://github.com/perfana/perfana-jmeter-timescaledb) | JMeter backend listener that writes test results directly to TimescaleDB for real-time performance analysis. |
| [**events-jmeter-maven-plugin**](https://github.com/perfana/events-jmeter-maven-plugin) | Maven plugin to integrate JMeter script with Perfana. |
| [**events-gatling-maven-plugin**](https://github.com/perfana/events-gatling-maven-plugin) | Maven plugin to integrate Gatling script with Perfana. |
| [**event-scheduler-maven-plugin**](https://github.com/perfana/event-scheduler-maven-plugin) | Maven plugin to integrate several test events  with Perfana. |
| [**test-events-neoload**](https://github.com/perfana/test-events-neoload) | Test event to integrate Neoload SAAS with Perfana. |
| [**test-events-command-runner**](https://github.com/perfana/test-events-command-runner) | Test event to run commandline commands in sync with Perfana. |
| [**test-events-test-run-config-command**](https://github.com/perfana/test-events-test-run-config-command) | Test event to capture test run configuration items to store in Perfana. |

---

## 🚀 Demo Environment

To try out Perfana locally with all components and a sample application under test, visit the [**perfana-demo** repository](https://github.com/perfana/perfana-demo).

---

## 📘 License

All repositories are released under the Apache 2.0 license unless otherwise specified.
