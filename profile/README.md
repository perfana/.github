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

> ℹ️ Perfana has been consolidated into a single monorepo. The previously
> separate `perfana-fe`, `perfana-grafana`, `perfana-snapshot`, and `perfana-ds`
> repositories are superseded by the [**perfana**](https://github.com/perfana/perfana) monorepo and kept for reference only.

## Integrations & Tooling

| Repository | Description |
|------------|-------------|
| [**helm-charts**](https://github.com/perfana/helm-charts) | Perfana Helm charts. |
| [**events-jmeter-maven-plugin**](https://github.com/perfana/events-jmeter-maven-plugin) | Maven plugin to integrate JMeter script with Perfana. |
| [**events-gatling-maven-plugin**](https://github.com/perfana/events-gatling-maven-plugin) | Maven plugin to integrate Gatling script with Perfana. |
| [**event-scheduler-maven-plugin**](https://github.com/perfana/event-scheduler-maven-plugin) | Maven plugin to integrate several test events  with Perfana. |
| [**test-events-neoload**](https://github.com/perfana/test-events-neoload) | Test event to integrate Neoload SAAS with Perfana. |
| [**test-events-command-runner**](https://github.com/perfana/test-events-command-runner) | Test event to run commandline commands in sync with Perfana. |
| [**test-events-test-run-config-command**](https://github.com/perfana/test-events-test-run-config-command) | Test event to capture test run configuration items to store in Perfana. |

## Legacy / Superseded Repositories

These repositories have been consolidated into the [**perfana**](https://github.com/perfana/perfana) monorepo and are no longer the primary development target.

| Repository | Superseded by |
|------------|---------------|
| [**perfana-fe**](https://github.com/perfana/perfana-fe) | `apps/web` + `apps/api` in the monorepo |
| [**perfana-grafana**](https://github.com/perfana/perfana-grafana) | `apps/grafana-sync` in the monorepo |
| [**perfana-snapshot**](https://github.com/perfana/perfana-snapshot) | Snapshot handling in the monorepo |
| [**perfana-ds**](https://github.com/perfana/perfana-ds) | `apps/worker` (ADAPT regression detection & SLO checks) in the monorepo |

---

## 🚀 Demo Environment

To try out Perfana locally with all components and a sample application under test, visit the [**perfana-demo** repository](https://github.com/perfana/perfana-demo).

---

## 📘 License

All repositories are released under the Apache 2.0 license unless otherwise specified.
