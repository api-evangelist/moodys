# Moody's (moodys)
Moody's provides a comprehensive suite of APIs spanning KYC compliance, economic data and forecasting, credit risk analytics, insurance and catastrophe modeling, climate risk, commercial real estate, and news aggregation.

**URL:** [Visit APIs.json URL](https://github.com/api-search/moodys/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Climate Risk, Compliance, Credit Risk, Economic Data, Entity Verification, Financial Analytics, Insurance, KYC, Risk, Screening

## Timestamps

- **Created:** 2024-09-25
- **Modified:** 2026-04-18

## APIs

### Moody's Data Buffet API
Moody's Analytics Data Buffet API enables retrieval of economic, demographic and financial time series data and forecasts.

**Human URL:** [https://www.economy.com/products/tools/data-buffet](https://www.economy.com/products/tools/data-buffet)

#### Tags:

 - Demographics, Economic Data, Forecasts, Time Series

#### Properties

- [Documentation](https://api.economy.com/data/v1/swagger)
- [GitHubOrganization](https://github.com/moodysanalytics/databuffet-api-codesamples)
- [OpenAPI](openapi/moodys-data-buffet-api-openapi.yml)
- [JSONSchema](json-schema/moodys-time-series-schema.json)
- [JSONLD](json-ld/moodys-context.jsonld)

## Common Properties

- [Portal](https://www.kompany.com/)
- [Plans](https://www.kompany.com/kycapi/dashboard/plans)
- [GettingStarted](https://www.kompany.com/kycapi/docs/guides/guides/get-started)
- [Console](https://www.kompany.com/kycapi/console)
- [Sandbox](https://www.kompany.com/kycapi/docs/guides/guides/get-started/sandbox-overview)
- [UseCases](https://www.kompany.com/kycapi/docs/guides/guides/use-cases)
- [Resources](https://www.kompany.com/kycapi/docs/resources)
- [StatusPage](https://kycapi-status.kompany.com/)
- [Portal](https://hub.moodysanalytics.com/)
- [Documentation](https://hub.moodysanalytics.com/products)
- [GettingStarted](https://hub.moodysanalytics.com/gettingstarted)
- [Contact](https://hub.moodysanalytics.com/contact)
- [Portal](https://developer.rms.com/)
- [GitHubOrganization](https://github.com/moodysanalytics)

## Features

| Name | Description |
|------|-------------|
| Economic Time Series Data | Access to international and subnational economic, demographic, and financial time series data and forecasts. |
| Credit Risk Analytics | Probability of default calculations for 400 million companies globally through the EDF-X model. |
| Climate Risk Modeling | Physical climate risk assessment leveraging the Intelligent Risk Platform for financial services. |
| KYC Compliance | Know Your Customer verification, anti-money laundering screening, and entity verification capabilities. |
| Scenario Analysis | Custom scenario generation using the Global Macroeconomic Model for stress testing and forecasting. |

## Use Cases

| Name | Description |
|------|-------------|
| Credit Risk Assessment | Evaluate counterparty credit risk using EDF-X probability of default and loss given default models. |
| Regulatory Stress Testing | Generate stress scenarios for DFAST, CCAR, and EBA regulatory compliance testing. |
| Commercial Lending | Automate financial spreading and credit analysis workflows for commercial loan underwriting. |
| Catastrophe Modeling | Model insurance portfolio risk exposure using catastrophe models and location intelligence. |

## Integrations

| Name | Description |
|------|-------------|
| Orbis Database | Integration with the Orbis database covering 400 million companies for credit risk analysis. |
| Intelligent Risk Platform | Platform integration for catastrophe modeling, underwriting, and reinsurance workflows. |
| News Sources | Integration with 24,000+ news sources for real-time media monitoring and sentiment analysis. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Moody's Data Buffet API](openapi/moodys-data-buffet-api-openapi.yml)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Data Buffet API](capabilities/shared/data-buffet.yaml) -- 16 operations for time series, baskets, orders, search, and reference data

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Economic Data Analytics](capabilities/economic-data-analytics.yaml) | Data Buffet | 16 | Economist / Data Scientist |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
