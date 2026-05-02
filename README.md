# SaaS Alerts

SaaS Alerts is a SaaS security monitoring platform purpose-built for Managed Service Providers (MSPs). The platform detects anomalous user behavior, data exfiltration, account compromise, and unauthorized access across cloud applications including Microsoft 365, Google Workspace, Salesforce, Slack, and Dropbox. Key capabilities include machine learning-based threat detection, automated remediation workflows, multi-tenant MSP management, and integration with PSA and RMM platforms. SaaS Alerts was acquired by Kaseya in 2023.

**Website:** [https://www.saasalerts.com](https://www.saasalerts.com)
**API Documentation:** [https://help.saasalerts.kaseya.com/help/Content/How-To/using-the-saas-alerts-api.htm](https://help.saasalerts.kaseya.com/help/Content/How-To/using-the-saas-alerts-api.htm)
**APIs.yml:** [https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/apis.yml)

## APIs

### SaaS Alerts API (v0.20.0)

REST API providing programmatic access to the SaaS Alerts security monitoring platform. Eight methods including GET and POST operations for event querying and reporting. Authentication uses API keys generated in the management interface (passed in `X-API-Key` header).

- **Base URL:** `https://api.saasalerts.com`
- **Documentation:** [https://help.saasalerts.kaseya.com/help/Content/How-To/using-the-saas-alerts-api.htm](https://help.saasalerts.kaseya.com/help/Content/How-To/using-the-saas-alerts-api.htm)
- **OpenAPI:** [openapi/saas-alerts-openapi.yml](openapi/saas-alerts-openapi.yml)
- **SwaggerHub:** [https://app.swaggerhub.com/apis/SaaS_Alerts/functions/0.20.0](https://app.swaggerhub.com/apis/SaaS_Alerts/functions/0.20.0)

### Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/reports/events` | List security events with filtering |
| POST | `/reports/event/query` | Execute structured JSON event query |
| GET | `/reports/alerts` | List security alerts |
| GET | `/reports/customers` | List monitored customers |
| GET | `/reports/users` | List monitored users |

## OpenAPI Specifications

| API | File |
|-----|------|
| SaaS Alerts API | [openapi/saas-alerts-openapi.yml](openapi/saas-alerts-openapi.yml) |

## Capabilities

| Capability | Description |
|-----------|-------------|
| [capabilities/msp-security-monitoring.yaml](capabilities/msp-security-monitoring.yaml) | Unified MSP SaaS security monitoring and incident response |

### Shared Definitions

| API | File |
|-----|------|
| SaaS Alerts API | [capabilities/shared/saas-alerts.yaml](capabilities/shared/saas-alerts.yaml) |

## JSON Schema

| Schema | File |
|--------|------|
| Security Event | [json-schema/saas-alerts-security-event-schema.json](json-schema/saas-alerts-security-event-schema.json) |
| Security Alert | [json-schema/saas-alerts-alert-schema.json](json-schema/saas-alerts-alert-schema.json) |

## JSON Structure

| Structure | File |
|-----------|------|
| Security Event | [json-structure/saas-alerts-security-event-structure.json](json-structure/saas-alerts-security-event-structure.json) |

## JSON-LD

| Context | File |
|---------|------|
| SaaS Alerts Context | [json-ld/saas-alerts-context.jsonld](json-ld/saas-alerts-context.jsonld) |

## Examples

| Example | File |
|---------|------|
| List Security Events | [examples/saas-alerts-list-security-events-example.json](examples/saas-alerts-list-security-events-example.json) |
| Query Security Events | [examples/saas-alerts-query-security-events-example.json](examples/saas-alerts-query-security-events-example.json) |

## Rules

| Ruleset | File |
|---------|------|
| SaaS Alerts Spectral Rules | [rules/saas-alerts-spectral-rules.yml](rules/saas-alerts-spectral-rules.yml) |

## Vocabulary

| Vocabulary | File |
|-----------|------|
| SaaS Alerts Vocabulary | [vocabulary/saas-alerts-vocabulary.yml](vocabulary/saas-alerts-vocabulary.yml) |

## Supported Applications

SaaS Alerts monitors security events across:

- Microsoft 365
- Google Workspace
- Salesforce
- Slack
- Dropbox

## Tags

MSP, SaaS Security, Security Monitoring, Threat Detection, Microsoft 365, Google Workspace, MSSP

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
