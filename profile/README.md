# Pisom Platform

Pisom is an API-first platform built to demonstrate high-scale engineering and full-cycle development practices.

The project focuses on building a safe and reliable environment for financial transactions.

## Main Goals
- **API-First**: Design the contract (OpenAPI) before writing any code.
- **Resilience**: Built-in mechanisms to handle failures, such as **Idempotency** (preventing double processing) and **Retries**.
- **Real Infrastructure**: Automated tests using **Testcontainers** (running real databases like PostgreSQL during tests).
- **Full Observability**: Monitoring the system health using logs and metrics (Grafana/CloudWatch).

## Project Structure

### Services (The Apps/Deployables)
- **`pisom-charges-service`**: Manages the life of a charge (Creation, Authorization, Success/Fail).
- **`pisom-payments-service`**: Integration with external **PSPs** (Payment Service Providers / Gateways).

### Foundation & Tools
- **`pisom-architecture`**: Documentation of technical decisions (**ADRs** - Architecture Decision Records).
- **`pisom-core`**: Shared libraries and common rules used by all services.
- **`pisom-test-platform`**: The "Quality Guard" – Integration and E2E (End-to-End) test suites.
- **`pisom-observability`**: Standards for monitoring and logging.
