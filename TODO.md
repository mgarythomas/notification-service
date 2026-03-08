# Notification Service TODOs

## Initial Setup & Specifications
- [x] Define what a standardized notification service will do (Specification Docs).
- [x] Define REST API OpenAPI specification (Contract First).

## Base Project Configuration
- [x] Initialize Spring Boot (Java LTS, Gradle) for Internal VPC services.
- [ ] Set up infrastructure architecture:
  - [ ] Provision Internal VPC.
  - [ ] Provision Internal API Gateways.
  - [ ] Deploy EKS cluster in the Internal VPC.

## Architecture & Implementation
- [x] Implement Hexagonal Architecture (Ports and Adapters).
- [x] Support templating of notifications.
- [x] Enable support for single and multiple notifications in a single request.
- [x] Audit all notifications (track source and destination).
- [ ] Integrate with OpenTelemetry for observability.
- [x] Enable feature flagging using OpenFeature standard.

## Integrations & Adapters
- [x] Define outward ports to delegate to third-party services (SMTP, Email, SMS, WhatsApp, Signal, Bluesky, X).
- [x] Implement initial adapter for Salesforce Email API. (initial implementation).

## Simulator & Testing
- [x] Build a separate notification simulator to capture and record all requests to a CSV file.
- [x] Build a query implementation for the simulator logs using DuckDB.
- [x] Implement automated Playwright tests for the API.

## Documentation
- [x] Integrate design specification into the primary README.md.
